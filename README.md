# Homebrew tap for FastLLM

Formulae for [FastLLM](https://github.com/c-vision/FastLLM) (run MLX and GGUF language models locally on Apple Silicon) and the
[LLMEnv](https://github.com/c-vision/LLMEnv) engine it uses.

```sh
brew tap c-vision/fastllm
brew trust c-vision/fastllm      # Homebrew 7 does not load a third-party tap until you trust it
brew install fastllm             # also installs llmenv
```

`brew install llmenv` installs only the engine. On macOS 26.2 and later you get the engine build with the NAX kernels; on macOS 14 and 15
you get the compatible build. Upgrade with `brew upgrade fastllm`.

Not Homebrew? `curl -fsSL https://github.com/c-vision/FastLLM/releases/latest/download/install.sh | bash` does the same without sudo.
