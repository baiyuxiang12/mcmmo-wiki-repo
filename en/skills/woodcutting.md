---
title: Woodcutting
description: View information about the Herbalism skill for mcMMO!
published: true
date: 2024-11-24T01:42:53.899Z
tags: skills, woodcutting
editor: markdown
dateCreated: 2022-07-17T14:37:12.913Z
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




# Woodcutting
> This page is under construction, **you** can add to it and help complete it!
{.is-warning}

Woodcutting is all about chopping down trees.

## XP Gain

XP is gained whenever you break log blocks.

## How does Tree Feller work?

Tree Feller is an active ability, you can right-click while holding an axe to activate Tree Feller. This will cause the entire tree to break instantly, dropping all of its logs at once.

## How does Leaf Blower work?

Leaf Blower is a passive ability that will cause leaf blocks to break instantly when hit with an axe. By default, this ability unlocks at level 100.

## How do Double Drops work?

This passive ability gives you a chance to obtain an extra block for every log you chop.
