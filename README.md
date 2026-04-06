# GuppyLM Workshop — Train a Tiny LLM Persona in 5 Minutes

A Google Colab-ready workshop kit for training a 9M parameter transformer with a custom personality. Built for corporate AI training sessions where participants can't install anything — just open a browser link and chat.

## What's Inside

| File | Description |
|------|-------------|
| `guppylm_workshop.ipynb` | Colab notebook — training loop, Gradio chat interface, 3 persona presets |
| `tech_grandma.jsonl` | 200 Q&A pairs — "Tech Grandma" persona (warm babcia who knows tech) |

## How to Use

1. Upload `guppylm_workshop.ipynb` to [Google Colab](https://colab.research.google.com)
2. Upload `tech_grandma.jsonl` to the same Colab session
3. **Runtime → Change runtime type → T4 GPU** (free tier)
4. Run all cells top to bottom
5. Gradio generates a public `*.gradio.live` link — share it with participants
6. They chat with the trained persona in any browser, no install needed

## Built-in Personas

The notebook includes 3 preset personas:
- **Tech Grandma** — loads from the included JSONL (200 pairs)
- **Sarcastic Coach** — 20 inline examples (expandable)
- **Noir Detective** — 20 inline examples (expandable)

Participants can also upload their own JSONL dataset (instruction/input/output format).

## Workshop Flow

1. **Demo (5 min):** Show Colab training on projector, chat with all 3 personas
2. **Exercise (20 min):** Participants write Q&A pairs in a shared Google Sheet
3. **Live Train (5 min):** Copy sheet → JSONL → upload → train on stage
4. **Chat (10 min):** New Gradio link — they talk to their own creation

## Dataset Format

```jsonl
{"instruction": "How do I fix slow WiFi?", "input": "", "output": "Honey, try restarting the router first..."}
```

## Credits

Model architecture based on [GuppyLM](https://github.com/arman-bd/guppylm) by Arman (MIT License).
