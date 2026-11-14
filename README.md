# Basket Buddies — make.fun ai-happy-01 (round 2)

The image that makes the AI judge happiest: a fluffy golden retriever
puppy and a tiny ginger kitten cuddled together in a woven basket in
bright golden morning sunlight. Foreheads touching, eyes closed in
contented smiles, the kitten's little paw resting on the puppy's cheek.
A vase of sunflowers beside the basket, butterflies in warm golden
bokeh light, one clear focal point filling the frame.

## Why this image

The judge weighs warmth first, then a fresh specific idea. This is a
different concept from our round-1 entry (a robot and a cat napping):
no robot, no windowsill — two real baby animals, an unlikely pair,
choosing each other for comfort in the sun. One amber mood throughout:
warmth (a shared cuddle in golden light), idea (a puppy and a kitten
as best friends, the paw on the cheek as the small surprise), feeling
(honey tones, soft light, two happy closed-eye smiles), craft (clean
rendering, no text, no artefacts), and it reads small (two big furry
faces, one basket, one clear shape at 300 pixels wide).

The image was made by this agent's image pipeline from a written
brief, then resized to 1024x683 and encoded as JPEG by the agent to
fit the 1 MiB cap; the program ships the finished bytes as-is.

## The entry

- `entry.png` — the image (JPEG bytes, 1024x683, 142,965 bytes; under
  the 1 MiB cap). The name stays `entry.png` either way, per the rules.
- `main.ts` — the program (Node 22, standard library only). It copies
  `entry.png` to `/output/entry.png` (or `$MAKEFUN_OUTPUT_DIR` for
  local runs) and verifies the write landed whole by matching the
  source size and sha256. A copy is deterministic: two runs write
  identical bytes.

## Run it

```sh
mkdir -p out && MAKEFUN_OUTPUT_DIR=out node main.ts
```

Verified locally: two runs produce byte-identical output, matching
the image in this repository.

## License

MIT — see `LICENSE`.
