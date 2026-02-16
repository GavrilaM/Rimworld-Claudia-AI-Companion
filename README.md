# Claudia - AI Companion for RimWorld
<img width="1024" height="559" alt="Preview" src="https://github.com/user-attachments/assets/86bc44e2-40d3-4b41-a761-5d83c5b16552" />

An intelligent AI companion that watches your colony in real-time, provides strategic advice, reacts to events, and chats with you like a friend.

![RimWorld 1.5](https://img.shields.io/badge/RimWorld-1.5-blue)
![OpenRouter](https://img.shields.io/badge/AI-OpenRouter-orange)
![License: MIT](https://img.shields.io/badge/License-MIT-green)

---

## Features

### Deep Colony Analysis
(WARNING: May not be 100% accurate, depends on the AI model you use and consumes a lot of tokens, more polishing in future updates.)
## Colony Data Claudia Can Read
- Colonist profiles: names, backstory, traits, skills, health conditions, equipment, apparel, weapons
- Colony identity: faction type (tribal/crashlanded/etc.), tech level
- Resources: food, meals, medicine, silver, steel, components, etc.
- Storage contents: full inventory scan of all stockpiles
- Weather: current conditions, outdoor temperature
- Season and time
- Threats: hostile pawns on map, active combat
- Battle log: recent combat damage, kills, injuries
- Research progress: current and completed projects
- Population: free colonists, prisoners count
- Relationships between colonists
- Active modlist currently loaded in the game

### Proactive AI Companion
- Claudia chats randomly every few in-game hours, commenting on weather, mood, seasons, and individual colonists
- Reacts to events such as raids, mental breaks, fires, colonist deaths, and research completion
- Full conversation memory with no context limit
- Powered by OpenRouter, supporting any AI model (Gemini, Claude, GPT, Llama, and more)

### Unique Personality Tones

| Personality | Description |
|---|---|
| Sarcastic | Backseat gamer that roasts your decisions with internet slang |
| Professional | Military commander delivering tactical briefings with zero fluff |
| Friendly | Wholesome companion emotionally invested in every colonist |
| Custom | Define your own system prompt |

### Mood-Reactive Avatar

Claudia's portrait changes expression depending on the context of her message.

| Mood | Triggers | Accent Color |
|---|---|---|
| Idle | Default state | Blue |
| Happy | Success, harvest, research | Green |
| Alert | Raids, threats, combat | Red |
| Amused | Sarcastic or funny moments | Purple |
| Worried | Starvation, sickness, death | Amber |

### In-Game UI
- Large floating message overlay with mood-reactive avatar portrait
- Chat window accessible from the bottom menu bar
- Click-to-dismiss messages
- Mood-colored accent bars and borders

### Configuration
- Accessible via Options > Mod Settings > Claudia AI Companion
- API key and model selection (no code editing required)
- AI parameters: temperature, max tokens
- Adjustable chat frequency, message duration, chat history limit
- Built-in API connection test with error diagnostics
- Toggle random chat and floating overlay independently

---

## Installation

### Requirements
- RimWorld 1.5 or later
- Harmony mod ([GitHub](https://github.com/pardeike/HarmonyRimWorld) | [Steam Workshop](steam://url/CommunityFilePage/2009463077))
- Internet connection (for API calls)

### Steps

1. Download or clone this repository.

2. Copy the `Claudia_AI` folder into your RimWorld Mods directory:
   ```
   [RimWorld Install]/Mods/Claudia_AI/
   ```

3. Launch RimWorld and enable "Claudia - AI Companion" in the mod list.
   Make sure Harmony is loaded above Claudia in the mod order.

4. Configure the mod in-game:
   - Go to Options > Mod Settings > Claudia AI Companion
   - Get an API key from https://openrouter.ai/keys
   - Paste your API key and choose a model ID (e.g. `google/gemini-2.0-flash-001`)
   - Click "Test API Connection" to verify

---

## Mod Structure

```
Claudia_AI/
├── About/
│   ├── About.xml
│   └── Preview.png
├── Assemblies/
│   └── RimAI_Core.dll
├── Defs/
│   └── RimAI_MainTabDef.xml
└── Textures/
    └── RimAI/
        ├── ClaudiaAvatar.png
        ├── ClaudiaAvatar_Happy.png
        ├── ClaudiaAvatar_Alert.png
        ├── ClaudiaAvatar_Amused.png
        └── ClaudiaAvatar_Worried.png
```

---

## Compatibility

- Compatible with all other mods. Claudia only reads colony data and does not modify game mechanics.
- No known mod conflicts.
- Safe to add or remove mid-save.

---
## In-game Preview
<img width="600" height="600" alt="Screenshot 2026-02-15 210108" src="https://github.com/user-attachments/assets/86750bcf-7c7d-4d2e-b1dc-dd31864f4522" />
<img width="600" height="600" alt="Screenshot 2026-02-15 210137" src="https://github.com/user-attachments/assets/9c43652e-eae8-4d16-b863-a01f38c9566c" />
<img width="600" height="600" alt="Screenshot 2026-02-15 210144" src="https://github.com/user-attachments/assets/2b6cfaf7-335a-4d75-addc-745b8b7c8022" />
<img width="600" height="600" alt="Screenshot 2026-02-15 210305" src="https://github.com/user-attachments/assets/689d4e4c-8726-4528-8bdb-4172cf019fb2" />

## License

MIT License. Feel free to modify and share.

## Author

Gavrila M - [GitHub](https://github.com/GavrilaM)

