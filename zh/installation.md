---
title: Install or Update mcMMO
description: Instructions on how to install or update mcMMO
published: true
date: 2024-11-24T02:31:22.978Z
tags: install, update
editor: markdown
dateCreated: 2022-07-17T22:27:04.825Z
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




# 安装 & Upgrading

## Pre-Requisites

-   Recommended to use the latest version of Java Minecraft
-   Use a compatible version of Spigot, Paper or Folia

> mcMMO officially supports Spigot, Paper, and Folia. Any support outside of these platforms is unsupported at best.


Modern versions of mcMMO expect you to be running the latest available Java Minecraft release, however older versions of mcMMO are still available and should work perfectly fine for those playing on legacy versions.  
mcMMO is a plugin for the Spigot API接口, which makes running Spigot or Paper a requirement, other forks of Spigot/Paper may work but for those wanting a painless installation and having everything just work we officially recommend sticking to Spigot or Paper.  
Historically very old versions of mcMMO ran directly against CraftBukkit (the spiritual predecessor to Spigot) but this is no longer the case and mcMMO will not work if you are just running CraftBukkit.

## Installing the newest mcMMO

1.  Grab the latest version of mcMMO from the spigotmc or polymart
2.  Place mcMMO.jar in /path/to/your/spigotorpaperserver/plugins/ directory

## Upgrading to the newest mcMMO

Upgrading mcMMO is meant to be as simple as possible, you are never required to delete data or configs.

1.  Grab the latest version of mcMMO from spigotmc or polymart
2.  Make sure that your Spigot or Paper server is up to date
3.  Place mcMMO.jar in /path/to/your/spigot-or-paper-or-folia-server/plugins/ directory
4.  Replace the existing mcMMO.jar

Congratulations, you have upgraded mcMMO. Make sure you are running a compatible version of Java Minecraft and Spigot/Paper. The newest versions of mcMMO target the latest versions of Java Minecraft and therefor may not work with older versions.

# 配置 Updates

If you have been running mcMMO for a while, chances are you may be on an older version of the config. mcMMO will for the most part respect user config settings, so it does not modify when they change unless it is necessary to keep mcMMO working.

Occasionally mcMMO will update its default config file values, and in certain config files if you do not add the new values yourself they simply won't exist. This is true for the treasure config files, the repair config files, and salvage config files.  
 

## Updating your mcMMO config files

If you're the type of server owner who does no customization of the aforementioned config files, you can simply delete the .yml files you find inside the mcMMO directory to regenerate the file with the latest default values. If you are the type who does customize their mcMMO installation extensively, then you will want to follow the changelog with every release and update values in these config files yourself as needed. Take care to not delete the mcMMO directory itself as that is where player data is saved by default. 

# Legacy

## Upgrading from mcMMO classic

If you are upgrading from mcMMO classic you will be able to follow the upgrade instructions and everything should work normally. However you will not be able to go back to mcMMO classic after you do this as the config files get updated to be compatible with the newest changes in mcMMO. A simple fix to this is to simply delete the .yml files when switching back to classic, and classic will generate new ones.

## Legacy 安装 & Pre-Requisites

When using mcMMO against older versions of the game you must make sure to use a compatible version of mcMMO for that version of the game, and you must match this with the latest version of Spigot or Paper for that version of Java Minecraft. Legacy versions are as-is and any bugs/exploits found in them are simply left the way they are. No effort is underway by mcMMO devs to maintain legacy versions at this time.

-   Grab the version of mcMMO compatible with the version of Java Minecraft you are using
-   Grab the latest Spigot or Paper software for that version of Java Minecraft
-   Place mcMMO.jar in /path/to/your/legacy/spigot-or-paper-or-folia-server/plugins/ directory

If you encounter any errors/issues running Legacy versions, make sure that you have the latest Spigot (from BuildTools) or the latest Paper. If issues persist, you are likely out of luck as legacy versions are as-is and receive no updates, however mcMMO source code is freely available on GitHub so those with a programming background can fork older versions of the codebase and fix any problems themselves.