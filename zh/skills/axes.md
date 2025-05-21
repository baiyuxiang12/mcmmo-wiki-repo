---
title: 斧技
description: View information for the mcMMO Skill Axes.
published: true
date: 2024-11-24T01:43:23.987Z
tags: axes, skills
editor: markdown
dateCreated: 2022-07-17T01:32:38.684Z
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




# 斧技
> This page is under construction, **you** can add to it and help complete it!
{.is-warning}

With the 斧技 skill you can use your axe for much more than just deforesting! You can hack and chop away at mobs and players to gain 经验值, hitting mobs with the effect of knockback and inflicting DEADLY criticals on mobs and players. Your axe also becomes a hand-held woodchipper, breaking down the enemy's armor with ease as your level increases.

## 经验值 Gain

To gain 经验值 in this skill you need hit other mobs or players with an Axe.

## How does Skull Splitter work?

This ability allows you to deal an AoE (Area of Effect) hit. This AoE hit will deal half as much damage as you did to the main target, so it's great for clearing out large piles of mobs.

## How does Critical Strikes work?

Critical Strikes is a passive ability which gives players a chance to deal additional damage. With the default settings, every 2 skill levels in 斧技 awards a 0.1% chance to deal a Critical Strike, causing 2.0 times damage to mobs or 1.5 times damage against other players.

## How does Axe Mastery work?

Axe Mastery is a passive ability that will add additional damage to your hits when using 斧技. By default, the bonus damage increases by 1 every 50 levels, up to a cap of 4 extra damage at level 200.

## How does Armor Impact work?

Strike with enough force to shatter armor! Armor Impact has a passive chance to damage your opponent's armor. This damage increases as you level in 斧技.

## How does Greater Impact work?

You have a passive chance to achieve a greater impact when hitting mobs or players with your axe. By default this chance is 25%. This passive ability has an extreme knockback effect, similar to the Knockback II enchantment. In addition, it deals bonus damage to the target.
