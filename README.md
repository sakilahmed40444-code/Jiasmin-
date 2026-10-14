# 🔥 LIA Web v1.0 — "Talk to it. Watch it build."

LIA build guide (`lia-build-guide`) ka Hopweb-ready **single-file web build**.
Ek hi `index.html` — Hopweb me kholo, APK banao, phone me chalao.

## Kya-kya hai (guide ke spec ke hisaab se)

| Spec step | Is build me |
|---|---|
| 02 State & storage | Naam, Gemini API key, model, theme — sab phone me (localStorage) |
| 03 10 Personalities | Normal, Friendly, Professional, Funny, Companion, GF Mode, Teacher, Developer, Hungry, Nautanki — beech baat me badal sakti ho |
| 03 Language detect | Hindi (Devanagari) / Hinglish / English auto-detect + fixed mode |
| 04–06 Voice | Continuous voice loop: bolo → suno → jawab → phir bolo (✕ tak). Mic mute button. |
| 07 Phone actions | "YouTube kholo", call ke liye dialer, WhatsApp/SMS **composer** (tum Send dabate ho — spec ke `play` flavor jaisa) |
| 08 Text chat | Gemini REST + offline Hinglish brain fallback |
| 09 Design system | Gehri indigo raat `#06050E` + marigold `#FFB547` accent, dark/light theme |
| 10 3D orb | Canvas orb — 7 styles (NOVA…ARCHER), state palettes, tilt-driven light, voice ripples, edge glow (violet=sun rahi, pink=bol rahi) |
| 11 Screens | Home, Voice, Forge, Chat, Personality, History, Settings, Permissions, About |
| 14 **Website Forge** | "Ek cafe ki website banao" bolo → 3D reactor scene (stages, progress, log cards, tok/s) → real Gemini SSE stream se website → sandboxed viewer → Share / Save / Browser / Edit / Rebuild / Meri websites |

## Chalane ke liye

1. Hopweb app me `index.html` kholo → APK banao. (Ya Chrome me seedha kholo.)
2. Pehli voice tap par **Microphone Allow** dabao.
3. (Optional) Settings → Gemini API key dalo — bina key ke offline dimaag chalta hai; Forge bina key ke built-in template se website banata hai.

## Imandaar note (kya nahi hoga)

- Real-time **Gemini Live full-duplex** voice is web build me nahi — Web Speech loop hai (ek baar me ek taraf). Yehi ek wajah se native Kotlin app alag hota.
- **Screen control / auto-tap / auto-send** nahi — web app dusre apps ke button nahi daba sakti. Messages hamesha composer kholti hain.
- Voice input ke liye internet chahiye (Google ka free STT), API key nahi.

## Files

- `index.html` — poori app (79 KB, sab inline)
- `../lia-web-v1.0.zip` — Hopweb ke liye ready zip
