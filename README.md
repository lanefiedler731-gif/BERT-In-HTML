# BERT Studio

Single-file web app for masked language modeling in the browser. It uses Transformers.js via CDN to run BERT/RoBERTa-style fill-mask models and renders a chat-like UI with model selection and tuning controls.

## Features
- Multiple models: BERT, DistilBERT, RoBERTa, multilingual, and large ONNX options.
- Fill-mask with `_`, `[MASK]`, or `<mask>` tokens.
- Top-K, confidence threshold, and temperature controls.
- Minimal, mask, and assistant modes with streaming responses.
- Optional confidence bars, probabilities, and filled sentence previews.

## Run
1. Open `bert-studio.html` in a modern browser.
2. Enter text with mask tokens (example: `Paris is the _ of France.`).
3. Select a model and click Run.

Note: The app loads models over the network from the Transformers.js CDN, so an internet connection is required on first use, other uses of same model will not require networking.

## File Layout
- `bert-studio.html` - UI, styles, and app logic in one file.

## Tech
- HTML/CSS/JS (no build step)
- `@xenova/transformers` via CDN
