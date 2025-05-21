---
title: Home
description: Welcome!
published: true
date: 2024-11-24T02:30:53.032Z
tags: 
editor: markdown
dateCreated: 2022-07-16T05:21:57.454Z
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




> A gentle reminder that **anyone** can edit this wiki, and I would *sincerely* appreciate any volunteers from the community to help bring pages up to date.
{.is-warning}

# mcMMO Wiki

Welcome to the mcMMO wiki.

The pages on this wiki can be edited by the community on [our wiki git repo](https://github.com/mcMMO-Dev/mcmmo-wiki-repo) hosted on GitHub.
It would be wonderful if you would make any contribution to help us get the wiki up to date.

Use the sidebar or the search function to find what you're looking for!

## Get mcMMO
- [Download mcMMO from Polymart](https://polymart.org/resource/mcmmo.727)
- [Download mcMMO from Spigot](https://www.spigotmc.org/resources/official-mcmmo-original-author-returns.64348/)
## mcMMO Development
- [mcMMO GitHub](https://github.com/mcMMO-Dev/mcMMO)
- [Changelog](https://github.com/mcMMO-Dev/mcMMO/blob/master/Changelog.txt)
- [mcMMO Community Discord](https://discord.gg/mcmmo)

## Getting Started

- [Installation](/installation) - Everything you need to know about installing or updating mcMMO
- [Skills](/skills) - Read about mcMMO skills and sub-skills
- [Permissions](/permissions) - Information on permission nodes used within mcMMO

## Useful Pages

- [Configuration](/config) - Customize mcMMO
- [Locale](/locale) - Customize mcMMO messages or change the language for mcMMO
- [Plugin Integration](/plugin-integration/plugin-support) - Optional mcMMO features making use of other plugins
- [World Blacklist](/config/world-blacklist) - Information about the world blacklist feature
- [Hardcore Mode](/config/hardcore-mode) - Information about mcMMO's optional hardcore mode
- [Vampirisim](/config/vampirism) - Information about mcMMO's optional vampirism PVP setting

## For plugin developers...

- [API](/api/mcmmo-api) - mcMMO API Information for developers