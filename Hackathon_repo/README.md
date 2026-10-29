# Zero Emissions?

**AI for Good — Hackathon 4: Picture the Planet**
Lucas Jansze & Cameron Ruiter

A 27.7-second climate film about the part of an electric car's footprint that the "zero emissions" label hides. Every frame was generated with ComfyUI.

| | |
|---|---|
| Film (MP4) | [`hackathon_4_no_voice_over.mp4`](hackathon_4_no_voice_over.mp4) (1920×1080, 27.7 s) |
| Film (YouTube) | *link will be added here* |
| ComfyUI workflow | [`zero_emissions_workflow.json`](zero_emissions_workflow.json): the exact file that rendered every clip in the film |
| The workflow explained (with screenshots) | [`WORKFLOW.md`](WORKFLOW.md) |
| Storyboard and shot list | [`STORYBOARD.md`](STORYBOARD.md) |
| Ethical reflection | [`ETHICS.md`](ETHICS.md) |
| Individual clips | `shot1_clip_00004_.mp4` … `shot7_clip_00005_.mp4` (1280×736, 24 fps, straight out of the workflow) |
| Keyframes | [`keyframes/`](keyframes): the SDXL keyframe of each shot, taken from the first frame of its clip |
| Frames from the film | [`frames/`](frames): one frame from the middle of each shot |
| Slides | [`Zero_Emissions_Hackathon4_presentation.pptx`](../presentation/Zero_Emissions_Hackathon4_presentation.pptx) |
| SDG | SDG 13 Climate Action, target 13.3 |
| Language | English |

> **The images in this film are AI-generated.** They were made with ComfyUI (SDXL + MiniMax H3). They are not photos or footage of real places, and no frame should be used as evidence of what a real mine, power plant or landfill looks like.

---

## Problem definition

Electric cars are sold as "zero emissions", but that is only true at the tailpipe. Building the battery, mining its materials, making the electricity to charge it and dealing with the battery at the end of its life all cause emissions and harm. Buyers who take the label literally think their choice of EV no longer matters for the climate. So they see no reason to choose a smaller battery, charge on green power or drive less.

This is happening in the Netherlands right now. In 2025, 156,139 new fully electric cars were registered, 40.2% of all new cars (RAI Vereniging & BOVAG, 2026), and every one of them fixes its battery size for the life of the car.

The label being misleading is not only our opinion. In January 2024 the Dutch Advertising Code Committee (Reclame Code Commissie) ruled that an advert claiming "0 g CO2/km" for an electric car was misleading, because the average consumer cannot be expected to know that this number only covers exhaust emissions (Stichting Reclame Code, 2024).

The costs that the label hides are real:

- **The battery.** An electric car's production emissions are about 40% higher than a petrol car's because of the battery, and it takes about 17,000 km of driving to pay this back (ICCT, 2025).
- **Cobalt.** About 76% of the world's cobalt is mined in DR Congo (USGS, 2025), where Amnesty International found children as young as seven working in artisanal cobalt mines (Amnesty International, 2016).
- **Lithium.** In Chile's Atacama desert, lithium mining evaporates on average half a million litres of brine per tonne of lithium carbonate, and groundwater levels have dropped more than 10 metres in 15 years (Mongabay, 2025).
- **The electricity.** In 2025, 48% of Dutch electricity still came from fossil fuels, mostly natural gas (CBS, 2026).
- **End of life.** Landfilling car batteries is banned in the EU (Directive 2006/66/EC, art. 14), so the risk at the end is a battery that is not collected and recycled.

At the same time, an electric car is clearly the better choice. Over its whole life, a medium-size electric car in the EU emits about **63 g CO2-equivalent per km, against 235 g for a petrol car**: 73% less, but not zero (ICCT, 2025). That is the message of our film. Switching is right, but how you switch still matters.

## SDG 13 — Climate Action

The film addresses **SDG 13, target 13.3**: *"Improve education, awareness-raising and human and institutional capacity on climate change mitigation, adaptation, impact reduction and early warning"* (United Nations).

