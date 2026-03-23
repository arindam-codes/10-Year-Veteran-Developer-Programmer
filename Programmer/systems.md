
---

## 📦 Systems Overview

| # | System Name | Module Name | Description | Key Features |
|--|--|--|--|--|
| 1 | Player Data System | PlayerDataService | Stores all player data | Coins, levels, inventory, attributes |
| 2 | Data Persistence | DataPersistenceSystem | Saves/loads data | Auto-save, retry, error handling |
| 3 | Leaderboard System | LeaderboardService | Displays player stats | leaderstats, real-time updates |
| 4 | Global Leaderboard | GlobalLeaderboardService | Top players globally | OrderedDataStore, rankings |
| 5 | Currency System | CurrencyService | Manages currencies | Add/remove, validation |
| 6 | Upgrade System | UpgradeService | Handles upgrades | Scaling costs, multipliers |
| 7 | Rebirth System | RebirthSystem | Prestige mechanic | Reset + permanent boosts |
| 8 | Shop System | ShopService | In-game purchases | Item buying, validation |
| 9 | Gamepass System | GamepassService | Robux purchases | Gamepass checks, dev products |
| 10 | Inventory System | InventorySystem | Stores items | Equip/unequip, storage |
| 11 | Pet System | PetService | Pet mechanics | Multipliers, rarity |
| 12 | Loot / RNG System | LootService | Random rewards | Probability tables |
| 13 | Quest System | QuestService | Tracks tasks | Progress + rewards |
| 14 | Daily Reward System | DailyRewardService | Login rewards | Streaks, scaling rewards |
| 15 | Trading System | TradingService | Player trading | Secure exchange system |
| 16 | Round System | RoundManager | Game loop | Lobby → Game → End |
| 17 | Combat System | CombatService | Damage system | Health, hit detection |
| 18 | Anti-Exploit | SecurityService | Prevent exploits | Remote validation |
| 19 | World System | WorldManager | Multi-world support | Teleport + progression |
| 20 | UI Framework | UIFramework | UI handling | Notifications, menus |

---

## 📁 Project Structure

| Folder | Contents |
|--|--|
| ReplicatedStorage/Modules | All reusable systems |
| ServerScriptService | Server-side systems (data, security, leaderboard) |

---

## ⚙️ Example Usage

```lua
local CurrencyService = require(game.ReplicatedStorage.Modules.CurrencyService)

CurrencyService:Add(player, "Coins", 100)
