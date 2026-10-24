# OWLv2, 768 px - for Stein Flow

A prompt model: shown boxes on a few pictures, or told words, it finds those things in new pictures without
training. In Stein Flow it is the base of a prompt set (Models window, **Add…**, then the set's prompts).

**Made from** [google/owlv2-base-patch16-ensemble](https://huggingface.co/google/owlv2-base-patch16-ensemble)
(Minderer, Gritsenko and Houlsby, *Scaling Open-Vocabulary Object Detection*, 2023), licensed under the Apache
License 2.0 ([LICENSES/Apache-2.0.txt](../../LICENSES/Apache-2.0.txt)). Its weights were converted for Stein Flow;
the network and what it answers are the original's. No endorsement by the authors or by Google is implied.

The text part reads words with CLIP's byte-pair vocabulary, which comes with the model above; CLIP's vocabulary is
© 2021 OpenAI under the MIT License ([LICENSES/MIT-CLIP.txt](../../LICENSES/MIT-CLIP.txt)).

## Files

`owlv2-768.zip` holds one folder, `owlv2_768/`:

| file | what it is |
|---|---|
| `owlv2_768.stmp` | the picture part |
| `owlv2_768_text.stmp` | the text part: prompts in words (English); without it the model takes boxes only |
| `meta.json` | what the model is, for Stein Flow |

Unzip it and add the folder in Stein Flow. It runs on the processor or on an NVIDIA card; choose in the Models
window's Device.