**The specific issue within SDG 13.** Our film is not about "the climate" in general. It is about one awareness gap in climate change mitigation: people who switch to an electric car believe the "zero emissions" label and think their driving no longer has a climate cost. Switching to electric lowers a car's lifetime emissions by about 73% (ICCT, 2025), but the label hides the part of the footprint that the buyer can still influence: the size of the battery, the electricity it is charged with and the number of kilometres driven. Target 13.3 is about exactly this: mitigation only works if people know what actually lowers emissions.

**How the film addresses it.** Every part of the film is linked to that gap:

| What target 13.3 asks for | What the film does |
|---|---|
| **Awareness-raising** | Shots 2 to 6 show the emissions and harm that the label leaves out: the battery's carbon debt, the mining, the fossil electricity and the end of life. |
| **Education on mitigation** | The last line, "Better than petrol. But not zero.", gives the correct picture: an EV emits 73% less over its life (ICCT, 2025), so the switch is right, but the footprint is not gone. |
| **Human capacity to act** | The final shot shows what the viewer can do with that knowledge: a small EV, charged at a house with solar panels, with a cyclist riding past for the trips that need no car at all. |

**Who benefits if it works.** First the buyers themselves: they make a choice that fits what they already want, a car that is really better for the climate, and a smaller EV is usually also cheaper to buy and to charge. Second everyone affected by climate change: a smaller battery means less mining and lower production emissions, and green charging and fewer kilometres lower the emissions of every year the car is on the road. With more than 156,000 new electric cars a year in the Netherlands, small differences per car add up.

**What it does not do.** A 28-second film changes no advertising rule, no battery factory and no electricity mix. It only closes an information gap, which is necessary for a better choice but not enough by itself. And not everything in the film is strictly a climate issue: child labour in cobalt mining and water use in lithium mining belong to SDG 8 (decent work) and SDG 6 (clean water). They are in the film because they are part of the same hidden chain behind the same label, but the climate core of our message is the battery's carbon debt (shot 2) and the fossil electricity (shot 5).
## User group

Our film is made for **Dutch adults aged 25–40 who are about to buy or private-lease their first electric car**, new or second-hand, and who choose electric partly because it feels like the green choice.

This is the next wave of EV buyers:

- In Germany, 29% of 18–29-year-olds expect their next car to be electric, against 9% of people over 50 (ADAC, 2024).
- In the Netherlands, 1 in 5 consumers plans to buy an EV within five years, and 28% see a used EV as affordable (Marktplaats, 2025).
- A quarter of current Dutch EV drivers expect their next EV to be a used one (VER & RVO, 2026).

**Why this group.** They are at the moment where the problem is created: the purchase. Most of them will buy several cars in their life, so the habits they form with their first EV matter most: how big a battery they think they need, how they charge, how much they drive. They buy privately or through private lease with their own money, so unlike many company-lease drivers they choose the model and the battery size themselves.

**What they already believe.** They care about the climate: among Dutch EV drivers, the environment is the second most important reason to drive electric, after driving pleasure (VER & RVO, 2026). But they also believe the adverts: *"An EV has zero emissions, so with this car my driving is climate-neutral."* The Dutch Advertising Code Committee confirmed that the average consumer cannot be expected to know better (Stichting Reclame Code, 2024).

**What we want them to do.** After watching, they should choose a smaller EV with a smaller battery, consider shared or second-hand, charge on green power, and still drive less.

**Placement and conditions of use.** The film is a 28-second pre-roll or sponsored post on YouTube and Instagram, next to EV adverts and car review videos, where this group compares models. Dutch 20–39-year-olds spend about 147 minutes a day on social media (Newcom, 2025). They watch on a phone, in a feed, between other content, so the film has only a few seconds to hold their attention. That is why it opens like the car adverts they already know. The film is in English, so it also reaches the many international residents in the Netherlands.

### Not for

- **People without a car or without plans to buy one.** The film is about a purchase choice they do not make.
- **EV sceptics looking for a reason not to switch.** The film must not become ammunition for "EVs are worse than petrol". That is why the last line of the voiceover is "Better than petrol" and this README gives the ICCT numbers.
- **Company-lease drivers who pick from a fixed list.** They have little say over the model or the battery size, so the main call to action does not fit them.
- **Policy makers and experts.** A 28-second film is too short and too simplified for them; they need the full reports in our sources.

