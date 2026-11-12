# waBot — bot WhatsApp per chat di gruppo

Bot WhatsApp in **Node.js** basato su [WPPConnect](https://github.com/wppconnect-team/wppconnect), con comandi per i gruppi e integrazione **OpenAI** per la generazione di immagini.

## Funzionalità

- `!ping` — verifica che il bot sia attivo
- `!help` — elenco dei comandi
- `!everyone` — menziona tutti i membri del gruppo
- Versetti casuali da `versetti.json`
- Generazione immagini con OpenAI (`gpt-image-1`)
- Keep-alive periodico verso il proprietario del bot

## File

| File | Contenuto |
|---|---|
| `wbFinal.js` | Versione attuale del bot |
| `wb.js`, `wb2.js` | Versioni precedenti |
| `versetti.json` | Dataset dei versetti |

## Avvio

```bash
npm install @wppconnect-team/wppconnect winston axios openai sharp
node wbFinal.js
```

Al primo avvio scansiona il QR code con WhatsApp. Imposta `BOT_ID`, `OWNER_ID` e la chiave OpenAI (`OPENAI_API_KEY`) prima di partire.
