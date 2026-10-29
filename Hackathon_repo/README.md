# Week 7 · Hackathon 7 "Eyes on Earth": BinWatch

**Which bin should the crew clear first?** BinWatch looks at photos of The Hague's underground rubbish containers, finds bags and litter left beside them, and ranks the bins so crews clear the worst ones before gulls spread the rubbish.

**SDG 15: Life on Land** | AI for Good, Hackathon 7 | Cameron Ruiter and Nina Borutyńska

| | |
|---|---|
| 🌐 **Live app** | [binwatch.streamlit.app](https://binwatch.streamlit.app) |
| 📦 **Code repository** | [github.com/cameronruiter/binwatch](https://github.com/cameronruiter/binwatch) |
| ⚖️ **Ethical reflection (data card)** | [DATA_CARD.md](DATA_CARD.md) |
| 🎞️ **Presentation** | [BinWatch slides (PDF)](BinWatch_slides_final.pptx.pdf) |
| 🌍 **SDG 15** | [sdgs.un.org/goals/goal15](https://sdgs.un.org/goals/goal15) |

## What it does
You upload photos of underground containers in The Hague. Our Roboflow model, trained on photos we took ourselves, looks for 4 things around the bin: closed bags (`bag`), bags torn open (`torn_bag`), loose rubbish (`loose_litter`) and other things people dumped, like cardboard or a rolled-up rug (`dumped_item`). The app then tells you which bins to clear first.

## The problem
People in The Hague often leave rubbish bags next to the container instead of in it. Gulls rip the bags open and the rubbish spreads over the street, into parks and canals. The city even hands out free extra-strong bags because gulls peck through normal ones [1]. In 2025, illegally dumped bulky waste rose to 11.2 million kilos, and more bags and boxes were left beside containers [2]. The containers have sensors, but these only measure what is inside the bin, not what is next to it.

## Who it is for
The municipal team that plans where the waste crews go. Residents report bins with a photo; on a busy day there are too many reports to visit at once, so BinWatch puts them in order. **Not for** enforcement officers who want to give fines, or anyone watching a street or its residents: the model sees rubbish, not who put it there.

## Why SDG 15
When gulls tear bags open, plastic and food waste blows into green areas, where animals eat it or get caught in it, and gulls learn to live off our rubbish. Clearing the worst bins first gives rubbish less time to spread. It also links to SDG 14, because litter in the canals can reach the sea.

## How it works
1. Upload one or more photos, or take one with your phone in the app (Streamlit).
2. Each photo goes to our Roboflow model (RF-DETR), which draws a box around everything it finds and gives it one of the 4 labels. A slider hides boxes the model is unsure about (0.40 by default).
3. The app turns the labels into a priority: **Clear first** (torn bag or loose litter: rubbish is already spreading), **Clear on next round** (closed bags or dumped items), or **Clean** (nothing found).
4. You see each photo with its boxes, counts and priority. Several photos give a **Clear-up order**, worst bin first.

Why not something simpler? The sensors can't see next to the bin, and a fixed route also stops at bins that are already clean.

## Results
300 hand-labelled images from 7 videos we filmed, split 211 train / 60 validation / 29 test. On the test set: **mAP@50 89.6%, precision 88.5%, recall 86.4%.**

| Class | Found | Missed | False alarms |
|---|---|---|---|
| `torn_bag` | 9 of 9 | 0 | 0 |
| `bag` | 12 of 13 | 1 | 1 |
| `dumped_item` | 13 of 15 | 2 | 2 |
| `loose_litter` | 6 of 9 | 3 | 2 |

Hardest class: **loose litter**, because small pieces are easy to miss. On a new photo of scattered litter it ranked the bin *Clear first*, but at 0.40 it found the bigger pieces and missed many small ones. The test images come from the same videos as the training images, so real-world scores will be lower.

## Run it yourself (Windows)
```
pip install -r requirements.txt
copy .streamlit\secrets.toml.example .streamlit\secrets.toml
python -m streamlit run app.py
```
Put your own Roboflow API key in `.streamlit/secrets.toml` first. Never commit that file.

**Sources.** [1] Gemeente Den Haag, *Meeuwenoverlast beperken*, denhaag.nl. [2] *The Hague sees sharp rise in illegal bulky waste*, The Hague Online, 24-04-2026.
