# Install a pet in ChatGPT Work

1. Download this repository as a ZIP and unzip it.
2. Choose one pet folder under `pets/`.
3. In a ChatGPT Work or Codex chat with the **Pets** capability available, attach that pet's `spritesheet.png`.
4. Ask:

   > Create and activate a custom ChatGPT Work pet named **PET NAME** using this exact v2 sprite sheet. Validate it first, preserve the exact bytes, and keep the returned stable pet ID.

5. After creation, ask the assistant to list the pet library and confirm the new pet is active.

Suggested names and descriptions are in [`manifest.json`](manifest.json).

## Important

- Upload `spritesheet.png`, not the preview GIF or contact sheet.
- Do not crop, resize, flatten, recolor, or pass the sheet through an image optimizer.
- Creation makes a new owned copy in the recipient's pet library. It does not reuse the original owner's pet ID.
- If ChatGPT reports that the Pets capability is unavailable, the recipient's current workspace or account does not expose custom pet creation yet.

## Sheet layout

The v2 atlas has 11 rows:

1. idle — 6 frames
2. running right — 8 frames
3. running left — 8 frames
4. waving — 4 frames
5. jumping — 5 frames
6. failed — 8 frames
7. waiting — 6 frames
8. active work — 6 frames
9. review — 6 frames
10. look directions 000°–157.5° — 8 frames
11. look directions 180°–337.5° — 8 frames

The unused cells at the right ends of shorter rows must remain fully transparent.
