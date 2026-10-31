# Network analysis

The inspected HTML includes references to:

- WebSocket communication.
- `RTCPeerConnection` (WebRTC browser API).
- tRPC-style `httpBatchLink` implementation commentary.

## Open questions

- Which connections are active in current production?
- Which endpoints are public and which require authorization?
- Is peer-to-peer traffic used for gameplay, signaling, or neither?
- What data is exchanged during a match?