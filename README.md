# Stein Flow — Models

Ready-made models for Stein Flow, to download and use.

**Flint** · steinflow47@users.noreply.github.com

## Models

| Model | Task | What it does | Download |
|---|---|---|---|
| **OWLv2, 768 px** | prompt | finds what a few boxes or words show it, without training - the base of a prompt set | [Release `owlv2-768-v1`](https://github.com/steinflow47/stein-flow-models/releases/tag/owlv2-768-v1) |

Each model's page in `models/` says what it is made from, its licence, and which of its files you need.

## How to use one

1. Download the model's files from its Release into **one folder** (a model's files go together).
2. In Stein Flow: **Models** → **Add…** → choose that folder.
3. Choose where it runs in the Models window's **Device**: the processor, or an NVIDIA card.

`models.json` lists every model with its files, their sizes and sha256, so a download can be checked:

```bash
sha256sum owlv2_768.stmp owlv2_768_text.stmp meta.json
```

## Licences

The models are made from others' published work, each under its own licence, named on its page in `models/`;
the licence texts are in `LICENSES/`. No endorsement by their authors is implied. The files are packaged for
Stein Flow and open in it.

---
© Flint. Stein Flow is proprietary; this repository holds models for it, never its source.
