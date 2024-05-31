# Week 1 Practice set

## Text-to-image Progression

**Task**: Generate images from text at different stages of the mode's iteration process at 10, 15, 20, 15, 20 steps.

**Tool used**: [Playground](https://playground.com/)

**Filter**: RealVis XL

**Model**: Stable Diffusion XL

**Prompt Guidance**: 7

**Refinement**: 64

**Seed**: 109099558

**Sampler**: DPM++ 2M Karras

**Prompt**: "King positioned on an iron throne, captured mid-preparation for warfare, armoured, sword grasped, adorned in a black and red robe, crowned, studio lighting enhancing the scene, ultra clear, dramatic lighting."

**Negative Prompt**: "Ugly, deformed, noisy, blurry, distorted, crown, tiara, out of focus, bad anatomy, extra limbs, poorly drawn face, poorly drawn hands, missing fingers, nudity, nude"

### Results

| STEPS | RESULTS                                |
| ----- | -------------------------------------- |
| 10    | <img src="step-10.jpeg"  width="300"/> |
| 15    | <img src="step-15.jpeg"  width="300"/> |
| 20    | <img src="step-20.jpeg"  width="300"/> |
| 25    | <img src="step-25.jpeg"  width="300"/> |
| 30    | <img src="step-30.jpeg"  width="300"/> |

## Image-to-image Variation

**Task**: Modify an existing image at varying strengths (20, 40, 60, 80, 100) to observe the intensity of changes.PGenerate images with specific control over traits (pose, edge, depth), adjusting the influence of each trait.

**Tool used**: [Playground](https://playground.com/)

**Filter**: RealVis XL

**Model**: Stable Diffusion XL

**Prompt Guidance**: 7

**Refinement**: 64

**Seed**: 327138681

**Sampler**: DPM++ 2M Karras

**Prompt**: "A marble sculpture standing in a garden."

**Negative prompt**: "ugly, deformed, noisy, blurry, distorted, out of focus, bad anatomy, extra limbs, poorly drawn face, poorly drawn hands, missing fingers, nudity, nude"

### Results

| STRENGTH | RESULTS                                    |
| -------- | ------------------------------------------ |
| 20       | <img src="strength-20.png"  width="300"/>  |
| 40       | <img src="strength-40.png"  width="300"/>  |
| 60       | <img src="strength-60.png"  width="300"/>  |
| 80       | <img src="strength-80.png"  width="300"/>  |
| 100      | <img src="strength-100.png"  width="300"/> |

## Control Traits in Image Generation

**Task**: Generate images with specific control over traits (pose, edge, depth), adjusting the influence of each trait.

**Tool used**: [Playground](https://playground.com/)

**Filter**: RealVis XL

**Model**: Stable Diffusion XL

**Prompt Guidance**: 7

**Refinement**: 64

**Seed**: 368710

**Sampler**: DPM++ 2M Karras

### Pose

**Reference Image**
<img src="pos-ref.jpeg"  width="300"/>

**Prompt**: "A steampunk sci-fi warrior stands in front of a destroyed city with a post-apocalyptic atmosphere and dramatic lighting."

**Negative prompt**: "ugly, deformed, noisy, blurry, distorted, out of focus, bad anatomy, extra limbs, poorly drawn face, poorly drawn hands, missing fingers, nudity, nude"

### Results

| WEIGHT | RESULTS                                  |
| ------ | ---------------------------------------- |
| 0.2    | <img src="weight-0.2.png"  width="300"/> |
| 0.8    | <img src="weight-0.8.png"  width="300"/> |
| 1.2    | <img src="weight-1.2.png"  width="300"/> |
| 2      | <img src="weight-2.png"  width="300"/>   |

### Edge

**Reference Image**

<img src="edge-ref.jpg"  width="300"/>

**Prompt**: "Portrait of a steampunk sci-fi warrior wearing a gas mask in a destroyed city in the background."

**Negative prompt**: "ugly, deformed, noisy, blurry, distorted, out of focus, bad anatomy, extra limbs, poorly drawn face, poorly drawn hands, missing fingers, nudity, nude"

### Results

| EDGE | THRESHOLD | RESULTS                                    |
| ---- | --------- | ------------------------------------------ |
| 0.2  | 139       | <img src="edge-0.2-139.png"  width="300"/> |
| 0.5  | 200       | <img src="edge-0.5-200.png"  width="300"/> |
| 0.6  | 120       | <img src="edge-0.6-120.png"  width="300"/> |
| 1    | 200       | <img src="edge-1-200.png"  width="300"/>   |
| 1    | 255       | <img src="edge-1-255.png"  width="300"/>   |
| 2    | 255       | <img src="edge-2-255.png"  width="300"/>   |

### DEPTH

**Reference Image**

<img src="pose-ref.jpeg" width="300"/>

**Prompt**: "batman standing in front of the Whitehouse"

**Negative prompt**: "ugly, deformed, noisy, blurry, distorted, out of focus, bad anatomy, extra limbs, poorly drawn face, poorly drawn hands, missing fingers, nudity, nude"

### Results

| DEPTH | RESULTS                                |
| ----- | -------------------------------------- |
| 0.2   | <img src="depth-0.2.png" width="300"/> |
| 0.6   | <img src="depth-0.6.png" width="300"/> |
| 1     | <img src="depth-1.png" width="300"/>   |
| 1.5   | <img src="depth-1.5.png" width="300"/> |
| 2     | <img src="depth-2.png" width="300"/>   |

## Reverse Prompting

**Task**: Create an image from a prompt and then generate a text description that accurately matches the produced image.

### Image 1

**Tool used**: [Playground](https://playground.com/)

**Model**: Playground 2.5

**Reference Image**

<img src="boy-ref.png" width="400"/>

**Reverse Prompt Image**

<img src="boy-reverse.png" width="400"/>

**Prompt**: "Pixar animated soft 3d character, Pixar 3d style, Closeup shot of a sweet cheerful boy with a big smile facing front, visible teeth, wearing a red puffy hoodie jacked charcoal grey undershirt, with a backpack with a black strap, brown messy hair, big brown expressive eyes, black background, intense flames in blurred background, face lit up by fire."

**Negative prompt**: "ugly, deformed, noisy, blurry, distorted, out of focus, bad anatomy, extra limbs, poorly drawn face, poorly drawn hands, missing fingers, nudity, nude"

### Image 2

**Tool used**: [Playground](https://playground.com/)

**Model**: Playground 2.5

**Reference Image**

<img src="noodles-ref.png" width="400"/>

**Reverse Prompt Image**

<img src="noodles-reverse.png" width="400"/>

**Prompt**: "Top view shot, lots of white spaghetti with small green herbs on the spaghetti, served in a two-handled white ceramic bowl, a spoon placed inside the spaghetti, bowl is placed on a marble countertop"

**Negative prompt**: "ugly, deformed, noisy, blurry, distorted, out of focus, bad anatomy, extra limbs, poorly drawn face, poorly drawn hands, missing fingers, nudity, nude"

### Image 3

**Tool used**: [Playground](https://playground.com/)

**Model**: Playground 2.5

**Reference Image**

<img src="painting-ref.jpg" width="400"/>

**Reverse Prompt Image**

<img src="painting-reverse.png" width="400"/>

**Prompt**: "japanese animated long shot of a couple holding hands and walking away from the shot. The boy is wearing a red jacket, the girl is wearing a light blue dress . Two snowclad Mountain peaks in the background, green pasture and flowers on both the sides with cherry blossom trees. Pink flowers on the side closer to the shot."

**Negative prompt**: "ugly, deformed, noisy, blurry, distorted, out of focus, bad anatomy, extra limbs, poorly drawn face, poorly drawn hands, missing fingers, nudity, nude"
