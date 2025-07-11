# 🌀 OpenAI Compatible Reverse Proxy

Exactly what it says on the tin:
Plug in your API key, set the endpoint, choose your port — fire it up — and *presto!* You’ve got your very own AI Endpoint, no fancy wallet required.

## ⚙️ How It Works

1. Drop your `API_KEY`, `API_ENDPOINT`, and `PORT` in a `.env` file.
2. Run the thing.
3. Point your apps at it like it’s OpenAI — because it *is* (sort of).

## ✅ What Works

* **Sequential requests** — like a polite line at the post office.
* Perfect for cheapskates (hello, yes, it’s me) who just want their LLM fix without paying for fancy concurrency.

## 🧪 Coming Soon™

* 🔑 **Multi-Key Support** — so you don’t get rate-limited into oblivion.
* 🔗 **Multi-Provider Support** — run OpenRouter, local models, or your neighbor’s AI rig.
* ⚡ **Parallel Processing** — so your requests can run like caffeinated squirrels instead of a single sloth.

## 🚀 Quickstart

```bash
# 1️ Clone it
git https://github.com/Iteranya/AnyReverseProxy.git
cd AnyReverseProxy

# 2️ Make your environment
python -m venv/venv
venv/scripts/activate (in windows)
source venv/bin/activate (in linux)
cp .env.example .env

# Example .env
# --------------------------
# API_ENDPOINT=https://openrouter.ai/api/v1
# API_KEY=MLEM
# PORT=5000
# --------------------------

# 3️ Install dependencies
pip install -r requirements.txt

# 4️ Run it
python main.py
```

Now hit `http://localhost:PORT` with your OpenAI-compatible requests. Models, completions, chat — all yours, baby.

## 📌 Notes

* This proxy just forwards your requests — the actual magic still happens at the real endpoint.
* Keep your API key safe. Or don’t. I’m not your mom.
* Contributions, feature ideas, or bribes welcome.

---

### ⚡ License

AGPL-3, Like All Of My Project