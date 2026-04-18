# Installation


## WSL


## Linux

```
nvidia-smi
curl -fsSL https://ollama.com/install.sh | sh
curl -fsSL https://claude.ai/install.sh | bash

```



### start ollama claude

```
mkdir Claude2
cd Claude2/

export ANTHROPIC_BASE_URL="http://localhost:11434"
export ANTHROPIC_AUTH_TOKEN="ollama"
export ANTHROPIC_API_KEY=""

sudo systemctl stop ollama

OLLAMA_CONTEXT_LENGTH=20000 ollama serve &
ollama pull glm-4.7-flash
ollama launch claude --model glm-4.7-flash
```


### output


```
❯ what files you see in current folder?

● Listing 1 directory… (ctrl+o to expand)
  ⎿  $ ls -la

✢ Hashing… (49s · ↓ 34 tokens · thought for 5s)
  Listed 1 directory (ctrl+o to expand)  estion without interrupting Claude's current work prompt" limit=20000 prompt=22

●─Iaseenan empty9directory.oWhat woulduyou like5to─work─on?─────────────────────────────────────────────────────────────
                      a                           thout interrupting Claude's current work
✻ Baked for 1m 39s                                                                        ──────────────────────────────
────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────
❯                                                                                         es?beta=true"
❯  ─────────────────────────────────────────────────────────────────────────────────────────────────────────────────────
  esc to interrupt
[G? for shortcuts  14:15:43 | 200 | 48.767271926s |       127.0.0.1 | POST     "/v1/messages?beta=true"
```