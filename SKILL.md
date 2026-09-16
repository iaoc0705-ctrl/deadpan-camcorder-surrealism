---
name: deadpan-camcorder-surrealism
description: Generate or art-direct original still images that combine mundane late-1990s/early-2000s consumer-camcorder realism with one calmly observed impossible event. Use for deadpan suburban surrealism, degraded MiniDV/VHS found-footage imagery, or ordinary public spaces made subtly absurd; do not use for a generic retro filter, polished cinematic surrealism, or copying a source video's people and scenes.
---

# Deadpan Camcorder Surrealism

Create images that feel like accidental evidence of an impossible event, recorded by an ordinary person on a cheap consumer camera. The image succeeds when the event is strange but the world around it remains boring, plausible, and emotionally flat.

## Build the image around four decisions

1. Choose a mundane location with recognizable practical detail: a strip-mall parking lot, laundromat, convenience store, ATM vestibule, public restroom, loading bay, car interior, small office, or municipal recreation space.
2. Introduce one clear rule violation: an everyday object is impossibly large, an inappropriate activity is performed as routine work, architecture behaves like furniture, or a machine appears where it physically should not be.
3. Keep human behavior deadpan. People continue shopping, waiting, working, or watching with mild curiosity. Avoid theatrical fear, spectacle crowds, action poses, or exaggerated comedy.
4. Place a believable amateur camera. Prefer an awkward eye-level angle, slight tilt, imperfect crop, casual foreground obstruction, late reaction, or modest digital zoom.

One anomaly is usually stronger than a scene full of random oddities. The impossible element must be legible in a thumbnail without turning the entire world into fantasy.

## Preserve the visual grammar

- Default to 4:3 landscape unless the user requests another format.
- Describe an authentic late-1990s or early-2000s consumer MiniDV/VHS frame, not a modern photograph with a vintage preset.
- Use direct on-camera flash, flat fluorescent light, overcast daylight, or mixed practical lighting. Allow clipped highlights, cool or green-gray shadows, low dynamic range, and imperfect white balance.
- Ask for restrained analog/digital defects: chroma bleed, red/cyan edge fringing, interlacing, edge ringing, tape noise, scanline shimmer, low-bitrate blocks, and slight motion softness.
- Keep materials ordinary and specific: scuffed linoleum, cracked asphalt, dented carts, worn upholstery, cheap plastic, stained tile, brushed metal, faded clothing.
- Favor faded beige, concrete gray, dirty white, washed blue, weak green, and occasional practical orange-red light.

Do not stack every degradation effect at maximum intensity. The scene must remain readable and photographic.

## Handle references as style evidence

When reference frames are supplied, inspect representative frames across the sequence. Use them to infer camera behavior, color response, texture, framing, and the relationship between normality and anomaly.

- Treat frames as style references unless the user explicitly asks to edit one.
- Prefer 3-5 varied reference frames over many near-duplicates.
- Create new people, locations, actions, props, and compositions.
- Do not reproduce recognizable identities, branded signs, captions, or a source video's signature scene.
- Do not package third-party reference images into this skill. The instructions must work without them.

## Generate and refine

The user's explicit instructions take precedence over this skill's defaults. Honor requested image counts, aspect ratios, reference usage, and whether the user wants concepts, prompts, generation, or editing.

When the user asks for an image but does not specify a count or workflow, use this default selection flow:

1. Draft three short text-only concepts without calling an image-generation tool. Vary the mundane location or the physical expression of the rule violation while preserving the user's core idea.
2. Rank the concepts by instant readability, strength of the normal-versus-impossible contrast, deadpan behavior, camera credibility, originality, and suitability for a single still. Select the strongest concept autonomously.
3. Generate only one image for the selected concept. Do not generate the two runners-up.
4. Evaluate the result using the checks below.
5. If one clear, localized failure prevents the concept from reading, make one targeted edit that changes only that dimension. Otherwise keep the first image.
6. Stop after the first passing image or one targeted edit. Do not automatically generate more alternatives or continue iterating.

If the user requests text concepts only, stop before image generation. If the user requests a specific number of images or variants, generate exactly that number and use a separate generation for each distinct concept.

Before generation, read [references/prompt-patterns.md](references/prompt-patterns.md) for the prompt scaffold and correction patterns. Label reference images by role and state that they control visual language only.

Evaluate each result on these questions:

- Could this pass as a paused frame from a cheap consumer camcorder?
- Is the location more ordinary than the anomaly?
- Is there one instantly understandable impossible event?
- Do people behave as if it is routine or only mildly interesting?
- Are degradation artifacts plausible rather than decorative?
- Is the scene original and free of readable brands, accidental captions, and watermarks?

When an explicit user request calls for further iteration, change one failing dimension at a time and preserve the approved concept.
