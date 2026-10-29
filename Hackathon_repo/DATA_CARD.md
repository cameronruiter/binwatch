# Ethical reflection: BinWatch data card

**BinWatch** | AI for Good, Hackathon 7 "Eyes on Earth" | SDG 15 | Cameron Ruiter and Nina Borutyńska

## Data card

| | |
|---|---|
| **What** | Photos of underground rubbish containers in The Hague and the area around them |
| **How** | 7 videos we filmed ourselves with our phones in October 2026, day, evening and night, at a few streets in The Hague. We took 3–4 frames per second and removed blurry and near-duplicate frames. |
| **Labels** | `bag`, `torn_bag`, `loose_litter`, `dumped_item`, with boxes drawn by hand in Roboflow. Cameron did the labelling with help from Claude (an AI assistant) and checked the results. Photos of clean bins are kept with no boxes, so the model also learns "nothing to do". |
| **Size** | 300 labelled images, split 211 train / 60 validation / 29 test. About 23 of them are clean bins. |
| **Privacy** | We never labelled people, cars or bikes. 21 frames with a readable number plate were removed. The original videos are not published. |
| **Model** | Roboflow RF-DETR (Small), trained in Roboflow |

**Limits:** only a few streets in one city, only autumn (gulls are worst in spring and summer), not many torn bags (the most important class), and WhatsApp made the videos less sharp.

## Results and how honest they are

On Roboflow's test set the model scored **mAP@50 89.6%, precision 88.5% and recall 86.4%**.

| Class | Found | Missed | False alarms |
|---|---|---|---|
| `torn_bag` | 9 of 9 | 0 | 0 |
| `bag` | 12 of 13 | 1 | 1 |
| `dumped_item` | 13 of 15 | 2 | 2 |
| `loose_litter` | 6 of 9 | 3 | 2 |

These numbers look better than they really are:

- **The test images come from the same videos as the training images.** Frames from one video look almost the same, so the model has seen near-copies of its test images. On a street we never filmed, the score will be lower.
- **The test set is small** (29 images), so one mistake changes the score by several percent.
- **The perfect `torn_bag` score is based on very few real bags**, mostly the same bag filmed from different angles. It does not prove the model recognises torn bags in general.
- **Loose litter is the weakest class.** On a new photo of scattered litter, the app correctly said *Clear first*, but at 0.40 it found the bigger pieces and missed many small ones.

## Where it can go wrong

- **It sees damage, not the cause.** A bag torn by a rat looks the same as one torn by a gull, so it can't be used to count gull damage. Using it as evidence against gulls would also be unfair: wild birds, including gulls, are protected in the Netherlands.
- **It misses things.** In the dark, with small litter, or when a bag is just outside the photo. Then a dirty bin gets "Clean" and has to wait, which is the worst mistake it can make. A wrong "Clear first" only costs a short trip. So BinWatch should help decide the order of the route, not replace it.

## Who takes the photos

We decided that residents will report a bin with a photo. We left out a camera on the collection truck (filming streets every day is too close to surveillance), the crew itself (if they're already at the bin they can just clear it) and officers (they give fines, and BinWatch is not for that).

Our choice has risks too:

- **Some neighbourhoods report more than others**, so quiet areas could get less help. → BinWatch only sets the order of reported bins; the normal route stays the same for everyone.
- **Photos can show neighbours, house numbers or number plates.** → Blur them automatically and delete the photo once the bin is cleared.
- **Someone could use it to get a neighbour in trouble.** → The app only shows the bin and the rubbish, never who left it, and results are never used for fines.

## What we did and what's next

**Done:** removed number plate frames, added clean-bin photos, tested the app on a new photo, and the app itself says it's only a hint for route planning, never proof for fines.
**Next:** test on bins we never filmed for training, automatic blurring, more torn bags from different bins, film in spring and summer, test night photos separately.

**Who did what.** Cameron and Nina filmed the videos. Cameron labelled the data, trained the model and built and deployed the app, with Claude helping with the labelling and the app code. Nina wrote the README, this ethical reflection and the slides, with Claude helping with the texts and slides.
