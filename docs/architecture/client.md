# Client architecture

## Observed in supplied HTML

- Single large HTML document containing extensive inline CSS and JavaScript.
- HTML5 Canvas rendering and interactive HUD/lobby.
- Font assets referenced from relative `fontes/` paths.
- Portuguese UI strings and inline version annotations.
- Player profile, lobby, ranked mode, training, replay, store and HUD configuration features appear in source.

## Architectural boundaries

- **Browser/UI layer:** HTML, CSS, DOM and Canvas.
- **Game logic layer:** client-side JavaScript for input, rendering and local state.
- **Network layer:** client code references WebSocket, WebRTC and tRPC-style HTTP batching; the presence of references alone does not prove each path is active in production.
- **Backend:** implementation not present in supplied file.
