![X-Prison Header](https://i.imgur.com/VpYT0KA.png)
# X-Prison Armors
![Discord](https://img.shields.io/discord/1387881708581290257?label=Discord&logo=Discord)

**X-Prison Armors** gives every player one armor set that **levels up by mining**. The set starts as a grey leather **Common** set, earns armor XP for every raw block the player breaks, and climbs a configurable ladder of tiers — leather, chainmail, iron, gold, diamond, netherite — up to **Insanity**. Every level grows its boosts to money, tokens, gems, pickaxe XP and enchant proc chance; finishing a tier transforms the four pieces in place into the next tier's armor. Permission-based **skins** change how a set looks and speed up its progression.

It is an add-on for [X-Prison](https://github.com/Drawethree/X-Prison) — every boost hooks into X-Prison's public API, and the [Events addon](https://github.com/Drawethree/X-Prison/wiki/Events)'s **Armor Training** event doubles armor XP.

## 💎 Get X-Prison Armors

**X-Prison Armors is a premium paid resource.** You can purchase it here:

### 👉 [**Buy X-Prison Armors on BuiltByBit**](https://builtbybit.com/resources/x-armors-armor-progression-system.84696/) 👈

We also offer **a lot more for prison servers** — the core, addons, setups and premium extras — at our [**Prison Store**](https://builtbybit.com/store/prison-store.392/), with **amazing bundle discounts**. Need a custom bundle? Open a ticket on [Discord](https://discord.gg/ZeSkmEC6mG).

> **What's New in 2.0.0** — the permission multiplier of 1.x is now a **progression**: seven bundled tiers × ten levels, ~5,000,000 blocks to a fully upgraded Insanity set that boosts everything 3×, soulbound sets locked into the armor slots, the old permission tiers reborn as [skins](https://github.com/Drawethree/X-Prison-Armors/wiki/Skins), new menus, level-up effects, placeholders and a developer API. [See the Changelog](https://github.com/Drawethree/X-Prison-Armors/wiki/Changelog)

---

## Getting Started

| Step | Page |
|------|------|
| 1. Install | [Setup](https://github.com/Drawethree/X-Prison-Armors/wiki/Setup) |
| 2. Understand the ladder | [Armor Progression](https://github.com/Drawethree/X-Prison-Armors/wiki/Armor-Progression) |
| 3. Tune the numbers | [armors.yml](https://github.com/Drawethree/X-Prison-Armors/wiki/armors.yml) |
| 4. Sell skins | [Skins](https://github.com/Drawethree/X-Prison-Armors/wiki/Skins) |
| 5. Learn the commands | [Commands & Permissions](https://github.com/Drawethree/X-Prison-Armors/wiki/Commands-&-Permissions) |

---

## Requirements

| Requirement | Notes |
|---|---|
| Java 17+ | Required |
| Paper or Spigot 1.14+ | All text is MiniMessage; Spigot downsamples to classic colour codes |
| [X-Prison](https://github.com/Drawethree/X-Prison) 2026.3.8.7+ | Required |
| [helper](https://ci.lucko.me/job/helper/lastSuccessfulBuild/artifact/helper/target/helper.jar) | Required |
| PlaceholderAPI | Optional — `%xprisonarmors_*%` placeholders |
| NBTAPI | Optional — only to convert armor items from 1.x |
| X-Prison Events 1.0.3+ | Optional — the Armor Training event |

---

## Highlights

- **One set that levels as a whole** — tier, level, XP and skin live on the four pieces; no database. Maxing a tier converts the whole set in place.
- **Boosts that grow every level** — currency (any X-Prison currency), pickaxe XP and enchant proc chance, from +1 % at Common Lv 1 to +200 % at Insanity Lv 10 out of the box.
- **Soulbound and locked in** — no dropping, storing, trading or unequipping by default; kept on death. Three independent switches.
- **Skins** — look override per piece, armor-XP multiplier, optional extra boosts, unlocked by permission. The four bundled skins keep the 1.x permission nodes.
- **Menus** — `/armors` tier ladder and `/armors skins` picker, every slot and line in `gui.yml`.
- **Feedback** — level-up, tier-up and max-level messages, titles, sounds, action bar, broadcasts and particles, each its own toggle.
- **Zero item writes on the block-break path** — XP is banked and flushed every five seconds.
- **89 automated tests.**

---

# Pages
### General
* [Home](https://github.com/Drawethree/X-Prison-Armors/wiki)
* [Features](https://github.com/Drawethree/X-Prison-Armors/wiki/Features)
* [Setup](https://github.com/Drawethree/X-Prison-Armors/wiki/Setup)
* [Commands & Permissions](https://github.com/Drawethree/X-Prison-Armors/wiki/Commands-&-Permissions)
* [Placeholders](https://github.com/Drawethree/X-Prison-Armors/wiki/Placeholders)
* [FAQ & Troubleshooting](https://github.com/Drawethree/X-Prison-Armors/wiki/Frequently-Asked-Questions---Troubleshooting)
* [Changelog](https://github.com/Drawethree/X-Prison-Armors/wiki/Changelog)

### Guides
* [Armor Progression](https://github.com/Drawethree/X-Prison-Armors/wiki/Armor-Progression)
* [Skins](https://github.com/Drawethree/X-Prison-Armors/wiki/Skins)
* [Menus](https://github.com/Drawethree/X-Prison-Armors/wiki/Menus)
* [Level-Up Effects](https://github.com/Drawethree/X-Prison-Armors/wiki/Level-Up-Effects)
* [Events Integration](https://github.com/Drawethree/X-Prison-Armors/wiki/Events-Integration)
* [Developer API](https://github.com/Drawethree/X-Prison-Armors/wiki/Developer-API)
* [Upgrading from 1.x](https://github.com/Drawethree/X-Prison-Armors/wiki/Upgrading-from-1.x)

### Default Configs
* [_config.yml_](https://github.com/Drawethree/X-Prison-Armors/wiki/config.yml)
* [_armors.yml_](https://github.com/Drawethree/X-Prison-Armors/wiki/armors.yml)
* [_skins.yml_](https://github.com/Drawethree/X-Prison-Armors/wiki/skins.yml)
* [_gui.yml_](https://github.com/Drawethree/X-Prison-Armors/wiki/gui.yml)
* [_messages.yml_](https://github.com/Drawethree/X-Prison-Armors/wiki/messages.yml)

---

## Commands

| Command | Permission | Description |
|---|---|---|
| `/armors` | `xprisonarmors.use` | Opens the tier ladder (aliases `/armor`, `/xarmors`) |
| `/armors skins` | `xprisonarmors.use` | Opens the skin picker |
| `/armors claim` | `xprisonarmors.use` | Returns missing pieces of your set |
| `/armorsadmin give <player> <tier> [level] [piece]` | `xprisonarmors.admin` | Gives a set or one piece |
| `/armorsadmin set <player> <tier> [level]` | `xprisonarmors.admin` | Sets the worn set's tier and level |
| `/armorsadmin addxp <player> <amount>` | `xprisonarmors.admin` | Adds armor XP |
| `/armorsadmin skin <player> <skin\|none>` | `xprisonarmors.admin` | Applies a skin |
| `/armorsadmin info <player>` | `xprisonarmors.admin` | Shows a player's armor |
| `/armorsadmin reload` | `xprisonarmors.admin` | Reloads every config |

Full reference: [Commands & Permissions](https://github.com/Drawethree/X-Prison-Armors/wiki/Commands-&-Permissions) · [Placeholders](https://github.com/Drawethree/X-Prison-Armors/wiki/Placeholders)

---

## For Developers

```java
XPrisonArmorsAPI api = XPrisonArmorsAPI.get();
Optional<ArmorSetState> state = api.getSetState(player);   // tier, level, xp, skin
SetBoosts boosts = api.getBoosts(player);                   // percent per currency, pickaxe XP, enchant proc
```

Events: `ArmorLevelUpEvent`, `ArmorTierUpEvent`, `ArmorSkinApplyEvent` (cancellable). Every XP gain also fires X-Prison's `PlayerProgressionXpGainEvent` with the key `xprisonarmors:armor`, so any plugin can boost or block armor XP without depending on this one. See the [Developer API](https://github.com/Drawethree/X-Prison-Armors/wiki/Developer-API).

---

### Support
* [Discord](https://discord.gg/ZeSkmEC6mG)
* [X-Prison wiki](https://github.com/Drawethree/X-Prison/wiki)
