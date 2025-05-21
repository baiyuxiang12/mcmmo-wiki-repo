---
title: 挖掘
description: View information about the Excavation skill for mcMMO!
published: true
date: 2024-11-24T01:43:42.890Z
tags: excavation, skills
editor: markdown
dateCreated: 2022-07-17T01:36:33.657Z
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




# 挖掘
> This page is under construction, **you** can add to it and help complete it!
{.is-warning}

挖掘 is the act of digging up dirt to find treasures. By excavating the land you will find treasures. The more you do this the more treasures you can 

## 经验值 Gain

To gain 经验值 in this skill you must dig with a shovel in hand. Only certain materials can be dug up for treasures and 经验值.

Compatible Materials: Grass, Dirt, Sand, Clay, Gravel, Mycelium, Soul Sand, Snow

## 如何 use Giga Drill Breaker

With a shovel in hand right click to ready your tool. Once in this state you have about 4 seconds to make contact with 挖掘 compatible materials this will activate Giga Drill Breaker.

## What is Giga Drill Breaker?

Giga Drill Breaker is an ability with a cooldown tied to 挖掘 skill. It triples your chance of finding treasures and enables instant break on 挖掘 materials.

## How does Archaeology work?

Every possible treasure for 挖掘 has its own skill level requirement for it to drop, as a result it's difficult to say how much it is helping you. Just keep in mind that the higher your 挖掘 skill is, the more treasures that can be found. And also keep in mind that each type of 挖掘 compatible material has its own unique list of treasures. In other words you will find different treasures in Dirt than you would in Gravel.

## Notes about 挖掘

> 挖掘 drops are completely customizable, so results vary server to server.
{.is-warning}

