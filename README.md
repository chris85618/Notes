# Notes

## Introduction

* This repository places some notes about cyber security.

## File Manifests

* `README.md`: This README file.
* [`112-1-Cryptography.md`](./112-1-Cryptography/112-1-Cryptography.md): My note about Cryptography in the 1st semester of 2024 in NTUT.
* [`112-2-PPSC.md`](./112-2-PPSC/112-2-PPSC.md): My note about PPSC in the 2nd semester of 2024 in NTUT.

## Fork the Repository

1. Fork it
2. 修改PlantUML渲染的時使用的連結
    * Solution　(Linux):
      ```
      cd <repository_path>;
      YOUR_REPOSITORY_NAME=<GithubName>/Notes;
      sed -i "s:\(http\://www\.plantuml\.com/plantuml/proxy?cache=no&src=https\://raw\.githubusercontent\.com/\)chris85618/Notes\(/main/.*\.puml\):\1${YOUR_REPOSITORY_NAME}\2:g" $(find -mindepth 2 -type f -name '*.md');
      ```
    * Problem: [`112-1-Cryptography.md`](./112-1-Cryptography/112-1-Cryptography.md)及[`112-2-PPSC.md`](./112-2-PPSC/112-2-PPSC.md)有使用PlantUML來撰寫，但是Markdown沒有原生支援PlantUML的繪圖功能，且GitHub版的Markdown render也不支援，因此目前的作法是使用PlantUML的官方方式來渲染，例如: `![](http://www.plantuml.com/plantuml/proxy?cache=no&src=https://raw.githubusercontent.com/chris85618/Notes/main/112-1-Cryptography/images/plantuml_1.puml)`
    以此為例，當中需要帶入source code的完整連結，因為fork之後的repository link會改變，因此會需要修改所有與repository link有關的連結: https://raw.githubusercontent.com/chris85618/Notes/main/112-1-Cryptography/images/plantuml_1.puml

