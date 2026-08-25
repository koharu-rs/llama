# Llama runtime for Koharu

Weekly prebuilt [llama.cpp](https://github.com/ggml-org/llama.cpp) shared libraries for [Koharu](https://github.com/mayocream/koharu).

The release workflow resolves the newest listed llama.cpp release, including prereleases, and builds CUDA, HIP, Vulkan, and Metal variants for Windows, Linux, and macOS. It runs every Sunday at 03:17 UTC and can also be started manually.

Build jobs use the `ubuntu-latest-16-cores`, `windows-latest-8-cores`, and `macos-latest-xlarge` GitHub-hosted larger runners.

Generated binaries are published through this repository's [releases](https://github.com/koharu-org/llama/releases).
