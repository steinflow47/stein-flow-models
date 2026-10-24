# DeiT-Tiny - for Stein Flow

A classifier: it says which of ImageNet's 1000 kinds of things a picture shows, best first. In Stein Flow: an
ai_vision/Classify node's model; its map shows where in the picture it looked.

**Made from** [facebookresearch/deit](https://github.com/facebookresearch/deit)'s DeiT-Tiny weights trained on ImageNet-1k
(Touvron et al., *Training data-efficient image transformers & distillation through attention*, 2021), licensed
under the Apache License 2.0 ([LICENSES/Apache-2.0.txt](../../LICENSES/Apache-2.0.txt)). Its weights were converted
for Stein Flow; the network and what it answers are the original's. No endorsement by the authors or by Meta is
implied.

It was trained on ImageNet-1k, whose terms of access bind those who download that database; this model holds no
picture of it.

## Files

`deit-tiny.zip` holds one folder, `deit_tiny/`:

| file | what it is |
|---|---|
| `deit_tiny.stmc` | the model, 224 x 224 px |
| `meta.json` | what the model is, its labels, for Stein Flow |

Unzip it and add the folder in Stein Flow (Models → Add…). It runs on the processor or on an NVIDIA card; choose in
the Models window's Device.
