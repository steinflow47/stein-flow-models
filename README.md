# Stein Flow — Models

Ready-made models for Stein Flow, to download and use.

**Flint** · steinflow47@users.noreply.github.com

## Models

| Model | Task | What it does | Download |
|---|---|---|---|
| **OWLv2, 768 px** | prompt | finds what a few boxes or words show it, without training - the base of a prompt set | [owlv2-768.zip](https://github.com/steinflow47/stein-flow-models/releases/download/owlv2-768-v2/owlv2-768.zip) (615 MB) |
| **D-FINE-N, 640 px** | detection | finds COCO's 80 kinds of objects, up to 300 a picture | [dfine-n-640.zip](https://github.com/steinflow47/stein-flow-models/releases/download/dfine-n-640-v1/dfine-n-640.zip) (15 MB) |
| **D-FINE-N, 416 px** | detection | the same at 416 px: faster, small objects less well | [dfine-n-416.zip](https://github.com/steinflow47/stein-flow-models/releases/download/dfine-n-416-v1/dfine-n-416.zip) (15 MB) |
| **D-FINE-N lite, 416 px** | detection | COCO's 80 kinds, up to 100 a picture: faster on a processor | [dfine-n-lite-416.zip](https://github.com/steinflow47/stein-flow-models/releases/download/dfine-n-lite-416-v1/dfine-n-lite-416.zip) (15 MB) |
| **D-FINE-N lite, 320 px** | detection | the fastest: COCO's 80 kinds, up to 100 a picture | [dfine-n-lite-320.zip](https://github.com/steinflow47/stein-flow-models/releases/download/dfine-n-lite-320-v1/dfine-n-lite-320.zip) (15 MB) |
| **DeiT-Tiny** | classification | tells ImageNet's 1000 kinds of things apart - Train Classify's starting network | [deit-tiny.zip](https://github.com/steinflow47/stein-flow-models/releases/download/deit-tiny-v1/deit-tiny.zip) (23 MB) |

Each model's page in `models/` says what it is made from, its licence, and which of its files you need.

## How to use one

1. Press the model's `.zip` in the table - it downloads at once - and unzip it: you get **one folder** (`owlv2_768/`), the model's
   files inside.
2. In Stein Flow: **Models** → **Add…** → choose that folder.
3. Choose where it runs in the Models window's **Device**: the processor, or an NVIDIA card.

`models.json` lists every model: its zip's size and sha256, and each file inside, so a download can be checked:

```bash
sha256sum owlv2-768.zip
```

## SAM, for the labeler's SAM tool

SAM's weights are not in this repository: download them from Meta, its makers, under their own licence
(SAM 2: Apache 2.0, [facebookresearch/sam2](https://github.com/facebookresearch/sam2)).

| Model | Size | Download (Meta) |
|---|---|---|
| SAM 2.1 tiny | 38.9 M parameters | [sam2.1_hiera_tiny.pt](https://dl.fbaipublicfiles.com/segment_anything_2/092824/sam2.1_hiera_tiny.pt) |
| SAM 2.1 small | 46 M | [sam2.1_hiera_small.pt](https://dl.fbaipublicfiles.com/segment_anything_2/092824/sam2.1_hiera_small.pt) |
| **SAM 2.1 base+** (start here) | 80.8 M | [sam2.1_hiera_base_plus.pt](https://dl.fbaipublicfiles.com/segment_anything_2/092824/sam2.1_hiera_base_plus.pt) |
| SAM 2.1 large | 224.4 M | [sam2.1_hiera_large.pt](https://dl.fbaipublicfiles.com/segment_anything_2/092824/sam2.1_hiera_large.pt) |

1. Put the `.pt` file in the SAM models folder, which Stein Flow makes when it starts - the SAM tool's panel →
   **Models folder** opens it: `~/_stein_flow/models/sam` (Windows: `%USERPROFILE%\_stein_flow\models\sam`).
   Keep the file's name as it downloads.
2. Choose the SAM tool again: the model shows in its list (`sam2.1-base` for base+). Several may sit
   side by side.

Check base+'s download: `sha256sum sam2.1_hiera_base_plus.pt` gives
`a2345aede8715ab1d5d31b4a509fb160c5a4af1970f199d9054ccfb746c004c5`.

## Licences

The models are made from others' published work, each under its own licence, named on its page in `models/`;
the licence texts are in `LICENSES/`. No endorsement by their authors is implied. The files are packaged for
Stein Flow and open in it.

---
© Flint. Stein Flow is proprietary; this repository holds models for it, never its source.
