## Day 1 (Monday) — HTTP Re-examined

### Concept Questions
1. HTTP request-response model **kyun** dominate karta hai? Aur konse cases mein *galat fit* hai?
2. Stateless protocol ka asli matlab kya hai? State manage kahan ho?
3. HTTP/1.1 vs HTTP/2 vs HTTP/3 — har version ne kya problem solve ki?

### Reading (45 min)
- "Why HTTP is the way it is" — search Hussein Nasser ka video
- High Performance Browser Networking — Chapter 9 (free online)

### Case Study (30 min)
- **WhatsApp** kyun WebSocket pe chala, HTTP polling pe nahi?
- **Instagram feed** — HTTP polling, long polling, ya WebSocket? Kyun?

### What Breaks Here? (30 min)
- HTTP request middle mein fail ho jaye to client ko kaise pata chale?
- Idempotency kyun HTTP design ka core hai? Kis method mein zaroori, kis mein nahi?

### Self-Quiz
1. POST aur PUT mein asli difference kya hai? (Hint: idempotency)
2. 502 aur 504 mein farak kya hai? Production debugging mein kab kaunsa milega?
3. CORS ka asli purpose kya hai? (Hint: security, not convenience)
4. Why is HTTP/2 multiplexing important?
5. Server-Sent Events vs WebSocket — trade-offs?