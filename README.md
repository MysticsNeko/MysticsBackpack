# 🎒 MysticsBackpack – Mystical Backpack for Your Server
MysticsBackpack is an advanced, fully secure plugin for Minecraft (Paper/Spigot 1.21+) that allows players to store items in additional, magical backpacks. Designed with server economy, duplication security, and administrative convenience in mind.

## ✨ Key Features
Multi-level capacity: Players receive a default small backpack (9 slots). Larger sizes (18 and 27 slots) are unlocked via permissions.
Complete security (Anti-Duplication): Eliminates the risk of item duplication, even in the event of a player's sudden death, logout, or server crash.
Advanced administration: Administrators can view and edit any player's backpacks (both online and offline), making it easier to combat cheaters (e.g., removing items from a player who used X-ray).
Full logging (Audit Logs): Every administrative action is logged in the audit_log.txt file with the date and time, ensuring full transparency and verifiability of admin actions.

Support for version 1.21+: Optimized for the latest Paper/Spigot versions, using native item serialization methods (serializeAsBytes / deserializeBytes).

Lightweight and efficient: No external dependencies (except for the Paper API), data saved in YAML files, minimal server load.

## 🛠️ Features

**For Players**
Command: /mysticpack: Opens a custom backpack.

Dynamic size: Backpack size adjusts to your permissions (Small 9, Medium 18, Large 27).

Autosave: Items are safely saved after closing the backpack or logging out.

Clear interface: Aesthetically pleasing GUI with colorful titles indicating backpack size.

**For Administrators**

Command: /mysticpackadmin <player>: View another player's backpack (read-only).

Command: /mysticpackadmin <player> edit: Edit another player's backpack (allows removing and adding items).

Offline Support: Allows editing the backpacks of players who are not currently online (e.g., after detecting cheats in the logs).

Audit Logs: Automatically records every admin action in the audit_log.txt file in the following format: [DATE TIME] Admin 'Nickname' performed the action 'ACTION' on player 'Target' (Status: ONLINE/OFFLINE).

## ⚙️ Configuration and Permissions

**Permissions**

Permission -- Description -- Default

mysticsbackpack.use -- Allows you to open your own backpack. -- true (everyone)

mysticsbackpack.medium -- Unlocks a medium backpack (18 slots). -- op

mysticsbackpack.large -- Unlocks a large backpack (27 slots). -- op

mysticsbackpack.admin -- Allows you to view and edit other players' backpacks. -- op

**Commands**

Command -- Description -- Permission

/mysticpack -- Opens your backpack. -- mysticsbackpack.use

/mysticpackadmin <player> -- View the player's backpack. -- mysticsbackpack.admin

/mysticpackadmin <player> edit -- Edit the player's backpack. -- mysticsbackpack.admin

## 🚀 Requirements
Server: PaperMC or Spigot 1.21 or later.
Java: Version 21 or later.
Dependencies: None (Plugin is self-contained).

## 💡 Why MysticsBackpack?
Unlike other plugins, MysticsBackpack emphasizes data security and transparent administration. Thanks to its logging system and anti-duplication protection, it is ideal for survival, RPG, and economy servers where item integrity is crucial.
