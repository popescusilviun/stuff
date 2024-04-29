# ai-codeassist-ollama-continue

> Local AI code assist in IDEs with ollama.

`ollama` is a tool to install and manage LLM (Large Language Model) locally. Once installed, the LLM can be used in different coding (but not only) tasks.

`condinue` is an opensource Visual Studio Code / VSCodium and JetBrains plugin that integrates LLMs into the IDE.

## install LLMs

- macOs instruction

```sh
# install ollama and run it as a background service
brew install ollama
brew services start ollama

# install some LLMs
ollama pull starcoder2:3b   # coding specialized LLM, used for autocompletion
ollama pull llama3          # generic LLM
```

## IDE plugin configuration

- install the [continue.dev](https://www.continue.dev) IDE plugin

- configure `continue` to use your local LLMs
    - edit the `~/.continue/config.json` (on VSCode, call the command `Continue: Open config.json`)
    - add or replace local LLMs in the `models` section, optionnaly disable telemetry

```json
{
    "models": [
        {
            "title": "llama3",
            "provider": "ollama",
            "model": "llama3",
            "completionOptions": {}
        },
        {
            "title": "starcoder2 (code)",
            "provider": "ollama",
            "model": "starcoder2:3b",
            "completionOptions": {}
        },
    ],

    ...

    "allowAnonymousTelemetry": false
}  
```
