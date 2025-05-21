---
title: Plugin Integrations
description: mcMMO integrations when used with other plugins
published: true
date: 2024-11-24T02:29:34.304Z
tags: plugin-integration, world guard
editor: markdown
dateCreated: 2024-11-24T02:29:34.304Z
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




# Plugin Integration
mcMMO has limited support for some optional features when used with other plugins, such as World Guard.

> Feel free to ask for support for integration with other plugins in the discord, or to expand existing support, I'm always open to suggestions

# World Guard
## World Guard Region Flags
`mcmmo` Enables or disables mcMMO in a specific WG region
`mcmmo-xp` Enable or disable mcMMO XP in a specific WG region
`mcmmo-hardcore` Enable or disable mcMMO hardcore features in a specific WG region


> This page is under construction, **you** can add to it and help complete it!
{.is-warning}

## PAPI / Placeholders
### Note
The latest versions of mcMMO have built in support for PAPI, no need to download anything from the PAPI ecloud.

# mcMMO Placeholders for PlaceholderAPI (PAPI)

## Skill-Specific Placeholders

- `%mcmmo_level_<skillname>%` - Current level of the skill.
- `%mcmmo_xp_<skillname>%` - Current XP in the skill.
- `%mcmmo_xp_remaining_<skillname>%` - XP remaining to level up in the skill.
- `%mcmmo_xp_needed_<skillname>%` - Total XP needed for the next level.
- `%mcmmo_rank_<skillname>%` - Rank of the player in the skill.
- `%mcmmo_xprate_<skillname>%` - XP rate multiplier for the skill.

## General Placeholders
These placeholders are not skill-specific:

- `%mcmmo_power_level%` - Player's total power level (sum of all skill levels).
- `%mcmmo_power_level_cap%` - Maximum power level cap.

## Party Placeholders
These placeholders provide information about the player's party status:

- `%mcmmo_in_party%` - Whether the player is in a party (true/false).
- `%mcmmo_party_name%` - Name of the party the player belongs to.
- `%mcmmo_is_party_leader%` - Whether the player is the leader of the party (true/false).
- `%mcmmo_party_leader%` - Name of the party leader.
- `%mcmmo_party_size%` - Number of members in the party.

## XP Event Placeholders
These placeholders are related to global XP events:

- `%mcmmo_is_xp_event_active%` - Whether an XP event is currently active (true/false).
- `%mcmmo_xprate%` - Current global XP rate multiplier.

### Notes
- Replace `<skillname>` with the lowercase name of the skill (e.g., `mining`, `fishing`).
- Ensure PlaceholderAPI and mcMMO are correctly configured for these placeholders to function.
