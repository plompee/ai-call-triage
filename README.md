# AI Call Triage

Interactive demo of an AI call-routing system — a recreation of the triage pipeline I helped build at **Apex27** (real estate, remote).

Play a preset caller — meeting request, callback, telemarketing, debt collection — or type your own line, and watch the engine:

- "transcribe" the call (live ASR typing effect)
- match the utterance against weighted intent patterns
- score the three intents: **meeting / notification / spam**
- route the call: book a meeting, forward a notification, or flag & end

The scoring is transparent and deterministic — the whole "model" runs in the reasoning log on screen. No backend, no libraries: plain HTML, CSS and JavaScript in one file.

## Run it

Open `index.html` in a browser, or:

```
python3 -m http.server 8000
```

## Live demo

https://plompee.github.io/projects/call-triage.html
