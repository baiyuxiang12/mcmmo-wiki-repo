---
title: Localization
description: Learn how to edit the locale in mcMMO!
published: true
date: 2022-07-18T00:13:13.163Z
tags: locale
editor: markdown
dateCreated: 2022-07-18T00:13:13.163Z
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




# 本地化

## Built in translations

mcMMO has several built in translations, you can choose which translation by updating config.yml with the appropriate locale code For a list of built in translations, view this link: https://github.com/mcMMO-Dev/mcMMO/tree/master/src/main/resources/locale

## Info on overriding / customizing locales

Locales are the language files used by mcMMO, they also contain color codes and most of the styling used by mcMMO. You can customize a locale outside of the JAR in version 2.1.51 and up.

Locales can be overridden by placing a file with an appropriate name inside /plugins/mcMMO/locales/

You can find the up to date current en_US locale entries on the [GitHub repo](https://github.com/mcMMO-Dev/mcMMO/blob/master/src/main/resources/locale/locale_en_US.properties).

Make a new file with the same name as this one, and copy only the strings you want to replace, otherwise you will not see any updated strings as they are changed as your copy of the file will have priority. If you wish to replace every line in some way, feel free to copy the entire contents of this file, just be advised that you will need to be on top of locale updates in mcMMO.

Locales only support ASCII and UTF16 characters at the moment, so you'll need to run special characters through a UTF16 converter (google it) to get them to work. This will be fixed in the future!

The locale name must match the internal file you are overriding (ie: `locale_en_US.properties`) The locale file names are structured like this `locale_XX_XX.properties`, replace XX with your country codes, if you are not overriding `en_US` you will have to change the targetted locale inside `config.yml`.

本地化 will first check for a users locale file, if it doesn't exist it will use the files inside the JAR.

If a locale is found, it will use locale entries from that file, and if any entries are missing, it will use entries from en_US inside the JAR

You must restart the server for these changes to take effect. Once you have the locale file set in the config.yml file, you can use the command `/mcmmoreloadlocale` if you make changes to the locale properties file. This command only affects a locale properties file, not a config file.