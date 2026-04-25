# Canals and Straits

[![Victoria 3 Version](https://img.shields.io/badge/Victoria%203-1.12.*-blue)](https://store.steampowered.com/app/529340/Victoria_3/)
[![Mod Version](https://img.shields.io/badge/Version-1.0.0-green)](./.metadata/metadata.json)
[![License](https://img.shields.io/badge/License-MIT-yellow.svg)](./LICENSE)
[![Multiplayer](https://img.shields.io/badge/Multiplayer-Compatible-success)](./.metadata/metadata.json)
[![Languages](https://img.shields.io/badge/Languages-EN%20%7C%20ES-purple)]()

> **A complete overhaul of maritime chokepoints: toll canals, blockable straits, and naval geopolitics.**

Transform Victoria 3's canals and straits into true instruments of economic and diplomatic power. Manage your canals, collect tolls, deny passage to rival powers, and project naval influence over the world's most important sea lanes.

---

## Table of Contents

- [Features](#features)
- [Canals](#canals)
- [Straits](#straits)
- [Diplomacy and War](#diplomacy-and-war)
- [Economic Engine](#economic-engine)
- [Requirements](#requirements)
- [Installation](#installation)
- [Compatibility](#compatibility)
- [Screenshots](#screenshots)
- [Roadmap](#roadmap)
- [Credits and License](#credits-and-license)

---

## Features

| System | Description |
|--------|-------------|
| **3 Playable Canals** | Suez, Panama, and Kiel with independent ownership and operation models. |
| **4 Passive Straits** | Gibraltar, Bosphorus, Malacca, and Hormuz with automatic geopolitical control. |
| **Canal Diplomacy** | Selective blockades, toll exemptions, and diplomatic plays to force canal opening. |
| **Economic Engine** | Tolls calculated from the combined GDP of Great Powers and Major Powers. |
| **Land Purchases** | Acquire Port Said, Colon, and Kiel to consolidate control over each canal. |
| **Multiplayer** | Fully synchronized for multiplayer sessions. |

---

## Canals

Each canal can be configured with two independent production method groups:

### Canal Ownership

- **Privately Owned Canal**: Commercial management. Capitalists and technical staff run operations. 30% of profits go to the state treasury; 70% is reinvested locally as a construction boom.
- **Government Run Canal**: Direct state administration. Engineers and bureaucrats manage the canal. 100% of profits go to the treasury.

### Canal Operation

| Mode | Effect |
|------|--------|
| **Free Transit** | No direct toll income, but improves prestige and commercial efficiency in the canal state. |
| **Moderate Tolls** | All traffic pays a moderate fee. Balanced option between revenue and administrative costs. |
| **Tolls Except Allies** | Subjects and power bloc partners get free passage; everyone else pays. Higher profit but harder to manage. |
| **Maximum Revenue Tolls** | Squeeze as much revenue as possible. Higher income but also higher oversight costs. |
| **Total Blockade** | Canal closed to foreign passage. Revenue collapses, naval enforcement costs rise, and +15 Infamy is gained. |

### Key Land Purchases

You can acquire strategic territories through special decisions to consolidate full control over a canal:

- **Port Said** → Full control of the Suez Canal.
- **Colon** → Full control of the Panama Canal.
- **Kiel** → Full control of the Kiel Canal.

Each purchase grants temporary minting modifiers and unlocks additional strategic options.

---

## Straits

The strait system is **100% passive**: no buttons, no manual decisions, no active policies required. Control is checked automatically every month.

### How It Works

- **One-shore control**: Grants trade advantage (`state_trade_advantage_mult`) and convoy capacity (`country_convoys_capacity_mult`).
- **Both-shore control**: Doubles the bonuses, plus prestige (`country_prestige_add`) and diplomatic influence (`country_influence_mult`).

### Implemented Straits

| Strait | Key Shores | Both-Shore Bonus |
|--------|-----------|------------------|
| **Gibraltar** | Iberia / Morocco | +10% trade advantage, +5% convoys, +15 prestige, +5% influence |
| **Bosphorus** | Anatolia / Balkans | +12% trade advantage, +5% convoys, +15 prestige, +5% influence |
| **Malacca** | Malaysia / Sumatra | +14% trade advantage, +5% convoys, +15 prestige, +5% influence |
| **Hormuz** | Persia / Arabia | +16% trade advantage, +5% convoys, +15 prestige, +5% influence |

> *Tip: Controlling both shores of a strait is one of the strongest commercial and naval power multipliers in the game.*

---

## Diplomacy and War

### Diplomatic Actions

- **`Canal Access Blockade`**: The canal owner can selectively block passage for a target country. Requires diplomatic relevance (shared regions, interest markers, or relations). Adds extra bureaucracy cost.
- **`Canal Toll Exemption`**: A treaty article available in the treaty drafting panel. Grants free passage to an ally bilaterally.

### Diplomatic Plays and War

- **`Force Open Canal`**: Any country with aggressive diplomatic plays permitted can demand the opening of a blocked canal. No Great Power rank required.
- **War Goal**: Upon enforcing forced opening, the loser receives the `Canal Forced Open` modifier for 1800 days (-3000 minting, -10 prestige).

---

## Economic Engine

Canal profits are calculated monthly based on global GDP:

```
Profit = Base Fee (500) × (GP_GDP + MP_GDP) / 10,000,000
```

- The GDP of all **Great Powers** and **Major Powers** worldwide is summed.
- The base fee automatically scales with the size of the global economy.
- **Private ownership**: 30% to treasury + local construction boom.
- **State ownership**: 100% to treasury.

---

## Requirements

- **Victoria 3** version `1.12.*` or compatible.
- **Community Mod Framework (CMF)** — mandatory dependency. Subscribe to CMF on the Steam Workshop first.

---

## Installation

### Steam Workshop (Recommended)

1. Subscribe to **[Community Mod Framework](https://steamcommunity.com)** on the Steam Workshop.
2. Subscribe to **Canals and Straits**.
3. Enable both mods in the Victoria 3 launcher.
4. Enjoy!

### Manual Installation

1. Download and extract this mod into:
   ```
   C:\Users\<username>\Documents\Paradox Interactive\Victoria 3\mod\
   ```
2. Download and install the dependency **[Community Mod Framework](https://github.com/Victoria-3-Modding-Co-op/Community-Mod-Framework)** following its instructions.
3. Enable the mod in the launcher.

---

## Compatibility

| Aspect | Status |
|--------|--------|
| **Multiplayer** | Compatible and synchronized |
| **Achievements** | No (mods disable Ironman achievements) |
| **Replaced Files** | `common/buildings/10_canals.txt`, `common/journal_entries/00_canals.txt`, `common/company_types/00_companies_africa.txt`, `common/company_types/00_companies_americas.txt` |
| **Known Conflicts** | Mods that alter the same replaced files or vanilla canals/straits |

> To report incompatibilities or bugs, open an issue on the repository or leave a comment on the Steam Workshop page.

---

## Screenshots

<!-- Replace the placeholder image links below with your actual Steam Workshop screenshot URLs once uploaded -->

| | |
|:--:|:--:|
| ![Suez Canal PM Panel](https://via.placeholder.com/400x225?text=Suez+Canal+PM+Panel) | ![Gibraltar Strait Control](https://via.placeholder.com/400x225?text=Gibraltar+Strait+Control) |
| *Suez Canal production methods* | *Passive control of the Strait of Gibraltar* |
| | |
| ![Canal Access Blockade](https://via.placeholder.com/400x225?text=Canal+Access+Blockade) | ![Private Investment Boom](https://via.placeholder.com/400x225?text=Private+Investment+Boom) |
| *Diplomatic action: Canal Access Blockade* | *Private ownership reinvesting locally in Panama* |

> **Note for the author**: Upload 4-5 screenshots to the Steam Workshop showing: (1) the PM panel of a canal, (2) the map with strait control, (3) the diplomatic blockade action, (4) the treaty drafting panel with toll exemption, and (5) a before/after of canal economic profits.

---

## Roadmap

- [x] Core canal system with ownership and operation PMs
- [x] GDP-scaled economic engine
- [x] Passive system for 4 geopolitical straits
- [x] Canal diplomacy (blockade, exemption, diplomatic play)
- [x] Full localization in English and Spanish
- [ ] French and German translation *(coming soon)*
- [ ] Additional flavor events for straits
- [ ] Additional canals (Corinth, Nicaragua, etc.) *(under consideration)*

---

## Credits and License

**Author**: Flussen  
**Contributors**: Victoria 3 Modding Community

This project is licensed under the **[MIT License](./LICENSE)**.

```
Copyright 2026 - Flussen

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the “Software”), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.
```

> **Disclaimer**: I am not responsible for constant updates. I started and manage the project, but it belongs to everyone. If you wish to contribute, you are welcome!

---

## Links

- [Steam Workshop](https://steamcommunity.com)
- [Community Mod Framework](https://github.com/Victoria-3-Modding-Co-op/Community-Mod-Framework)

---

<p align="center">
  <i>"Whoever controls the canals and straits controls the commerce of the world."</i>
</p>
