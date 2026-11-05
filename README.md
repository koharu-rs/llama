# Llama runtime for Koharu

Daily prebuilt [llama.cpp](https://github.com/ggml-org/llama.cpp) shared libraries for [Koharu](https://github.com/mayocream/koharu).

The release workflow resolves the newest listed llama.cpp release, including prereleases, and builds CUDA, HIP, Vulkan, and Metal variants for Windows, Linux, and macOS. It runs daily at 03:17 UTC, on pushes to `main`, and when started manually.

Build jobs use the standard `ubuntu-latest`, `windows-latest`, and `macos-latest` GitHub-hosted runners.

Each archive holds `llama`, `mtmd`, and `llama-common`. `llama-common` is llama.cpp's common library with the C wrapper in [`cmake/wrapper`](cmake/wrapper), from [llama-cpp-rs](https://github.com/utilityai/llama-cpp-rs), so callers that load it at runtime can use it through `llama_rs_*` functions.

Generated binaries are published through this repository's [releases](https://github.com/koharu-org/llama/releases).

## License

This repository is dual-licensed under the [MIT License](LICENSE-MIT) or the
[Apache License, Version 2.0](LICENSE-APACHE), at your option.

Third-party code and dependencies retain their respective licenses.
