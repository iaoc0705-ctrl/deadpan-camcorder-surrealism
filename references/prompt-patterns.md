# Evidence-First Prompt Patterns

Read this reference when generating an image, selecting a capture profile, or diagnosing why a result misses the style.

## Concept engine

Combine a mundane location, one rule violation, and a chain of ordinary consequences. The location establishes normality, the anomaly supplies the impossibility, and the evidence makes it believable.

| Location | Rule violation | Physical evidence | Environmental feedback | Camera excuse |
|---|---|---|---|---|
| Laundromat | A familiar object receives the wrong kind of maintenance | Wet floor, compressed cart wheel, dragged hose | A worker has placed one caution cone | Filmed late from the doorway |
| Strip-mall lot | An indoor machine is embedded in asphalt | Cracked sealant, pooled rain, cast shadow | Cart traffic curves around it | Shot past a parked car |
| Convenience store | The checkout processes something that cannot fit | Bent display rack, blocked aisle, reflected mass | The queue shifts without complaint | Friend filming from aisle end |
| Public restroom | A fixture doubles as recreation equipment | Damp footprints, strained bracket, scuffed tile | Users follow an improvised route | Nervous handheld wide shot |
| Car interior | A control becomes an implausible household object | Indented upholstery, wiring, hand contact | Driver tests it seriously | Passenger-seat camcorder |
| Small office | Architecture behaves like furniture | Carpet compression, clipped ceiling tile, dust | Staff move chairs around it | Late zoom from the hall |

Do not select evidence that creates a second impossible event. Use two or three consequences with different roles: one contact cue, one optical cue, and optionally one human response.

## Evidence patterns

Use only consequences that logically follow from the chosen anomaly.

- **Weight/contact:** compressed carpet, bowed shelf, cracked asphalt, displaced gravel, strained fastener.
- **Occlusion/scale:** blocked doorway, clipped ceiling tile, hidden floor line, foreground object partly covering the anomaly.
- **Light/optics:** cast shadow, dull reflection, colored spill, condensation, exposure shift near a bright surface.
- **Motion/history:** drag marks, disturbed dust, wet trail, swaying cable, recently moved chair.
- **Human accommodation:** taped boundary, improvised sign with unreadable text, rerouted queue, worker continuing around the obstruction.

Evidence should be visible rather than merely asserted. “Heavy” is weaker than “two caster wheels sink into damp asphalt.”

## Accidental-camera logic

Give the frame a witness, position, and timing mistake:

1. **Witness:** customer, passenger, employee, neighbor, or passerby.
2. **Position:** doorway, aisle end, car seat, hallway, curb, or behind another person.
3. **Late discovery:** the event is partly clipped, initially obstructed, already underway, or caught during a small corrective zoom.
4. **Imperfection:** one or two of slight tilt, loose crop, mild motion smear, autofocus uncertainty, or consumer zoom softness.

Avoid piling on arbitrary mistakes. A plausible bad view is more convincing than aggressively chaotic framing.

## Capture profiles

Choose one profile and use its traits consistently.

### VHS-C

```text
Early-1990s VHS-C home-video frame; very soft horizontal detail; unstable analog chroma; slight color bleed and head-switching noise near the lower edge; wandering warm auto white balance; low-light gain noise; first-generation tape, still readable.
```

### Hi8

```text
Late-1990s Hi8 consumer-camcorder frame; soft analog luminance with comparatively stronger color; mild chroma crawl and edge smear; clipped practical highlights; gentle tape noise; handheld exposure breathing; no modern film emulation.
```

### Digital8

```text
Early-2000s Digital8 frame; interlaced consumer video with sharpened edges and mild ringing; analog-tape handling feel with occasional restrained blocky breakup; imperfect auto white balance; modest zoom softness.
```

### MiniDV

```text
1999-2006 MiniDV consumer-camcorder frame; 4:3 interlaced video; cool-green auto white balance; clipped highlights; consumer edge enhancement; mild DV mosquito noise and block breakup only in motion; clean enough to read as a first-generation recording.
```

## Generation scaffold