## Solution: how the workflow turns the problem into a film

The workflow in [`zero_emissions_workflow.json`](zero_emissions_workflow.json) is our prototype. It is built on the official ComfyUI MiniMax H3 image-to-video template, extended with a keyframe stage and **one group per shot (seven groups)**. It runs completely inside ComfyUI. For every shot it first generates a still keyframe with SDXL, then animates that keyframe with MiniMax H3 into a short clip with sound. We cut the seven clips together into the film in Clipchamp.

```
shot list ──► keyframe prompt + negative + seed ──► SDXL (KSampler) ──► keyframe PNG
                                                                         │
                                                         Image Scale to video size
                                                                         ▼
              motion prompt + duration + seed ───────► MiniMax H3 (first_frame) ──► clip MP4 with ambient sound
                                                                         │
                                          7 clips, in order, hard cuts ──► Clipchamp + voiceover + music ──► film
```

1. **Input.** For each shot: a keyframe prompt, a negative prompt and a keyframe seed, plus a motion prompt, a duration and a video seed. All of these are in the workflow and listed per shot in [`STORYBOARD.md`](STORYBOARD.md).
2. **Keyframe.** SDXL base 1.0 turns the keyframe prompt into a 1344×768 image (fixed seed, 30 steps, cfg 6.5, `dpmpp_2m` / `karras`). We check this still first: the right car, no faces, no brand badge, the battery in the centre. If it is wrong, we change the prompt or the seed. Only an approved keyframe goes on to the video step.
3. **Fit to video size.** *Image Scale* resizes the keyframe to the video resolution set in the global *Resolution Selector* (0.9 MP → 1280×736).
4. **Clip.** The *Shot to Video (MiniMax H3)* node takes the keyframe as its `first_frame` and animates it according to the motion prompt: the camera move and what moves in the scene. It also generates matching ambient sound (wind, a motor hum, rattling stones). The motion prompt only describes what is already in the keyframe: when a prompt mentioned something that was not there, H3 invented it (a carport in shot 7).
5. **Output.** Per shot, one keyframe (PNG) and one clip with sound (MP4, 1280×736, 24 fps).
6. **Edit.** In Clipchamp we put the seven clips in order at their full generated length, with hard cuts and no effects, and add our own voiceover and royalty-free music. Nothing visual is added outside ComfyUI. The film is exported as MP4 (1920×1080, 27.7 s).

**How this answers the problem.** Every shot shows one cost that the "zero emissions" label leaves out: the battery, cobalt, lithium, the electricity and the end of life. They are shown in places we could never film ourselves. All shots come from one workflow with a shared car description and one look per act, so they read as one film. The same white car that is sold as "zero emissions" in shot 1 is parked in front of a gas power plant in shot 5.

**Why ComfyUI is needed.** Every frame of the film comes out of this workflow; there is no stock footage and no other image generator. Without it there would be no images of the mine, the ponds, the power plant or the landfill. Without the keyframe step we could not control what is in each shot before spending GPU time on the video.

A node-by-node walkthrough of the workflow, with screenshots from ComfyUI and the keyframe → clip result of every shot, is in **[WORKFLOW.md](WORKFLOW.md)**. The full shot list with every prompt, seed, keyframe and frame per shot is in **[STORYBOARD.md](STORYBOARD.md)**.

## Problem–solution fit

The problem is created at one moment, the purchase, and our audience is at that moment now or in the coming years. The belief we want to correct comes from advertising, so we answer in the same format and in the same place. The film opens as a glossy EV advert, exactly what they are used to seeing, and then looks behind it shot by shot, following the battery from the mine to the landfill. It ends on a hopeful, realistic alternative: a small EV at a house with solar panels on its roof, with a cyclist riding past. The viewer leaves with something to do instead of guilt.

Simpler alternatives do not achieve the same result:

- **A fact sheet or article** can be accurate, but our audience does not go looking for it. A pre-roll meets them next to the EV adverts they already watch.
- **A text-only awareness advert** cannot show the chain from mine to landfill in 28 seconds; images can.
- **Filming it ourselves** is impossible. We cannot film a cobalt mine in DR Congo, the Atacama or the inside of a battery, and stock footage is not allowed.

