# Liberty — The Desktop Eagle

**Freedom · Focus · Strength · Always Near**

Liberty is Fenton Lab's second companion, a separate product from Sprocket. She has her own identity, her own character and her own data. Where Sprocket is a curious, playful fox, Liberty is a focused desktop eagle, built to help you understand and improve what you're working on.

> **Status: early development.** Liberty is further from release than Sprocket. Her signature capabilities below are **planned, not built**. There is no download or release date.

## What exists today (development milestone 0.2)

**Verified in development:**
- Liberty runs as her own Windows desktop application. She doesn't use Sprocket's code, data or artwork, and doesn't need Sprocket installed.
- **Desktop window:**
  - a small, draggable, always-near window that doesn't steal keyboard focus, and lets clicks pass through the transparent parts of the image;
  - handling for multiple monitors and high-DPI displays. It passes automated tests but hasn't yet been tried on a physical multi-monitor setup.
- **Animation:** an animation system with eight states (perched idle, observe, alert, wing stretch, preen, takeoff, landing and rest), driven by a versioned animation manifest. For now it shows placeholder graphics.
- **Artwork checks:** a strict pipeline that loads production artwork only when it passes format checks and an owner-approved provenance record.
- **Local storage:** her own settings and database on the user's computer.
- **Tests:** 15 automated tests pass, plus Windows acceptance checks (internal development evidence, not certification).

**Not finished:**
- AI chat;
- screen research;
- the final eagle artwork and complete animations. The current builds use placeholder graphics while production eagle art goes through design and rights approval.

## Planned signature capability: Patriot Lens

Patriot Lens is the planned way to point Liberty at something on your screen and get help with exactly that. **None of the features below is available yet.**

| Planned action | What it would do |
| --- | --- |
| **Research This** | You deliberately select an area of your screen, and Liberty helps you research what's in it |
| **Explain This** | Explains the selected text, chart, message or interface in plain language |
| **Debug or Improve** | Suggests fixes or improvements for selected code, writing or settings. You decide what to apply |
| **Teach Me About This** | Turns the selection into a short, step-by-step lesson |
| **Continuity** | Follow-up questions keep the context of the conversation and the research, but only the context you've allowed |

## Planned boundaries

These are design commitments for Liberty, to be verified before any release:
- **Local first:** conversations, research history and settings stay on your computer by default.
- **Screen capture only with your consent:** Liberty sees only an area of the screen you deliberately select, each time. There is no background screen watching and no recording.
- **Her own memory:** Liberty's memory is separate from Sprocket's and from other applications. You can view and delete it.
- **No unauthorised access:** no file reading without your explicit choice, and no running programs or commands on your behalf.
- **Permissions you can see:** any context Liberty uses is shown to you and can be cleared.

## Relationship to Sprocket

Liberty follows the same principles as Sprocket and uses similar engineering patterns, but she is a **separate codebase today**. See [Fenton Lab's engineering approach](ENGINEERING_APPROACH.md).

Sprocket Desktop remains Fenton Lab's first release priority.
