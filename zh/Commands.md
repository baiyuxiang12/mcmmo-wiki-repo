---
title: 命令
description: mcMMO commands
published: true
date: 2024-11-24T02:53:25.157Z
tags: commands
editor: markdown
dateCreated: 2024-11-24T01:51:14.196Z
---


<!-- 语言切换器开始 -->
<div class="language-switcher">
  <div class="language-switcher-current">
    <span class="current-language">English</span>
    <span class="dropdown-icon">▼</span>
  </div>
  <div class="language-switcher-dropdown">
        <div class="language-option active" data-lang="en">English</div>
    <div class="language-option " data-lang="zh">中文</div>
    <div class="language-option " data-lang="es">Español</div>
    <div class="language-option " data-lang="fr">Français</div>
    <div class="language-option " data-lang="de">Deutsch</div>
    <div class="language-option " data-lang="ru">Русский</div>
    <div class="language-option " data-lang="ja">日本語</div>
    <div class="language-option " data-lang="ko">한국어</div>

  </div>
</div>

<style>
.language-switcher {
  position: relative;
  display: inline-block;
  margin: 10px 0;
  font-family: Arial, sans-serif;
  z-index: 100;
}

.language-switcher-current {
  display: flex;
  align-items: center;
  cursor: pointer;
  padding: 8px 12px;
  background-color: #f5f5f5;
  border: 1px solid #ddd;
  border-radius: 4px;
}

.current-language {
  margin-right: 8px;
  font-weight: bold;
}

.dropdown-icon {
  font-size: 10px;
}

.language-switcher-dropdown {
  display: none;
  position: absolute;
  top: 100%;
  left: 0;
  background-color: white;
  border: 1px solid #ddd;
  border-radius: 4px;
  box-shadow: 0 2px 5px rgba(0,0,0,0.1);
  min-width: 150px;
  z-index: 101;
}

.language-switcher:hover .language-switcher-dropdown {
  display: block;
}

.language-option {
  padding: 8px 12px;
  cursor: pointer;
  transition: background-color 0.2s;
}

.language-option:hover {
  background-color: #f0f0f0;
}

.language-option.active {
  background-color: #e6f7ff;
  font-weight: bold;
}
</style>


<script>
document.addEventListener('DOMContentLoaded', function() {
  // 语言切换功能
  const languageOptions = document.querySelectorAll('.language-option');
  languageOptions.forEach(option => {
    option.addEventListener('click', function() {
      const langCode = this.getAttribute('data-lang');
      const currentPath = window.location.pathname;
      
      // 提取当前文件路径（不含语言代码）
      const pathMatch = currentPath.match(/\/[a-z]{2}\/(.+)$/);
      const filePath = pathMatch ? pathMatch[1] : 'home.md';
      
      // 构建新路径
      const newPath = '/' + langCode + '/' + filePath;
      window.location.href = newPath;
    });
  });
});
</script>

<!-- 语言切换器结束 -->




> This is not a complete list of commands for mcMMO, this page is a WIP. Feel free to contribute!
{.is-warning}

# mcMMO 命令

## 插件 Info / Description

These commands provide basic information and settings for mcMMO.

| 命令      | Aliases   | Description                              | 权限               |
|--------------|-----------|------------------------------------------|--------------------------|
| `/mcmmo`     | None      | Shows a brief description of mcMMO.      | `mcmmo.commands.mcmmo`   |

---

## 技能 Management

Manage and view your mcMMO skills, experience, and rankings.

| 命令      | Aliases                        | Description                              | 权限                |
|--------------|--------------------------------|------------------------------------------|---------------------------|
| `/mctop`     | None                           | Shows mcMMO leaderboards.                | `mcmmo.commands.mctop`    |
| `/mcrank`    | None                           | Displays your mcMMO ranking.             | `mcmmo.commands.mcrank`   |
| `/mcstats`   | `/stats`                       | Shows your mcMMO stats and 经验值.           | `mcmmo.commands.mcstats`  |
| `/mmopower`  | `/mmopowerlevel`, `/powerlevel`| (WIP) Shows your powerlevel. | `mcmmo.commands.mmopower` |

### 技能 命令

View detailed information about specific skills:

| 命令        | Aliases | Description                      | 权限                  |
|----------------|---------|----------------------------------|-----------------------------|
| `/excavation`  | None    | Detailed mcMMO 挖掘 skill info. | `mcmmo.commands.excavation` |
| `/herbalism`   | None    | Detailed mcMMO 草药学 skill info.  | `mcmmo.commands.herbalism`  |
| `/mining`      | None    | Detailed mcMMO 采矿 skill info.     | `mcmmo.commands.mining`     |
| `/woodcutting` | None    | Detailed mcMMO 伐木 skill info.| `mcmmo.commands.woodcutting`|
| `/axes`        | None    | Detailed mcMMO 斧技 skill info.       | `mcmmo.commands.axes`       |
| `/archery`     | None    | Detailed mcMMO 箭术 skill info.    | `mcmmo.commands.archery`    |
| `/crossbows`   | None    | Detailed mcMMO 弩技 skill info.  | `mcmmo.commands.crossbows`  |
| `/swords`      | None    | Detailed mcMMO 剑术 skill info.     | `mcmmo.commands.swords`     |
| `/taming`      | None    | Detailed mcMMO 驯兽 skill info.     | `mcmmo.commands.taming`     |
| `/tridents`    | None    | Detailed mcMMO 三叉戟 skill info.   | `mcmmo.commands.tridents`   |
| `/unarmed`     | None    | Detailed mcMMO 格斗 skill info.    | `mcmmo.commands.unarmed`    |
| `/acrobatics`  | None    | Detailed mcMMO 杂技 skill info. | `mcmmo.commands.acrobatics` |
| `/repair`      | None    | Detailed mcMMO 修理 skill info.     | `mcmmo.commands.repair`     |
| `/fishing`     | None    | Detailed mcMMO 钓鱼 skill info.    | `mcmmo.commands.fishing`    |
| `/smelting`    | None    | Detailed mcMMO Smelting skill info.   | `mcmmo.commands.smelting`   |
| `/alchemy`     | None    | Detailed mcMMO 炼金术 skill info.    | `mcmmo.commands.alchemy`    |
| `/salvage`     | None    | Detailed mcMMO Salvage skill info.    | `mcmmo.commands.salvage`    |
| `/maces`       | None    | Detailed mcMMO 锤技 skill info.      | `mcmmo.commands.maces`      |

