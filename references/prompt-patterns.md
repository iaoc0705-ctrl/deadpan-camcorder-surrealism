# Prompt Patterns

Read this reference when generating images or diagnosing why a result misses the style.

## Concept engine

Combine one item from each column. Prefer a relationship that reads instantly rather than a random pairing.

| Location | Rule violation | Deadpan behavior | Camera excuse |
|---|---|---|---|
| Laundromat | A familiar object is used for the wrong form of maintenance | A worker continues methodically | Filmed from the doorway |
| Strip-mall parking lot | An indoor machine is embedded in the asphalt | Shoppers route carts around it | Shot past a parked car |
| Convenience store | The checkout processes something physically impossible | The queue waits without complaint | Friend filming from an aisle |
| Public restroom | Utility fixtures double as recreation equipment | Users follow an improvised routine | Nervous handheld wide shot |
| Car interior | One control is replaced by an implausible household object | The driver tests it seriously | Passenger-seat camcorder |
| Small office | The building's architecture behaves like office furniture | Staff finish paperwork nearby | Late digital zoom from the hall |

Avoid selecting a location, anomaly, and reaction that all compete for attention. The location establishes normality, the anomaly supplies the joke, and the people sell the deadpan tone.

## Generation scaffold

```text
Use case: stylized-concept
Asset type: <preview, storyboard still, editorial image, or requested use>
Primary request: Create a completely original still. In <mundane location>, <one clear impossible event>. <People continue an ordinary activity and react minimally>.
Input images: <Image 1...N are visual-language references only; do not reproduce their people, props, locations, text, or composition.>
Style/medium: Authentic late-1990s/early-2000s consumer MiniDV/VHS camcorder frame; amateur found-footage realism; underground prank or skate-tape energy; photographic, not an illustration.
Composition/framing: 4:3 landscape; <awkward handheld viewpoint>; slightly crooked horizon; imperfect crop; modest consumer-camera zoom.
Lighting/mood: <direct flash, flat fluorescent light, overcast daylight, or mixed practical light>; low dynamic range; imperfect white balance; mundane and emotionally flat.
Materials/textures: <specific ordinary surfaces>; restrained chroma bleed, RGB edge fringing, interlacing, tape noise, compression blocks, edge ringing, and motion softness.
Constraints: One anomaly only; keep physics and materials believable outside that anomaly; new people, new location, new action, and new composition; no readable brands, logos, captions, dates, interface overlays, or watermark.
Avoid: Polished cinematic lighting, dramatic depth of field, glossy CGI, cyberpunk color, horror staging, fantasy atmosphere, theatrical reactions, slapstick posing, excessive glitches, and a clean modern-camera look.
```

## Correction patterns

Apply only the correction that addresses the observed failure.

- **Too polished:** Keep the subject and staging unchanged. Replace cinematic lighting with flat practical light and weak direct flash; lower dynamic range; introduce consumer-lens softness and modest compression.
- **Looks like an Instagram filter:** Keep the palette restrained. Reduce decorative grain and light leaks; add structural video defects such as interlacing, chroma bleed, edge ringing, and imperfect white balance.
- **Too dreamlike or fantastical:** Keep only the central anomaly. Restore realistic materials, ordinary architecture, practical lighting, and routine human behavior everywhere else.
- **Too comedic or staged:** Remove exaggerated expressions and poses. Give each person a normal task and mild or absent reaction; shift to an accidental handheld composition.
- **The anomaly is unclear:** Simplify its silhouette, remove competing oddities, and frame it against an ordinary surface at readable scale.
- **Too similar to a reference:** Change the location category, human activity, anomaly mechanism, viewpoint, and foreground while preserving only camera texture and tonal restraint.
- **Artifacts overpower the image:** Reduce glitch intensity; preserve only edge fringing, light tape noise, gentle motion softness, and low-bitrate texture.

## Original concept seeds

Use these only as structural examples; invent new specifics for the user's request.

- A mundane service counter processes an object that cannot fit through the building, while the queue advances normally.
- A maintenance worker carefully repairs the wrong category of object using an ordinary tool.
- A large office appliance appears permanently integrated into outdoor infrastructure while pedestrians navigate around it.
- A vehicle control is replaced with a domestic object, and the driver performs a serious functional test.
