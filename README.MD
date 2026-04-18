# Installation


## WSL


## Linux

```
nvidia-smi
curl -fsSL https://ollama.com/install.sh | sh
mkdir Claude2
cd Claude2/
curl -fsSL https://ollama.com/install.sh | sh
curl -fsSL https://claude.ai/install.sh | bash
```



### start ollama claude

```
export ANTHROPIC_BASE_URL="http://localhost:11434"
export ANTHROPIC_AUTH_TOKEN="ollama"
export ANTHROPIC_API_KEY=""

sudo systemctl stop ollama

OLLAMA_CONTEXT_LENGTH=20000 ollama serve &
ollama pull glm-4.7-flash
ollama launch claude --model glm-4.7-flash
```


