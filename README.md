# capstone
# Pokémon Gen-III Battle Advisor

> Decision-support tool for Pokémon Emerald: live/read-only battle state → damage/KO odds → best move + “why,” with emulator companion bridge.

## About
A desktop advisor for Gen-III battles. It calculates expected damage, KO probabilities, and trade-offs for every legal move, then explains the top pick. Works offline from saved scenarios or live via a **read-only** bridge running alongside an emulator (Lua or OCR).

> Notes: Designed for educational/research use. No game assets are distributed. The live bridge is read-only and intended to work with personal backups you legally own.

## Key Features
- Deterministic Gen-III damage calc with correct rounding
- Best-move recommendation with a human-readable “why”
- Live read-only bridge (Lua) or OCR fallback
- Scenario loader/replayer for unit tests and demos


# Minecraft Human-Like Automation (External)
## About
A companion app that sits **beside** the vanilla Java client. It samples world/state via screen capture + OCR (incl. F3 overlay), client log tailing (`latest.log`), and an optional **map/tool feed** (JSON). It executes modular routines (e.g., fishing, farming) through OS-level input with realistic timing and micro-movement.  
*This is not a mod and does not patch the game binary.*

> Note: Use in accordance with your server’s rules.
> ## Key Features
**Reusable FSM framework** for scriptable routines
**Humanizer**: jittered timings, head sweeps, idle breaks
**Pluggable inputs**: OCR, logs, optional map/tool JSON feed
**Profiles & configs** per routine
**Dry-run** / visualize mode for debugging
