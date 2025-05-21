---
title: 技能
description: View an overview of all mcMMO 技能!
published: true
date: 2024-11-24T01:59:07.533Z
tags: skills
editor: markdown
dateCreated: 2022-07-16T20:23:34.236Z
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




# 技能

> This page is under construction, **you** can add to it and help complete it!
{.is-warning}

mcMMO has several skills for you to level up and gain abilities with. There are 16 parent skills. Each of them are breifly described below, and you may click on the skill name to view more information.

## [Acrobatics](/skills/acrobatics)

杂技 is the art of moving Gracefuly in mcMMO. It provides combat bonuses and environment damage bonuses.

## [Alchemy](/skills/alchemy)

炼金术 is about brewing potions. It provides a speed increase in the potion brew time, as well as the addition of new (previously) unobtainable potions.

## [Archery](/skills/archery)

箭术 is about shooting with your bow and arrow. It provides various combat bonuses, such as a damage boost that scales with your level and the ability to daze your opponents in PvP. In addition to this, you can retrieve some of your spent arrows from the corpses of your foes.

## [Axes](/skills/axes)

With the 斧技 skill you can use your axe for much more then just deforesting! You can hack and chop away at mobs and players to gain 经验值, hitting mobs with the effect of knockback and inflicting DEADLY criticals on mobs and players. Your axe also becomes a hand-held woodchipper, breaking down the enemy's armor with ease as your level increases.

## [Crossbows](/skills/crossbows)

弩技 is all about shooting with your crossbow.

## [Excavation](/skills/excavation)

挖掘 is the act of digging up dirt to find treasures. By excavating the land you will find treasures. The more you do this the more treasures you can find.

## [Fishing](/skills/fishing)

With the 钓鱼 skill, 钓鱼 is exciting again! Find hidden treasures, and shake items off mobs.

## [Herbalism](/skills/herbalism)

草药学 is about collecting herbs and plants.

## [Maces](/skills/maces)

The 锤技 skill is great at crushing your foes. 

## [Mining](/skills/mining)

采矿 consists of mining stone and ores. It provides bonuses to the amount of materials dropped while mining.

## [Repair](/skills/repair)

修理 allows you to use an iron block to repair armor and tools.

## [Swords](/skills/swords)

This skill awards combat bonuses to anyone fighting with a sword.

## [Taming](/skills/taming)

驯兽 will give players various combat bonuses when using tamed wolves.

## [Tridents](/skills/tridents)

The 三叉戟 skill involves impaling foes with your trident.

## [Unarmed](/skills/unarmed)

格斗 will give players various combat bonuses when using your fists as a weapon. 

## [Woodcutting](/skills/woodcutting)

伐木 is all about chopping down trees.