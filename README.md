# hf-claude

extension for `hf` to launch Claude Code with Hugging Face Inference Providers

It lets you pick:
- model (from `https://router.huggingface.co/v1/models`)
- provider (`auto` or a concrete provider for the selected model)

Then it runs `claude --model <model[:provider]>` with router env vars preconfigured.

## Requirements

- Claude Code CLI Installed
- `curl`, `jq`, `fzf`, `bash`
- `HF_TOKEN` set:

```bash
export HF_TOKEN='hf_...'
```

## Install

```bash
hf extensions install hanouticelina/hf-claude
```

## Run

```bash
hf claude
# or
hf extensions exec claude
```

Forward extra args to Claude Code:

```bash
hf claude --help
hf extensions exec claude -- --help
```
