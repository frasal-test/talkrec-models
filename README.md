# TalkRec models

Fixed copies of the speech models that [TalkRec](https://talkrec.app) downloads on its first start.
TalkRec checks every file against the SHA-256 below before using it, so a file that changes
upstream cannot reach a Mac by surprise. A new upstream version is adopted on purpose, after it has
been checked, as a new release here.

The files are redistributed unchanged, under their own licences (see `LICENSES/`).

| Release | File | Size (bytes) | SHA-256 | Licence | Source |
|---|---|---|---|---|---|
| `campplus-1` | `3dspeaker_speech_campplus_sv_zh_en_16k-common_advanced.onnx` | 28281164 | `aa3cfc16963a10586a9393f5035d6d6b57e98d358b347f80c2a30bf4f00ceba2` | Apache-2.0 | CAM++ speaker model of the [3D-Speaker](https://github.com/modelscope/3D-Speaker) project (Alibaba, ModelScope), ONNX export of [sherpa-onnx](https://github.com/k2-fsa/sherpa-onnx/releases/tag/speaker-recongition-models), as published there until November 2026 |
| `whisper-large-v3-turbo-q5_0-1` | `ggml-large-v3-turbo-q5_0.bin` | 574041195 | `394221709cd5ad1f40c46e6031ca61bce88931e6e088c188294c6d5a55ffa7e2` | MIT | [OpenAI Whisper](https://github.com/openai/whisper) large-v3-turbo, Copyright (c) 2022 OpenAI; ggml q5_0 conversion of [whisper.cpp](https://huggingface.co/ggerganov/whisper.cpp), Copyright (c) 2023-2026 The ggml authors |

Licence texts: `LICENSES/Apache-2.0.txt` (CAM++), `LICENSES/MIT-OpenAI-Whisper.txt` and
`LICENSES/MIT-whisper.cpp.txt` (Whisper). The models are not covered by any other licence of TalkRec.
