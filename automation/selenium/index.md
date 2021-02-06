---
title: Selenium Untuk Otomasi Jelajah Web
layout: workshop-index
description: Selenium untuk otomasi jelajah web
course-parent: automation
course-parent-url: ../
tags: [selenium]
---

https://www.selenium.dev/documentation/en/
https://selenium-python.readthedocs.io/installation.html

# Cara Penggunaan

## Instansiasi WebDriver
- WebDriver :
  - Chrome()

## Navigasi ke URL yang Diinginkan
- WebDriver :
  - get(alamat_url)
  
## Navigasi ke Window yang Diinginkan
- WebDriver :
  - switchTo() :
    - newWindow()
  - close()
  - quit()

## Mengambil Screenshot
https://www.selenium.dev/documentation/en/webdriver/browser_manipulation/

## Mencari Elemen 
- WebDriver :
  - getTitle()
- WebElement :
  - findElement(konfigurasi_selector)
  - findElements(konfigurasi_selector)

## WAIT, Menunggu Elemen Muncul
https://www.selenium.dev/documentation/en/webdriver/waits/

# Vendor Web Browser

## Chrome
- [List argumen chrome](https://peter.sh/experiments/chromium-command-line-switches/)
