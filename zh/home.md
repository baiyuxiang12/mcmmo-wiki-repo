---
title: 首页
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




> 温馨提示：**任何人**都可以编辑此百科，我*真诚地*感谢社区中的志愿者帮助更新页面内容。
{.is-warning}

# mcMMO百科

欢迎访问mcMMO百科。

本百科的页面可由社区在 [our wiki git repo](https://github.com/mcMMO-Dev/mcmmo-wiki-repo) 托管在GitHub上进行编辑。
如果您能为更新百科做出任何贡献，我们将不胜感激。

请使用侧边栏或搜索功能查找您需要的内容！

## 获取mcMMO
- [从Polymart下载mcMMO](https://polymart.org/resource/mcmmo.727)
- [从Spigot下载mcMMO](https://www.spigotmc.org/resources/official-mcmmo-original-author-returns.64348/)
## mcMMO开发
- [mcMMO GitHub](https://github.com/mcMMO-Dev/mcMMO)
- [Changelog](https://github.com/mcMMO-Dev/mcMMO/blob/master/Changelog.txt)
- [mcMMO社区Discord](https://discord.gg/mcmmo)

## 入门指南

- [安装](/installation) - 关于安装或更新mcMMO的所有必要信息
- [技能](/skills) - 了解mcMMO技能和子技能
- [权限](/permissions) - 关于mcMMO中使用的权限节点信息

## 实用页面

- [配置](/config) - 自定义mcMMO
- [本地化](/locale) - 自定义mcMMO消息或更改mcMMO的语言设置
- [插件集成](/plugin-integration/plugin-support) - 使用其他插件的mcMMO可选功能
- [世界黑名单](/config/world-blacklist) - 关于世界黑名单功能的信息
- [硬核模式](/config/hardcore-mode) - 关于mcMMO可选硬核模式的信息
- [吸血设置](/config/vampirism) - 关于mcMMO可选吸血PVP设置的信息

## 插件开发者专区...

- [API接口](/api/mcmmo-api) - 面向开发者的mcMMO API信息