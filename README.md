# ComfyUI-Dart
![Dart Preview](workflows/dart_generate_with_config.png)  
日本語版READMEは[こちら](README.jp.md)。

- Custom node for [ComfyUI](https://github.com/comfyanonymous/ComfyUI).
- Add nodes that generates danbooru tags by [Dart(Danbooru Tags Transformer)](https://huggingface.co/p1atdev/dart-v1-sft).

## Installation
```
cd <ComfyUI directory>/custom_nodes
git clone https://github.com/nkchocoai/ComfyUI-Dart.git
```

## Nodes
### Dart Generate
- Generate danbooru tags by [Dart(Danbooru Tags Transformer)](https://huggingface.co/p1atdev/dart-v1-sft).
- See the following URL for the syntax of prompt.
  - https://huggingface.co/p1atdev/dart-v1-sft#prompt-guidde
- Tags specified with `remove_tags` will not be output.

### Dart Compose Prompt
- Output input "prompt" of Dart Generate node.

### Dart Generation Config
- Output input "config" of Dart Generate node.

### Dart Generate(Advanced)
- Output a token ID sequence of danbooru tags generated by [Dart(Danbooru Tags Transformer)](https://huggingface.co/p1atdev/dart-v1-sft).
- See the following URL for the syntax of prompt.
  - https://huggingface.co/p1atdev/dart-v1-sft#prompt-guidde

### Dart Decode
- Decode the token ID sequence.

### Dart Rearranged By Animagine
- Rearrange the token ID sequence in the order of Animagine prompt.

### Dart Decode By Splited Parts
- Output decoded strings of the token ID sequence split by part.

### Dart Remove Tag Token
- Remove the specified tag from the token ID sequence.
