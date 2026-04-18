# Installation


## WSL


## Linux

```
   nvidia-smi
   curl -fsSL https://ollama.com/install.sh | sh
   mkdir Claude2
   cd Claude2/
   curl -fsSL https://ollama.com/install.sh | sh
   OLLAMA_CONTEXT_LENGTH=20000 ollama serve
   ollama ps
   curl -fsSL https://claude.ai/install.sh | bash
   ollama pull glm-4.7-flash
   systemctl restart ollama
```