A generated film fits this audience because it speaks the visual language of the adverts they already trust. ComfyUI lets us show every hidden cost while controlling exactly what is shown and what is not (no faces, no brands).

## How to run the workflow

### Requirements

- ComfyUI (recent version with MiniMax H3 support, see [ComfyUI#15224](https://github.com/Comfy-Org/ComfyUI/pull/15224)).
- A GPU that can run MiniMax H3. We used an **RTX 5070 (12 GB)**. The H3 text encoder is a 32B model in NVFP4, a format made for RTX 50-series cards. A 4 GB GTX 1650 could only make keyframes.
- These models, in `ComfyUI/models/…`.

| File | Folder |
|---|---|
| [`sd_xl_base_1.0.safetensors`](https://huggingface.co/stabilityai/stable-diffusion-xl-base-1.0) | `checkpoints` |
| [`minimax_h3_fl2va_pruned_int8_convrot.safetensors`](https://huggingface.co/Comfy-Org/MiniMax-H3/resolve/main/diffusion_models/minimax_h3_fl2va_pruned_int8_convrot.safetensors) | `diffusion_models` |
| [`qwen3vl_32b_minimax_h3_nvfp4_awq.safetensors`](https://huggingface.co/Comfy-Org/MiniMax-H3/resolve/main/text_encoders/qwen3vl_32b_minimax_h3_nvfp4_awq.safetensors) | `text_encoders` |
| [`minimax_h3_video_vae_int8_convrot.safetensors`](https://huggingface.co/Comfy-Org/MiniMax-H3/resolve/main/vae/minimax_h3_video_vae_int8_convrot.safetensors) | `vae` |
| [`minimax_h3_audio_vae_fp32.safetensors`](https://huggingface.co/Comfy-Org/MiniMax-H3/resolve/main/vae/minimax_h3_audio_vae_fp32.safetensors) | `vae` |
| [`minimax_h3_fl2v_turbo_8step_v1.0_comfyui_bf16.safetensors`](https://huggingface.co/lightx2v/Minimax-h3-Turbo/resolve/main/minimax_h3_fl2v_turbo_8step_v1.0_comfyui_bf16.safetensors) | `loras` |

### Steps

1. Open ComfyUI and drag `zero_emissions_workflow.json` onto the canvas.
2. Leave the **Global settings** group as it is. These are the settings that rendered the film:

   | Setting | Value used for the film |
   |---|---|
   | Keyframe model | `sd_xl_base_1.0.safetensors` |
   | Resolution Selector | 16:9, **0.9 MP → 1280×736** |
   | FPS | **24** |
   | `turbo_mode` on each H3 node | **true** (8 steps with the turbo LoRA) |
   | Keyframe size (Empty Latent Image) | 1344×768 |

3. Generate:
   - **One keyframe only:** right-click that shot's *Save Image* node → *Queue Selected Output Nodes*.
   - **One full shot:** right-click that shot's *Save Video* node → *Queue Selected Output Nodes*.
   - **The whole film:** *Run* (all seven shots in a row; takes a while).
4. Outputs appear in `ComfyUI/output/zero_emissions/` as `shotN_keyframe_*.png` and `shotN_clip_*.mp4`.
5. Put the seven clips in order (1 → 7) at full length with hard cuts in any video editor, then add the voiceover from [STORYBOARD.md](STORYBOARD.md) and the music below.

All seeds are fixed (`control_after_generate: fixed`), so the same prompt, seed and settings give the same keyframe on the same setup. To test on a weaker GPU, set the Resolution Selector to 0.2 MP and FPS to 12. That is only for testing: the result does not match the film.

## Sound

- **Ambient sound:** generated by MiniMax H3 together with each clip, inside ComfyUI.
- **Voiceover:** our own English voiceover, recorded on a phone. Script in [STORYBOARD.md](STORYBOARD.md).
- **Music:** royalty-free.
- No third-party AI voice tools were used.

## Ethical reflection

**The biggest risk is misleading the other way.** Our film criticises a misleading green label, so it could be read as "electric cars are worse than petrol cars". A viewer who believes that may put off switching or buy a petrol car, which means more emissions: the opposite of our goal. That is why the last line of the voiceover is "Better than petrol. But not zero.", the final shot shows a small EV at a house with solar panels as the good choice, and this README gives the ICCT numbers (63 against 235 g CO2-eq/km).

The full reflection, with five further risks specific to this film (the landfill shot, invented images of real places, a fake advert that looks real, viewers not seeing that the images are AI-generated, and the energy cost of our 37 clip renders and 66 keyframes), and the generation log per shot, is in **[ETHICS.md](ETHICS.md)**.

## What we learned

### Lucas Jansze

I learned that with AI video the work is in the still image, not in the video. A clip can only be as good as its first frame, so I built the workflow in two stages: SDXL makes a keyframe that I can check in a few seconds, and only an approved keyframe goes on to MiniMax H3, which takes minutes. Our first keyframes with SD 1.5 ignored complex prompts (shot 2 became an orange car in a showroom instead of an x-ray), and switching to SDXL with the main subject at the start of a short prompt fixed that. I also learned that a motion prompt may only describe what is already in the keyframe: when the shot 7 motion prompt mentioned a carport that was not in the image, H3 invented one halfway through the clip.

### Cameron Ruiter

## Sources

All figures were checked on 29 September 2026.

- ADAC & Bilendi. (2024, August). *Survey on electric car interest by age group (Germany).* Reported by EV Update: https://www.evupdate.nl/explainers/artikel/onderzoek-adac-evs-vooral-in-trek-onder-jongeren
- Amnesty International. (2016). *"This is what we die for": Human rights abuses in the Democratic Republic of the Congo power the global trade in cobalt.* https://www.amnesty.org/en/documents/afr62/3183/2016/en/
- CBS. (2026, 9 March). *Elektriciteitsproductie en -uitvoer op recordniveau.* https://www.cbs.nl/nl-nl/nieuws/2026/11/elektriciteitsproductie-en-uitvoer-op-recordniveau
- European Union. (2006). *Directive 2006/66/EC on batteries and accumulators*, article 14. https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=celex%3A32006L0066
- ICCT. (2025). *Life-cycle greenhouse gas emissions from passenger cars in the European Union: A 2025 update and key factors to consider.* https://theicct.org/publication/electric-cars-life-cycle-analysis-emissions-europe-jul25/
- Marktplaats. (2025, 23 September). *EV survey.* Reported by Nederland Elektrisch: https://nederlandelektrisch.nl/actueel/nieuwsoverzicht/i3120/1-op-5-nederlandse-consumenten-wil-binnen-5-jaar-elektrische-auto-kopen
- Mongabay. (2025, 10 September). *Lithium mining leaves severe impacts in Chile, but new methods exist: Report.* https://news.mongabay.com/2025/09/lithium-mining-leaves-severe-impacts-in-chile-but-new-methods-exist-report/
- Newcom. (2025). *Nationale Social Media Onderzoek 2025.* Reported by Frankwatching: https://www.frankwatching.com/archive/2025/01/25/social-media-onderzoek-2025/
- RAI Vereniging & BOVAG. (2026, January). *Autoverkoop stabiel in 2025.* https://www.raivereniging.nl/actueel/nieuws/autoverkoop-stabiel-in-2025/
- Stichting Reclame Code. (2024, 31 January). *Ruling 2023/00576, Lucid ("0 g CO2/km").* https://www.reclamecode.nl/uitspraak/?uitspraakId=469679
- United Nations. *Goal 13: Take urgent action to combat climate change and its impacts.* https://sdgs.un.org/goals/goal13
- U.S. Geological Survey. (2025). *Mineral Commodity Summaries 2025: Cobalt.* https://pubs.usgs.gov/periodicals/mcs2025/mcs2025-cobalt.pdf
- VER & RVO. (2026, 31 March). *EV- en Berijdersonderzoek 2025.* Reported by Nederland Elektrisch: https://nederlandelektrisch.nl/actueel/nieuwsoverzicht/i3258/ev-en-berijdersonderzoek-2025-elektrisch-rijden-stevig-verankerd-maar-kritiek-op-overheidsbeleid
