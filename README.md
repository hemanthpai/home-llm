# Local LLM
This project is a fork of the Home LLM Home Assistant integration originally created by [acon96](https://github.com/acon96/home-llm/tree/develop). This project deviates from the original by focusing exclusively on integration with a LLM that's running locally on capable hardware (i.e. not the RPI or similar hardware that's running Home Assistant). For example, Llama 3.1 running on an NVIDIA 4090 through Local AI or vLLM.

## Quick Start
Please see the [Setup Guide](./docs/Setup.md) for more information on installation.

## Local LLM Conversation Integration
In order to integrate with Home Assistant, we provide a custom component that exposes the locally running LLM as a "conversation agent".

This component can be interacted with in a few ways:  
- using a chat interface so you can chat with it.
- integrating with Speech-to-Text and Text-to-Speech addons so you can just speak to it.

The LLM is assumed to be running on a different machine through one of the following ways:
- [LocalAI](https://localai.io/) via the Generic OpenAI backend (easier)
- [vLLM](https://docs.vllm.ai/en/stable/getting_started/quickstart.html) via the Open AI server (advanced)

The following alternatives may work as well:
- [Ollama](https://ollama.com/) (easier)
- [oobabooga/text-generation-webui](https://github.com/oobabooga/text-generation-webui) project (advanced)
- [llama.cpp example server](https://github.com/ggerganov/llama.cpp/blob/master/examples/server/README.md) (advanced)
