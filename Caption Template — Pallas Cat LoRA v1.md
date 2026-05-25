# Caption Template — Pallas Cat LoRA v1

## Principle

Don't describe permanent species features. Captions should 
describe what *varies* across images: pose, background, lighting, 
framing. Permanent features (anatomy, fur, ear shape, eye 
geometry) are absorbed by the trigger word.

## Template

pallas cat, Otocolobus manul, [pose], [background], [lighting],
wildlife photography, photorealistic

## Example captions

| Image                 | Caption                                                      |
| --------------------- | ------------------------------------------------------------ |
| Front sitting on rock | `pallas cat, Otocolobus manul, sitting front view on rock, looking at camera, soft natural daylight, wildlife photography, photorealistic` |
| Side walking in snow  | `pallas cat, Otocolobus manul, walking side profile on snow, full body, overcast lighting, wildlife photography, photorealistic` |
| Head close-up         | `pallas cat, Otocolobus manul, head portrait close up, blurred green grass background, golden hour, wildlife photography, photorealistic` |

## Workflow used

1. BLIP auto-caption (first pass)
2. Manual audit of every line — BLIP often calls Pallas cats 
   "domestic cat" or "tabby"; correct each
3. Standardize order: trigger → species tag → pose → background 
   → lighting → wildlife photography → photorealistic
4. Remove any permanent-feature descriptions BLIP added