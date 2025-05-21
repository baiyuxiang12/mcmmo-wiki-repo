---
title: 采矿
description: View information about the Mining skill for mcMMO!
published: true
date: 2024-11-24T01:44:31.134Z
tags: mining, skills
editor: markdown
dateCreated: 2022-07-17T14:27:25.815Z
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




# 采矿

> This page is under construction, **you** can add to it and help complete it!
{.is-warning}

采矿 consists of mining stone and ores. It provides bonuses to the amount of materials dropped while mining.

## 经验值 Gain

To gain 经验值 in this skill, you must mine with a pickaxe in hand. Only certain blocks award 经验值.

Compatible Materials: Stone, Coal Ore, Iron Ore, Gold Ore, Diamond Ore, Redstone Ore, Lapis Ore, Obsidian, Mossy Cobblestone, Ender Stone, Glowstone, and Netherrack.

## 如何 use Super Breaker

With a pickaxe in your hand, right click to ready your tool. Once in this state, you have about 4 seconds to make contact with 采矿 compatible materials, which will activate Super Breaker.

## What is Super Breaker?

Super Breaker is an ability with a cooldown tied to the 采矿 skill. It triples your chance of extra items dropping and enables instant break on 采矿 materials.

## 如何 use Blast 采矿

With a pickaxe in hand, crouch and right-click on TNT from a distance. This will cause the TNT to instantly explode.

## How does Blast 采矿 work?

Blast 采矿 is an ability with a cooldown tied to the 采矿 skill. It gives bonuses when mining with TNT and allows you to remote detonate TNT. There are three parts to Blast 采矿. The first part is Bigger Bombs, which increases blast radius. The second is Demolitions Expert, which decreases damage from TNT explosions. The third part simply increases the amount of ores dropped from TNT and decreases the debris dropped.
