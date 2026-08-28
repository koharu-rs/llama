# Llama runtime for Koharu

Daily prebuilt [llama.cpp](https://github.com/ggml-org/llama.cpp) shared libraries for [Koharu](https://github.com/mayocream/koharu).

The release workflow resolves the newest listed llama.cpp release, including prereleases, and builds CUDA, HIP, Vulkan, and Metal variants for Windows, Linux, and macOS. It runs daily at 03:17 UTC, on pushes to `main`, and when started manually.

Build jobs use the standard `ubuntu-latest`, `windows-latest`, and `macos-latest` GitHub-hosted runners.

Generated binaries are published through this repository's [releases](https://github.com/koharu-org/llama/releases).
