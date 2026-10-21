# Storify voice models

Download mirror for the Natural voices in [Storify](https://apps.apple.com/app/id6742459979). The app fetches these files only if the Apple-hosted download is unavailable, and it checks every file against a pinned SHA-256 before using it.

Each release is named after the pinned upstream revisions, `pocket-<model>-<voices>`. The files are unmodified copies of:

- [KevinAHM/pocket-tts-onnx](https://huggingface.co/KevinAHM/pocket-tts-onnx), ONNX export of [Kyutai Pocket TTS](https://huggingface.co/kyutai/pocket-tts): weights CC BY 4.0, export code Apache 2.0
- [kyutai/pocket-tts-without-voice-cloning](https://huggingface.co/kyutai/pocket-tts-without-voice-cloning): voice embeddings, CC BY 4.0 / CC0. Only those voices are mirrored.

Asset names are `<language>--<path with "/" replaced by "--">`, e.g. `english_2026-04--voices--alba.safetensors`.

Full attribution: [NOTICE.txt](NOTICE.txt). Licenses: [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/), [CC0](https://creativecommons.org/publicdomain/zero/1.0/), [Apache 2.0](https://www.apache.org/licenses/LICENSE-2.0).
