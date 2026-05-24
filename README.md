# Negotiation Table

A turn-based negotiation game. You negotiate against an LLM counterparty in scripted scenarios, table a final offer or walk away, then receive an LLM coach verdict.

**Play it live:** [valykay.github.io/negotiation-table-app](https://valykay.github.io/negotiation-table-app/)

## Running locally

Any static file server will do, for example:

```sh
npx serve .
```

Then open the printed URL in a browser.

## Bring your own key

The app calls Anthropic, OpenAI, or Google Gemini directly from the browser. You supply your own API key via the Settings page. Keys are stored in `sessionStorage` by default (cleared when the tab closes) and can optionally be persisted to `localStorage` per provider.

Direct browser calls expose your key to any code running in the page. Use a key with spending limits and treat it accordingly.

## License

MIT. See [LICENSE](LICENSE).
