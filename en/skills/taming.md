---
title: Taming
description: View information about the Taming skill for mcMMO!
published: true
date: 2024-11-24T01:42:19.018Z
tags: skills, taming
editor: markdown
dateCreated: 2022-07-17T14:33:02.554Z
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




# Taming
> This page is under construction, **you** can add to it and help complete it!
{.is-warning}

Taming will give players various combat bonuses when using tamed wolves.

## XP Gain

To gain XP in this skill, you need to tame wolves/ocelots or get into combat with your wolves.

## How does Call of the Wild work?

Call of the Wild is an active ability that will allow you to summon a wolf or an ocelot by your side. You can do this by sneaking + left-clicking while holding bones or fish.

## How does Beast Lore work?

Beast Lore allows players to inspect pets and to check the stats of wolves and ocelots. Left-click a wolf or ocelot to use Beast Lore.

## How does Gore work?

Gore is a passive ability that has a chance of inflicting a bleeding effect on your wolves' targets.

## How does Sharpened Claws work?

Sharpened Claws provides a damage bonus to damage dealt by wolves. The damage bonus depends on your Taming level.

## How does Environmentally Aware work?

This passive ability will allow wolves to teleport to you when they get near hazards, such as Cacti/Lava. It will also give wolves fall damage immunity.

## How does Thick Fur work?

This passive ability will reduce damage and make wolves fire resistant.

## How does Shock Proof work?

This passive ability reduces damage done to wolves from explosions.

## How does Fast Food Service work?

This passive ability gives wolves a chance to heal whenever they perform an attack.
