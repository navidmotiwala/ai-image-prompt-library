# Complete AI image production workflow

[Back to README](../README.md)

Updated: 30 October 2026

This is a practical end-to-end workflow for product photography, social ads, ecommerce, branding, editorial visuals, education and client delivery. Custom slash labels are organizational shorthand, not native commands in image generators.

## Workflow overview

```text
Brief -> References -> Concepts -> Master prompt -> Generate -> Select -> Edit -> QC -> Export -> Measure
                      ^                                      |
                      |____________ revise if needed _______|
```

## Stage 1: Brief and acceptance criteria

Record the business objective, intended viewer, subject, single main message, distribution channel, exact copy, deliverable count, aspect ratios, deadline, approval owner and any restrictions.

**Input:** A product, idea or campaign request.

**Actions:**
1. State the one thing viewers should notice.
2. Define the target audience and placement.
3. Identify approved claims, brand assets and mandatory content.
4. Decide whether this is a new image, an edit, a composite or a coordinated series.
5. Define acceptance criteria before generation.

**Output:** Approved brief.

**Example:**

| Field | Value |
| --- | --- |
| Product | Wireless headphones |
| Goal | Product launch |
| Audience | Young professionals |
| Style | Premium, modern, realistic |
| Channels | Website hero and social feed |
| Outputs | 16:9 and 4:5 |
| Preserve | Actual product shape and logo |
| Avoid | Invented controls, misleading specifications |

**Gate:** Do not start production if exact product identity or mandatory factual copy is missing.

## Stage 2: Reference collection and rights

Gather approved product photographs, packaging, logo files, brand guidelines, color values, approved copy, moodboards and platform specifications.

Classify every reference as:
- Identity reference: what must stay exact.
- Composition reference: camera framing and spatial layout.
- Style reference: color, lighting and texture.
- Factual reference: claims, labels, dimensions and data.

Check rights and permissions. Do not assume a publicly accessible image can be reused commercially.

**Output:** Reference folder with a preservation checklist.

## Stage 3: Concept exploration

Develop at least three meaningfully different visual concepts before generating final assets. Compare visual idea, audience fit, production complexity, brand fit and risk of model errors.

```text
/creative-director /concept-matrix /distinct

Create four different advertising image concepts for [PRODUCT].
Audience: [AUDIENCE].
Goal: [GOAL].
Brand guidelines: [GUIDELINES].

For each concept, provide:
- Name and creative rationale
- Subject placement and environment
- Camera and lighting
- Palette and material direction
- Negative space for copy
- Full image prompt
- Accuracy risks and mitigation

Avoid near-duplicate concepts.
Do not invent product features.
```

**Output:** Selected visual direction and two alternatives.

## Stage 4: Master prompt specification

Use this reusable structure:

```text
/image /[category] /[style] /[composition]

Create a [OUTPUT TYPE] featuring [SUBJECT].
Purpose: [CHANNEL AND GOAL].
Audience: [AUDIENCE].
Concept: [VISUAL IDEA].
Setting: [ENVIRONMENT AND PROPS].
Composition: [ANGLE, CROP, PLACEMENT, NEGATIVE SPACE].
Lighting: [DIRECTION, SOFTNESS, COLOR].
Materials: [VERIFIED MATERIAL DETAILS].
Palette: [BRAND AND SUPPORTING COLORS].
Reference: [APPROVED SOURCE IMAGES].
Preserve exactly: [PRODUCT FEATURES, LABELS, IDENTITY].
Output: [ASPECT RATIO].
Avoid: [UNWANTED ELEMENTS].
Quality: consistent perspective, contact shadows,
realistic materials, accurate subject, no fabricated claims.
```

Avoid incompatible instructions such as simultaneously requesting an overhead and eye-level camera for the same shot.

**Output:** Reproducible master prompt.

## Stage 5: Controlled generation

1. Generate a small batch of candidate images.
2. Record model, version if available, date, prompt, references and settings.
3. Compare the candidates at the same crop and display size.
4. Change one main variable at a time, such as background, lighting or camera angle.
5. Select a winner against the original brief rather than personal preference alone.

**Output:** Selected candidate and version log.

## Stage 6: Refinement and editing

Use targeted edits rather than replacing the entire prompt.

```text
/edit /preserve /change-one-variable

Use the attached selected image.
Change only [EXACT ELEMENT] to [DESIRED RESULT].
Preserve [LIST OF UNCHANGED ELEMENTS].
Match existing perspective, lighting and materials.
Do not add new logos, text, objects or claims.
```

If a reference-locked edit fails repeatedly, use manual compositing or a design editor rather than assuming another generation will be exact.

**Output:** Approved visual master.

## Stage 7: Quality assurance

Inspect at full resolution and at the final display size.

