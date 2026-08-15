# Agape Primitives

Three standalone, zero-dependency Python packages extracted from the OpenRoot / UNE work.

They implement a simple claim:

> Structure beats scale.  
> A small model + fractal recursion + thermodynamic accounting + coherence filtering  
> can outperform a large model that has none of those things — and you can prove it.

## The three packages

| Package | One-line purpose | Install |
|---------|------------------|---------|
| **etaledger** | η = useful_joules / human_joules. Measure the real cost of any computation. | `pip install -e ./etaledger` |
| **fractallattice** | Six complementary nanobots recurse on any LLM. Depth instead of width. | `pip install -e ./fractallattice` |
| **agaperesonance** | Multiple predictions enter. Noise cancels. The standing wave survives. | `pip install -e ./agaperesonance` |

No cloud required. No patents. GPL-3.0.

## Quick local test (Termux / any Linux)

```bash
cd agape_primitives
python3 demo_integration.py          # mock LLM, proves the plumbing
python3 real_llm_runner.py           # tries Ollama first, falls back cleanly
```

## Real LLM bridge

`real_llm_runner.py` will:

1. Try a local Ollama model (preferred — zero cost, offline).
2. Fall back to a simple mock if Ollama is not running.
3. Feed every nanobot output into the resonance filter.
4. Record η, Landauer cost, Merkle provenance, and the standing wave.

Replace the mock with any `async def call_fn(prompt: str, system: str) -> str` (llama.cpp, OpenAI-compatible, etc.).

## Why this exists

Most AI progress is “more parameters, more GPUs, more energy”.  
These packages ask the opposite question: how much useful work can you extract per joule of human attention and silicon energy?

etaledger makes the cost visible.  
fractallattice gives a small model six complementary jobs and lets the lattice deepen.  
agaperesonance keeps only the patterns that survive mutual reinforcement.

The combination is a research instrument, not a chatbot.

## Origin

Built by Jesse Ray (OpenRoot), Sikeston, Missouri.  
Concrete by day. Thermodynamic ledgers and fractal lattices by night.  
Permaculture ethics applied to computation: observe, catch & store energy, produce no waste, use edges, value the marginal.

## License

Code: GPL-3.0  
Docs: CC-BY-SA 4.0  
No patents. Ever. Defensive publication.
