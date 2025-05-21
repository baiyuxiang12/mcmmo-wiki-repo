---
title: 杂技
description: View information about the Acrobatics skill for mcMMO!
published: true
date: 2022-08-08T16:22:50.747Z
tags: [acrobatics, skills]
editor: markdown
dateCreated: 2022-07-16T20:35:16.605Z
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




# 杂技

**杂技** is a [skill](/skills) focused around moving gracefully, reducing fall damage and avoiding attacks.

## 经验 Gain

经验 in 杂技 is gained by taking fall damage, successfully rolling on the ground, or successfully dodging attacks.

120XP per half heart of damage is gained when taking fall damage. Assuming no damage is being reduced, it can also be calculated as `(b - 3) * 120` where `b` is the amount of blocks fallen before taking damage. Any reduction of damage by use of hay bales, potions, enchantments etc. will reduce the amount of experience gained. If a roll or graceful roll as been executed, you will gain 80XP per half heart of damage instead of 120XP. This calculation uses the damage that would have been taken if you had not rolled.

Feather falling will double the amount of 经验值 you earn from falling, regardless of its enchantment level. Keep in mind that feather falling will also reduce the amount of base damage dealt when you fall.

Dodging an attack will give 120XP per half heart of damage dodged. So if you dodged an attack that would have dealt you 3 damage, it would give you 360XP.

### Anti Exploit

There is a config option found in [experience.yml](/config/experience) to prevent users from using AFK acrobatic farms that allow them to farm 经验值 while AFK.

```yml
ExploitFix:
    Acrobatics: true
```

A user will not gain experience if any of the following are true:

- User is holding an enderpearl in their main hand while inside a vehicle.
- User has teleported in the last 5 seconds
- User has landed in the same spot at least once within the last 50 times they have fallen from a high place and gained mcMMO 杂技 经验

Additionally, after gaining experience from a fall, there will be a cooldown of 3 seconds before you may gain experience again. If you take more fall damage during this period, extra time is added to the cooldown, starting at an additional 10 seconds and increasing by 1 each time more fall damage is taken before the cooldown is over.

## Active Sub-技能

### Roll

Rolling is an active sub-skill with a passive component. It provides a chance to negate fall damage based on the player's **杂技** skill level. At level 50, the player has a 50% chance to negate damage, or 100% if **Graceful Roll** is activated. The chance for success is scaled against the 杂技 skill level in a linear curve. Every level increases the chance to roll successfully by 1%. Therefore, it will always trigger at level 100.

A normal roll can be transformed into a **Graceful Roll** by sneaking while falling. Doing so will double the odds to roll and the amount of damage prevented.

#### Odds

等级 | Retro Mode | Roll | Damage Absorbed | Graceful Roll | Damage Absorbed Graceful
|:----:|:-----:|:-----:|:---:|:--:|:--:|
25 | 250 | 25% | 7 | 50% | 14 |
50 | 500 | 50% | 7 | 100% | 14 |
75 | 750 | 75% | 7 | 100% | 14 |
| 100 | 1000 | 100% | 7 | 100% | 14 |

## Passive Sub-技能

### Dodge

> Dodge unlocks at 等级 2 or 等级 20 for Retro Mode
{.is-info}

Dodge will give you a chance of reducing incoming damage by half. For instance, if you are receiving 6 damage, you will only receive 3 damage when successfully dodging. You will never dodge an attack if the incoming damage would be lethal, this check is done before dodge reduces incoming damage. Dodge also has a cooldown before it will award 经验值 if the player recently respawned from a death.

Dodge reduces the players damage from various harmful sources. There is a config option in [config.yml](/config/config) to allow Dodge to work for lightning strikes.

```yml
技能:
    Acrobatics:
        Prevent_Dodge_Lightning: false
        XP_After_Teleport_Cooldown: 5
```