```text
Use case: stylized-concept
Asset type: <preview, storyboard still, editorial image, or requested use>
Primary request: Create a completely original still. In <mundane location>, <one clear impossible event>. <People continue an ordinary task and react minimally>.
Physical evidence: <two or three visible, logically caused consequences: contact/weight, light/reflection, motion/history>.
Environmental feedback: <one practical way the place or people have accommodated the event>.
Input images: <Image 1...N are visual-language references only; do not reproduce their people, props, locations, text, or composition.>
Capture profile and period: <one of VHS-C, Hi8, Digital8, or MiniDV>; <plausible year range>; period-consistent vehicles, clothing, displays, packaging, and interiors.
Composition/framing: 4:3 landscape; recorded by <witness> from <position>; the camera notices late; <one or two plausible framing imperfections>.
Lighting/mood: <direct on-camera light, flat fluorescent light, overcast daylight, or mixed practical light>; low dynamic range; imperfect auto exposure; emotionally flat.
Materials/textures: <specific ordinary surfaces and wear>.
Constraints: One rule violation only; ordinary physics everywhere else; evidence must be visible; new people, location, action, and composition; no readable brands, logos, captions, dates, interface overlays, or watermark.
Avoid: Polished cinematic lighting, shallow depth of field, glossy CGI, cyberpunk color, horror staging, fantasy atmosphere, theatrical reactions, staged comedy, decorative light leaks, excessive glitches, mixed tape-format clichés, and modern objects inconsistent with the chosen period.
```

## Evidence test

Check the result in this order:

1. **Contact:** Does the anomaly touch, press, block, reflect in, or cast light/shadow onto the scene?
2. **Consequence:** Is at least one nearby object or surface changed by that contact?
3. **Accommodation:** Has a person or the environment responded in a small practical way?
4. **Single exception:** Are all consequences ordinary physics rather than additional magic?
5. **Camera causality:** Does the crop and viewpoint follow from a plausible witness position?

If contact or consequence fails, fix staging before changing texture. If only the recording feel fails, preserve scene geometry and correct the capture profile.

## Targeted correction patterns

Apply one correction per edit and preserve everything that already works.

- **Anomaly looks pasted in:** Keep its design, scale, and position. Add a contact shadow, local occlusion, one material reflection, and surface compression or displacement exactly where it meets the environment.
- **No environmental response:** Keep the anomaly unchanged. Add one practical accommodation such as a shifted queue, moved chair, bent route, improvised barrier, or partially blocked door.
- **Evidence becomes a second joke:** Remove unrelated reactions and impossible debris. Retain only consequences directly caused by the anomaly's weight, size, material, heat, moisture, or motion.
- **Camera feels art-directed:** Preserve the scene. Move the viewpoint to a plausible witness position, let a foreground object partly obstruct the frame, clip a nonessential edge, and soften only the active motion.
- **Too polished:** Preserve the staging. Replace cinematic light with flat practical light, lower dynamic range, and apply only the defects belonging to the selected capture profile.
- **Generic VHS filter:** Choose one capture profile. Remove decorative grain, light leaks, and stacked glitches; restore profile-specific resolution, color behavior, interlacing, and tape or codec artifacts.
- **Wrong period:** Preserve the anomaly and composition. Replace only anachronistic phones, displays, vehicles, fixtures, clothing, packaging, or lighting with plausible equivalents from the chosen year range.
- **Too dreamlike:** Keep the central anomaly. Restore ordinary materials, architecture, practical lighting, visible contact, and routine behavior everywhere else.
- **Too comedic or staged:** Remove exaggerated expressions and poses. Give each person a normal task and mild or absent reaction; retain one practical accommodation.
- **Anomaly unclear:** Simplify its silhouette, remove competing oddities, and frame it against an ordinary surface at readable scale without making the camera composition perfect.
- **Too similar to a reference:** Change the location category, human activity, anomaly mechanism, viewpoint, evidence chain, and foreground; preserve only camera texture and tonal restraint.
- **Artifacts overpower the image:** Reduce degradation to first-generation recording levels; preserve subject legibility and keep only profile-specific defects.

## Original concept seeds

Use these as structural examples only; invent new specifics for the user's request.

- A service counter handles an object that cannot fit through the building; the counter edge bows, a floor mat bunches beneath it, and the queue has shifted to one side.
- A maintenance worker repairs the wrong category of object; the tool leaves plausible marks and a small barrier redirects foot traffic.
- A large office appliance is integrated into outdoor infrastructure; rain pools along its base and pedestrians follow an established path around it.
- A vehicle control is replaced with a domestic object; mounting hardware and compressed upholstery sell the weight while the driver performs a serious functional test.
