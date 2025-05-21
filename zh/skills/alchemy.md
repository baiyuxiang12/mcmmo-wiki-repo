---
title: 炼金术
description: View information about the mcMMO Skill Alchemy.
published: true
date: 2024-11-24T01:41:12.847Z
tags: alchemy, skills
editor: markdown
dateCreated: 2022-07-16T21:46:19.551Z
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




# 炼金术
> This page is under construction, **you** can add to it and help complete it!
{.is-warning}

炼金术 is about brewing potions. It provides a speed increase in the potion brew time, as well as the addition of new (previously) unobtainable potions.

## 经验值 Gain

经验 in 炼金术 is gained by successfully crafting potions and by adding additional ingredients to existing potions.

## Passive Sub-技能

### Catalysis

Catalysis speeds of the brewing process, with a max speed of 4x at level 1000. This ability is unlocked at level 100 by default.

### Concoctions

Concoctions allows brewing of more potions with custom ingredients. Which special ingredients are unlocked is determined by your Rank. There are 8 ranks to unlock.

| Concoction Tier | Ingredients |
|-----------------|-------------|
| Tier 1 | Blaze Powder, Fermented Spider Eye, Ghast Tear, Redstone, Glowstone Dust, Sugar, Glistering Melon, Golden Carrot, Magma Cream, Nether Wart, Spider Eye, Suplhur, Water Lily, Pufferfish (Vanilla Potions) |
| Tier 2 | Carrot (Potion of Haste)<br>Slimeball (Potion of Dullness) |
| Tier 3 | Quartz (Potion of Absorption)<br>Rabbit's Foot (Potion of Leaping) |
| Tier 4 | Apple (Potion of Health Boost)<br>Rotten Flesh (Potion of Hunger) |
| Tier 5 | Brown Mushroom (Potion of Nausea)<br>Ink Sack (Potion of Blindness) |
| Tier 6 | Fern (Potion of Saturation)
| Tier 7 | Poisonous Potato (Potion of Decay) |
| Tier 8 | Regular Golden Apple (Potion of Resistance) |

