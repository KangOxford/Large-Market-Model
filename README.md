# Large Market Model

An English research website on dual-encoder action generation, deterministic state updates, and state completeness in order-book replay.

The page adapts `orderbook_state_closure_dual_encoder.md` into an academic project-page layout inspired by [Evolution Strategies at the Hyperscale](https://eshyperscale.github.io/). The layout is implemented independently; all supplied diagrams are preserved without modification.

## Local preview

```bash
python3 -m http.server 8000
```

Open http://localhost:8000. No build step or package installation is needed. MathJax 3.2.2 loads from jsDelivr to render equations; an internet connection is required for mathematical typesetting.

## Files

- `index.html`: English article and figure captions.
- `style.css`: responsive layout; two architecture panels on desktop, stacked on mobile.
- `math-config.js`: mathematical typesetting configuration.
- `assets/`: original figures, combined full-resolution figure, and favicon.

## GitHub Pages

Publish the `main` branch, `/ (root)`, in **Settings → Pages → Deploy from a branch**. The expected project URL is https://kangoxford.github.io/Large-Market-Model/ once Pages is enabled and its deployment completes.

## Scope

The single-step `(action, observation)` input is the design presented in the source note. This website does not claim to validate an implementation's data loader or cache. It distinguishes complete subsequent actions from a complete initial state: the former cannot generally recover missing initial information.
