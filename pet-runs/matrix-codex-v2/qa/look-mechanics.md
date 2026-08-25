# Matrix Codex look mechanics

## Natural movement

Matrix Codex is a compact cybernetic black cat with a separate round head, large physical green eyeballs, angular ears, a seated torso, planted front paws, and a raised cable-like tail. The gaze should lead with rotation of both complete eye globes inside their existing apertures, including iris, pupil, sclera glow, eyelid rim, and highlights. The head then yaws or pitches subtly, with the ears following the head as rigid attached parts. The torso, paws, lower-body contact point, tail base, circuitry pattern, and overall scale stay anchored. The tail may have only a tiny continuous follow-through near its tip; it must never flip sides or detach.

Do not slide pupils over a fixed eye surface, add replacement eye whites, or paint a second eye layer. Do not rotate, skew, tilt, or warp the whole sprite. Preserve the exact pixel-art face, black material, neon-green circuitry, proportions, silhouette, and seated-cat identity. There are no props.

## Cardinal pose families

- **000 up:** both complete eyeballs rotate upward with visible lower-eye exposure; the muzzle and nose lift slightly, the chin opens away from the chest, and the ears follow the small upward head pitch. The body and paws remain fixed. This must read as looking above the pet, not neutral/front.
- **090 screen-right:** both eyes and nose move unmistakably to the viewer's screen-right of the head center. The head yaws right; the screen-right eye/cheek becomes slightly more side-on and compressed while the opposite side remains fuller. The rightward face contour and ear relationship must support the turn.
- **180 down:** both complete eyeballs rotate downward with visible upper-eye exposure; the muzzle and nose tuck toward the chest, upper eyelids lower slightly, and the ears follow the restrained downward pitch. This must read as looking below, not sad or failed.
- **270 screen-left:** exact semantic opposite of 090. Both eyes and nose move unmistakably to the viewer's screen-left of the head center. The head yaws left; the screen-left eye/cheek becomes slightly more side-on and compressed while the opposite side remains fuller.

## Continuity and motion budget

Treat the 16 poses as one clockwise loop. Every 22.5-degree step should change eye rotation first and head/ear orientation second by roughly the same visual amount. Keep baseline, body height, lower-body anchor, paw spacing, tail base, and circuitry placement stable. Diagonals interpolate both required axes without snapping or pausing at a cardinal. The transition `157.5 -> 180` must continue smoothly into the downward family, and `337.5 -> 000` must close the loop with one equal final step. No adjacent pose may reverse direction, jump registration, change scale, alter facial proportions, or switch the tail to another side.
