# Agentic Cowork Workshop – Cheatsheet

Statický web s praktickými podklady pro účastníky workshopu **Přeskočte copy-paste. Pracujte s AI v symbióze** (Tempo Akademie, kurz „Agentic Cowork").

## Stránky

- [`index.html`](index.html) – Cheatsheet: terminál + Claude Code (základy)
- [`hranice.html`](hranice.html) – Hranice agenta (kam vidí, co musí odsouhlasit)
- [`varianty.html`](varianty.html) – Sedm cest k agentovi (různá UI / prostředí)

## Deploy

Deploy přes [Netlify](https://www.netlify.com) na web **[hyw-cheatsheet.netlify.app](https://hyw-cheatsheet.netlify.app)** (site ID je v `.netlify/state.json`, committed).

Web **není** napojený na GitHub CI — push do `main` automaticky nedeployuje. Deploy je nutné spustit ručně:

```bash
# Lokální preview
npx serve .

# Manuální deploy do produkce
netlify deploy --prod --dir .
```

## Struktura

```
.
├── index.html           # Cheatsheet (Terminál + Claude)
├── hranice.html         # Hranice agenta
├── varianty.html        # Sedm cest k agentovi
├── cheatsheet.css       # Styles
├── netlify.toml         # Netlify config (publish = root)
└── .netlify/state.json  # Site link (siteId)
```

## Historie

Web vznikl v projektu HYW 2026 (workshop 28. 4. 2026, Brno) a byl extrahován do samostatného repa, aby mohl pokračovat napříč dalšími běhy kurzu (Praha 22. 5. 2026 a dál).
