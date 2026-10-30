# Prompt engineering for image generation

[Back to README](../README.md)

## 1. Define the job

Write the actual use case: ecommerce listing, product launch, editorial illustration, instructional graphic, social ad, character sheet or packaging mockup. Different jobs require different composition and accuracy rules.

## 2. Specify the subject

Describe the object or person, its position, relevant visible features and any approved reference image. Avoid vague phrases like 'make it beautiful'.

## 3. Specify art direction

Use a small number of compatible directions: documentary photography, editorial studio, architectural CGI, paper collage or watercolor. Combining too many competing styles can weaken consistency.

## 4. Control the scene

Define location, surfaces, background objects, material properties, weather, time of day and how the subject interacts with its environment.

## 5. Control composition

Specify viewpoint, focal length as a photographic cue, subject placement, negative space, crop and intended aspect ratio. A camera cue is a visual instruction, not a guarantee of physical camera simulation.

## 6. Control lighting

Describe light direction, size, softness, temperature and shadow behavior. Check that shadows and reflections agree.

## 7. Lock what must not change

For edits, state exactly which elements to preserve: product label, colors, packaging, proportions, identity, background or framing. Attach the original image.

## 8. Specify final delivery

State target channel, aspect ratio, whether text will be overlaid later, and required safe zones. A requested pixel size may not be supported by every generator.

## 9. Iterate one variable at a time

If the first result is wrong, change a specific instruction rather than rewriting everything. For controlled creative comparisons, keep all other factors fixed.

## 10. Review before publishing

Check brand and product accuracy, text spelling, anatomy, hands, perspective, lighting, misleading claims, rights and platform specifications.

## Master prompt template

```text
Create a [OUTPUT TYPE] featuring [SUBJECT] for [AUDIENCE AND PURPOSE].
Art direction: [STYLE].
Environment: [SETTING AND SURFACES].
Composition: [VIEWPOINT, FRAMING AND SUBJECT PLACEMENT].
Lighting: [DIRECTION, SOFTNESS AND COLOR].
Materials: [VERIFIED MATERIALS AND DETAILS].
Palette: [COLORS].
Output: [ASPECT RATIO AND CHANNEL].
Preserve: [REFERENCE-BASED ELEMENTS THAT MUST NOT CHANGE].
Avoid: [SPECIFIC UNWANTED ELEMENTS].
Do not invent text, logos, product features or factual claims.
```

## Example: luxury watch

Create a premium product hero photograph of [WATCH] for a website landing page. Place it on dark slate with soft side lighting and controlled metal reflections. Use a three-quarter angle and leave negative space on the left. Preserve the supplied dial, markings, case shape and strap. Output 16:9. No extra text or invented branding.

## Example: authentic local business

Create an editorial photograph of [BUSINESS TYPE] in [CITY] showing a genuine working moment. Use accurate local environmental details, natural window lighting and unstaged expressions. Avoid generic corporate poses and fictional claims about the business.