---

## Party 命令

Manage your party and interact with party members.

| 命令    | Aliases          | Description                              | 权限                |
|------------|------------------|------------------------------------------|---------------------------|
| `/party`   | None             | Create or join a party.                  | `mcmmo.commands.party`    |
| `/ptp`     | None             | Teleport to a party member.              | `mcmmo.commands.ptp`      |
| `/partychat`| `/pc`, `/p`     | Toggle party chat or send party chat messages. | `mcmmo.chat.partychat` |

---

## 管理员 Chat 命令

Manage chat-related functionalities within mcMMO.

| 命令        | Aliases     | Description                                         | 权限                  |
|----------------|-------------|-----------------------------------------------------|-----------------------------|
| `/adminchat`   | `/ac`, `/a` | Toggle 管理员 chat or send admin chat messages.      | `mcmmo.chat.adminchat`      |

---

## 管理员 命令

命令 intended for server administrators to manage mcMMO settings and users.

| 命令              | Aliases             | Description                                                    | 权限                      |
|----------------------|---------------------|----------------------------------------------------------------|---------------------------------|
| `/mmoedit`   | None      | Edit the mcMMO skill values for a user.   | `mcmmo.commands.mmoedit` |
| `/xprate`            | `/mcxprate`         | Modify the 经验值 rate or start an event.                          | `mcmmo.commands.xprate`         |
| `/mcpurge`           | None                | Purge users with 0 power level and/or inactive for months.     | `mcmmo.commands.mcpurge`        |
| `/mcremove`          | None                | Remove a user from the mcMMO database.                         | `mcmmo.commands.mcremove`       |
| `/mcgod`             | None                | Toggle mcMMO god-mode on/off.                                  | `mcmmo.commands.mcgod`          |
| `/mcmmoreloadlocale` | `/mcreloadlocale`   | Reloads mcMMO locale settings.                                 | `mcmmo.commands.reloadlocale`   |
| `/mmoxpbar`          | `/xpbarsettings`    | Change 经验值 bar settings.                                        | `mcmmo.commands.mmoxpbar`       |
| `/mcchatspy`         | None                | Toggle mcMMO Party Chat spying on/off.                        | `mcmmo.commands.mcchatspy`      |
| `/mcrefresh` | None      | Refresh all cooldowns for mcMMO abilities. | `mcmmo.commands.mcrefresh` |
| `/addxp`     | None                           | Adds mcMMO 经验值 to a user.                  | `mcmmo.commands.addxp`    |
| `/addlevels` | None                           | Adds mcMMO levels to a user.              | `mcmmo.commands.addlevels`|
| `/skillreset`| None                           | Resets the level of one or all of your skills. | `mcmmo.commands.skillreset` |
| `/mcconvert` | None                           | Converts between different database and formula types. | `mcmmo.commands.mcconvert` |
| `/mcmmoreloadlocale` | `/mcreloadlocale`                                                                                            | Reloads mcMMO locale settings.          | `mcmmo.commands.reloadlocale` |

---

## Miscellaneous 命令

Additional commands for various functionalities within mcMMO.

| 命令              | Aliases                                                                                                      | Description                             | 权限                    |
|----------------------|--------------------------------------------------------------------------------------------------------------|-----------------------------------------|-------------------------------|
| `/mcnotify`          | `/notify`                                                                                                    | Toggle mcMMO abilities chat display notifications on/off. | `mcmmo.commands.mcnotify`     |
| `/mcscoreboard`      | `/mcsb`                                                                                                      | Manage your mcMMO Scoreboard.           | `mcmmo.commands.mcscoreboard` |
| `/mcability`         | None                | Toggle whether abilities get readied on right-click.           | `mcmmo.commands.mcability`      |
| `/mmocompat` | None      | Provides information about server compatibility and mode. | None             |

## Removed 命令
These commands existed for a brief period of time in older versions of mcMMO.

| 命令    | Aliases                                                                                                      | Description                                 | 权限                  |
|------------|--------------------------------------------------------------------------------------------------------------|---------------------------------------------|-----------------------------|
| `/hardcore`| `/mchardcore`                                                                                                | Modify the mcMMO hardcore percentage or toggle hardcore mode (removed). | `mcmmo.commands.hardcore`       |
| `/vampirism`| `/mcvampirism`                                                                                               | Modify the mcMMO vampirism percentage or toggle vampirism mode (removed). | `mcmmo.commands.vampirism`      |
| `/mcfools` | `/macho`, `/jumping`, `/throwing`, `/wrecking`, `/walking`, `/swimming`, `/falling`, `/climbing`, `/flying`, `/diving`, `/piggy` | April Fools command (removed). | `mcmmo.commands.mcfools` |

