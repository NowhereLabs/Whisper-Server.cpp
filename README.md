# whisper.cpp

![whisper.cpp](https://user-images.githubusercontent.com/1991296/235238348-05d0f6a4-da44-4900-a1de-d0707e75b763.jpeg)
[![License: MIT](https://img.shields.io/badge/license-MIT-blue.svg)](https://opensource.org/licenses/MIT)

## Deploy server with base.en

Prerequisites

Before you begin, ensure you have the following installed on your system:

    wget: A utility for downloading files from the web.
    make: A build automation tool that automatically builds executable programs from source code.
    A compatible C++ compiler (e.g., g++ or clang) to build the server.

Instructions

Follow the steps below to download the Whisper model and start the server:

    Download the Whisper Model

    Use the following command to download the Whisper model binary file from Hugging Face:

    bash

wget -P models/ https://huggingface.co/ggerganov/whisper.cpp/resolve/main/ggml-base.en.bin

You can download and run the other models as follows:

```
make -j tiny.en
make -j tiny
make -j base.en
make -j base
make -j small.en
make -j small
make -j medium.en
make -j medium
make -j large-v1
make -j large-v2
make -j large-v3
make -j large-v3-turbo
```

## Memory usage

| Model  | Disk    | Mem     |
| ------ | ------- | ------- |
| tiny   | 75 MiB  | ~273 MB |
| base   | 142 MiB | ~388 MB |
| small  | 466 MiB | ~852 MB |
| medium | 1.5 GiB | ~2.1 GB |
| large  | 2.9 GiB | ~3.9 GB |
