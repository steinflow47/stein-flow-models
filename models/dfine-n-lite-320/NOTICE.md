# D-FINE-N lite, 320 px - for Stein Flow

A detector: it finds the 80 kinds of objects of COCO - people, vehicles, animals, everyday things - with a box and a
confidence for each. In Stein Flow: an ai_vision/Detect node's model.

**Made from** [Peterande/D-FINE](https://github.com/Peterande/D-FINE)'s D-FINE-N checkpoint trained on COCO 2017 (Peng et
al., *D-FINE: Redefine Regression Task in DETRs as Fine-grained Distribution Refinement*, 2024), licensed under the
Apache License 2.0 ([LICENSES/Apache-2.0.txt](../../LICENSES/Apache-2.0.txt)). Its weights were converted for Stein
Flow, to run at 320 px with 100 queries instead of 300 (it finds at most 100 objects in a picture; faster). No endorsement by the authors is implied.

It was trained on COCO 2017, whose annotations are CC BY 4.0 and whose pictures are Flickr's, each under its own
terms; this model holds no picture of it.

## Files

`dfine-n-lite-320.zip` holds one folder, `dfine_n_lite_320/`:

| file | what it is |
|---|---|
| `dfine_n_lite_320.stmd` | the model, 320 x 320 px |
| `meta.json` | what the model is, its labels, for Stein Flow |

Unzip it and add the folder in Stein Flow (Models → Add…). It runs on the processor or on an NVIDIA card; choose in
the Models window's Device.