### Identity
- Product geometry and proportions match references.
- Branding, colors, packaging and labels are correct.
- Characters remain consistent across a series.

### Visual quality
- Shadows and reflections have coherent directions.
- Materials and perspective are plausible.
- Hands, faces, objects and fine details are not distorted.
- Focal point and visual hierarchy are clear.

### Accuracy and compliance
- No invented scientific, medical or product claims.
- Comparisons and testimonials are genuine and approved.
- No fabricated interface data or false product specifications.
- Source rights, privacy and advertising rules are considered.

### Delivery
- Safe zones and aspect ratios are correct.
- Text remains readable on mobile.
- No accidental cropping of critical content.
- Files open correctly and are named consistently.

**Gate:** Reject any candidate with a material factual or brand error even if visually attractive.

## Stage 8: Post-production

Add exact typography and verified logos in a design editor. Perform restrained retouching, alignment, color correction and platform-specific reframing. Keep the untouched source and edited master.

**Output:** Final production master.

## Stage 9: Export and delivery

| Use | Common ratio | Notes |
| --- | --- | --- |
| Square feed creative | 1:1 | Check platform placement rules |
| Portrait feed | 4:5 | Preserve subject and headline space |
| Stories or vertical cover | 9:16 | Allow for UI overlays |
| Website hero | 16:9 | Check responsive crops |
| Product listing | Platform-specific | Follow marketplace image requirements |

Choose PNG for assets needing lossless quality or transparency, and JPEG or WebP when supported and suitable. Verify output dimensions, compression, color profile, file size and transparency.

Suggested filename: `brand_campaign_concept_ratio_v03.png`.

Suggested folder structure:

```text
campaign-name/
  01-brief/
  02-references/
  03-concepts/
  04-prompts/
  05-generations/
  06-edits/
  07-qc/
  08-approved/
  09-exports/
  10-performance/
```

## Stage 10: Measurement and learning

For marketing assets, log platform, audience, objective, creative version, dates, impressions, clicks, conversions and spend when available. Compare like-for-like placements and audiences. A visual impression is not evidence of conversion impact.

Maintain a prompt register:

| Field | Example |
| --- | --- |
| Prompt ID | IMG-001 |
| Campaign | Headphone launch |
| Concept | Premium studio |
| Generator | Model name and version |
| References | Approved product photos |
| Main variable | Lighting direction |
| Status | Approved |
| Result | Actual campaign metric when measured |

## Branch workflows

### A. Product advertising
Brief -> Verified product reference -> Concept -> Product-locked generation -> Packaging QC -> Layout and copy -> Export -> Campaign test.

### B. Ecommerce catalog
SKU list -> Reference photography -> Standard camera and lighting -> Batch generation -> Per-SKU accuracy review -> Marketplace compliance -> Export.

### C. Social media campaign
Message -> Audience and placement -> Three concepts -> 4:5 and 9:16 compositions -> Copy and brand review -> Publish -> Measure.

### D. Existing-image editing
Original image -> Define exactly what changes -> Preserve everything else -> Targeted edit -> Pixel-level inspection -> Export.

### E. Character consistency
Character bible -> Turnaround sheet -> Approved master reference -> Scene prompts -> Face, outfit and proportion QC -> Series delivery.

### F. Educational and technical
Verified source material -> Simplified visual structure -> Generation -> Expert validation -> Accurate labels in editor -> Final review.

### G. Website and SaaS visuals
Page objective -> Layout wireframe -> Illustration or product visual -> Responsive safe zones -> Verified interface overlay -> Accessibility review -> Web export.

### H. Localized campaigns
Approved master -> Market-specific research -> Culturally accurate adaptation -> Local copy and legal review -> Format exports -> Regional test.

## Troubleshooting decision tree

```text
Is the product or factual content wrong?
  Yes -> Return to approved references and regenerate or composite.
  No  -> Is the composition wrong?
           Yes -> Change framing and subject placement only.
           No  -> Is the lighting or material wrong?
                    Yes -> Targeted relighting or material edit.
                    No  -> Is text wrong?
                             Yes -> Replace with verified typesetting.
                             No  -> Run final QC and export.
```

## Automation opportunities

Automate file naming, prompt logging, metadata capture, image dimensions checks, duplicate detection, export resizing and approval tracking. Keep human review for factual claims, brand identity, ethics, rights and high-stakes visual content.

Automation tools may include Python, n8n, GitHub Actions and local design scripts, depending on available model APIs and usage rights. Image generation itself may require access to a compatible model or local model runtime.

## Further reading

- [Prompt engineering](prompt-engineering.md)
- [Quality control](quality-control.md)
- [Creative trends](creative-trends-2026.md)
- [Prompt categories](../README.md)
- [Tools and learning resources](../RESOURCES.md)
