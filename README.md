# Lesoma voice models

Download mirror for the voices in [Lesoma](https://apps.apple.com/app/id6742459979) (formerly Storify). The app fetches these files only if the Apple-hosted download is unavailable, and it checks every file against a pinned SHA-256 before using it.

## Natural voices

Each release is named after the pinned upstream revisions, `pocket-<model>-<voices>`. The files are unmodified copies of:

- [KevinAHM/pocket-tts-onnx](https://huggingface.co/KevinAHM/pocket-tts-onnx), ONNX export of [Kyutai Pocket TTS](https://huggingface.co/kyutai/pocket-tts): weights CC BY 4.0, export code Apache 2.0
- [kyutai/pocket-tts-without-voice-cloning](https://huggingface.co/kyutai/pocket-tts-without-voice-cloning): voice embeddings, CC BY 4.0 / CC0. Only those voices are mirrored.

Asset names are `<language>--<path with "/" replaced by "--">`, e.g. `english_2026-04--voices--alba.safetensors`.

## Standard voices

Release `supertonic-3-<upstream commit>` holds the four ONNX weight files of [Supertone/supertonic-3](https://huggingface.co/Supertone/supertonic-3) at commit `3cadd1ee6394adea1bd021217a0e650ede09a323`, unmodified, under their upstream names (`duration_predictor.onnx`, `text_encoder.onnx`, `vector_estimator.onnx`, `vocoder.onnx`).

Copyright (c) 2026 Supertone Inc. The model is licensed under the BigScience OpenRAIL-M licence: [Supertonic-LICENSE.txt](Supertonic-LICENSE.txt). **Use of these files is subject to the use restrictions in paragraph 5 and Attachment A of that licence**; anyone who receives or redistributes them is bound by the same restrictions. The licence text is also attached to the release.

## Studio voices

Releases `qwen3-base-8bit-50f45ef` (Mac) and `qwen3-base-4bit-0d6bb6f` (iPhone) hold the MLX conversions of [Qwen/Qwen3-TTS-12Hz-0.6B-Base](https://huggingface.co/Qwen/Qwen3-TTS-12Hz-0.6B-Base), unmodified copies of:

- [mlx-community/Qwen3-TTS-12Hz-0.6B-Base-8bit](https://huggingface.co/mlx-community/Qwen3-TTS-12Hz-0.6B-Base-8bit) at commit `50f45ef0047cde7e84c2ef04326acb8ada2436a7`
- [mlx-community/Qwen3-TTS-12Hz-0.6B-Base-4bit](https://huggingface.co/mlx-community/Qwen3-TTS-12Hz-0.6B-Base-4bit) at commit `0d6bb6fe33f92d47a507e23b9148940e8366ab5b`

Licensed under the Apache License 2.0: [Apache-2.0-LICENSE.txt](Apache-2.0-LICENSE.txt), also attached to both releases. Asset names are the upstream paths with `/` replaced by `--`, e.g. `speech_tokenizer--model.safetensors`.

## Notices

Full attribution: [NOTICE.txt](NOTICE.txt). Licenses: [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/), [CC0](https://creativecommons.org/publicdomain/zero/1.0/), [Apache 2.0](Apache-2.0-LICENSE.txt), [BigScience OpenRAIL-M](Supertonic-LICENSE.txt).
