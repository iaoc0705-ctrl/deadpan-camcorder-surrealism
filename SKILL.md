---
name: deadpan-camcorder-surrealism
description: Generate or art-direct original evidence-first surreal stills that look accidentally recorded on late-1990s/early-2000s consumer camcorders. Use for deadpan suburban impossibilities, VHS-C/Hi8/Digital8/MiniDV found-footage imagery, or mundane spaces physically reacting to one absurd event; do not use for generic retro filters, polished cinematic surrealism, or copying source scenes.
---

# Deadpan Camcorder Surrealism

Create a still that feels like accidental evidence of one impossible event. The event may violate one rule, but its contact with the ordinary world must remain physically convincing: weight, displacement, reflections, shadows, wear, obstruction, or human accommodation should show that it is really there.

The image succeeds when the camera seems to have noticed the event late, the environment has already responded to it, and nobody is performing for the image.

## Build the scene

Decide these elements before writing a prompt:

1. **Mundane place:** Choose a recognizable, practically detailed location such as a strip-mall parking lot, laundromat, convenience store, public restroom, loading bay, car interior, small office, or municipal recreation space.
2. **Single rule violation:** Make one everyday object impossibly large, treat an inappropriate activity as routine work, let architecture behave like furniture, or place a machine where it cannot physically belong.
3. **Physical evidence:** Add two or three consequences that follow from the anomaly's size, material, position, or motion. Prefer displaced objects, compressed surfaces, cast shadows, blocked paths, condensation, reflections, cables, stains, footprints, disturbed dust, or plausible wear.
4. **Environmental feedback:** Let the setting and people accommodate the anomaly. A cart route bends around it, a door cannot fully open, a worker has improvised a barrier, or bystanders continue their tasks with mild curiosity.
5. **Accidental camera:** Give the operator a believable reason to be present, then frame as if recording began late: obstructed foreground, clipped subject, uncertain distance, slight tilt, modest zoom, motion softness, or a poor position that a real witness would accept.

One anomaly is stronger than a collection of oddities. Evidence must clarify the event, not introduce new surreal elements.

## Pass the evidence test

Before generation, ask:

- If the anomaly vanished, what traces or displaced objects would remain?
- What nearby surface receives its weight, shadow, reflection, moisture, heat, or motion?
- What has a person, worker, or passerby already done in response?
- Does each consequence obey ordinary physics except for the single rule violation?

If there is no visible answer to at least two of these questions, strengthen the physical evidence before adding camera degradation. Do not use tape noise or captions to disguise weak staging.

## Choose one capture profile

Use one named format as a coherent capture model. Do not blend every defect into a generic “VHS look.”

- **VHS-C:** Softest detail, unstable chroma, visible horizontal noise, occasional head-switching disturbance near the bottom, warm or wandering white balance. Best for early-1990s home-video roughness.
- **Hi8:** Softer analog luma with stronger color than VHS-C, mild chroma crawl, edge smear, and plausible date-era exposure behavior. Best for late-1990s analog consumer footage.
- **Digital8:** Analog-style tape handling with sharper digital edges, interlacing, ringing, and occasional blocky breakup. Best for the 1999-2005 transition period.
- **MiniDV:** Cleaner but still unmistakably consumer video: interlaced motion, clipped highlights, cool/green auto white balance, modest edge enhancement, and restrained DV blocks. Best default for 1999-2006 scenes.

Match damage intensity to the recording situation. A first-generation tape should not look repeatedly duplicated; a paused frame can show interlacing or field artifacts without becoming unreadable.

## Preserve period consistency

Treat the frame as belonging to one plausible year range. Keep vehicles, phones, displays, payment terminals, packaging, clothing, signage, lighting, and camera behavior consistent with it.

- Prefer generic or obscured period cues over prominent brands and readable text.
- Exclude smartphones, LED light strips, modern touchscreens, QR codes, current app interfaces, recent vehicle interiors, and contemporary minimalist retail design unless the user explicitly wants an anachronism.
- Do not add a date stamp or recording overlay by default. If requested, keep it secondary and internally consistent with the selected format and era.
- When the user's concept requires a modern object, preserve the requested object and treat the camcorder look as a deliberate later capture rather than silently forcing a historical setting.

## Keep the world ordinary

- Default to 4:3 landscape unless the user requests another format.
- Use direct on-camera light, flat fluorescent light, overcast daylight, or mixed practical lighting. Allow clipped highlights, low dynamic range, and imperfect auto exposure.
- Specify ordinary materials: scuffed linoleum, cracked asphalt, dented carts, worn upholstery, cheap plastic, stained tile, brushed metal, or faded clothing.
- Keep people occupied with normal tasks. Avoid theatrical fear, spectacle crowds, action poses, knowing comedy, or everyone staring at the anomaly.
- Avoid polished cinematic lighting, shallow depth of field, glossy CGI, cyberpunk color, horror staging, fantasy atmosphere, decorative light leaks, and excessive glitches.

The anomaly must remain legible at thumbnail size. The camera texture should support credibility, not become the subject.

## Handle references as style evidence

When reference frames are supplied, inspect representative frames across the sequence and infer camera behavior, color response, texture, framing, and the relationship between normality and anomaly.

- Treat frames as visual-language references unless the user explicitly requests an edit.
- Prefer 3-5 varied frames over many near-duplicates.
- Create new people, locations, actions, props, and compositions.
- Do not reproduce recognizable identities, branded signs, captions, or a source video's signature scene.
- Do not package third-party reference images into this skill.

## Generate and refine

The user's explicit instructions override these defaults. Honor requested counts, aspect ratios, references, capture formats, time periods, and whether the user wants concepts, prompts, generation, or editing.

When the user asks for an image without specifying a workflow:

1. Draft three short text-only concepts. Vary the location or the physical expression of the rule violation while preserving the user's idea.
2. Rank them by instant readability, physical evidence, environmental feedback, deadpan behavior, accidental-camera credibility, period consistency, originality, and strength as a single still.
3. Select the strongest concept and generate one image.
4. Evaluate it with the evidence test and final checks below.
5. If one localized failure prevents the image from reading, make one targeted edit that changes only that dimension. Otherwise keep the first image.
6. Stop after the first passing image or one targeted edit.

If the user requests concepts only, stop before generation. If the user requests a specific number of images or variants, generate exactly that number, using a separate generation for each distinct concept.

Before generating or correcting an image, read [references/prompt-patterns.md](references/prompt-patterns.md). Use its prompt scaffold, capture profiles, evidence patterns, and targeted corrections. Label supplied images by role and state that they control visual language only.

When the built-in image-generation tool is unavailable, use the configured o10.top fallback. Read [references/o10-api.md](references/o10-api.md), then run `scripts/generate_image.py` with the selected prompt and an explicit output path. This sends the prompt to an external OpenAI-compatible service and may consume account credit. Do not print, copy into prompts, or write the API key to project files. If the fallback is not configured, provide the final prompt instead of inventing credentials.

Use these final checks:

- Could the frame plausibly come from the selected consumer format and period?
- Is the location more ordinary than the anomaly?
- Is there one instantly understandable impossible event?
- Do at least two physical consequences prove the anomaly occupies the space?
- Does the environment respond without becoming a second joke?
- Do people behave as if the situation is routine or only mildly interesting?
- Does the framing feel accidentally captured rather than art-directed?
- Are artifacts plausible, restrained, and profile-specific?
- Is the scene original and free of readable brands, accidental captions, and watermarks?

When further iteration is explicitly requested, preserve the approved concept and change one failing dimension at a time.
