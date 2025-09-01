---
title: m3ww
layout: /src/layouts/autonum.astro
sidebar:
  badge:
    text: অবহিত
    variant: caution
lastUpdated: 2025-08-30
---

:::danger[সতর্কতা]
এই গুচ্ছ কনফিগ আর বজায় রাখা হচ্ছে না। আমরা এদের ব্যাবহার না করতে সুপারিশ করি।
:::

# Description
- সবচেয়ে আধুনিক ইউউ চালিত সেটআপ যা [Material Design 3](https://m3.material.io/) এর ধরন অনুসরণ করে
# Installation
- দিপেন্দেন্সি নামান এবং ব্যাবহারকারিকে `video` গোত্রে যোগ করুন 
```bash
# সাধারণ প্যাকেজ
sudo pacman -S bc blueberry bluez boost boost-libs cliphist coreutils curl findutils fish fuzzel fzf gawk gnome-control-center gnome-keyring grim ibus imagemagick libqalculate light networkmanager network-manager-applet nlohmann-json pavucontrol plasma-browser-integration playerctl procps polkit-gnome ripgrep slurp socat sox starship udev upower util-linux xorg-xrandr wget wireplumber yad tesseract
# AUR প্যাকেজ - yay ব্যাবহার করে ইন্সটলেশন
yay -S cava eww-tray-wayland-git geticons gojq gtklock gtklock-playerctl-module gtklock-powerbar-module gtklock-userinfo-module hyprland-git lexend-fonts-git python-material-color-utilities python-pywal python-desktop-entry-lib python-poetry python-build python-pillow swww ttf-material-symbols-git wlogout
# ব্যাবহারকারিকে `video` গোত্রে করুন
sudo usermod -aG video $(whoami)
```
- এগুলো কপি করুন
    - `.config`, `.local` আপনার home ফলদার এ
    - `.local/share/icons` এ থাকা ফলদার আপনার `/usr/share/icons` তে
    - `Import manually`তে থাকা জিনিসপাতি যদি আপনার দরকার পরে

- অইচ্ছিক
   - বিশেষ দ্রষ্টব্য: আপনার যদি একাধিক কিবোর্ড বিন্যাস এর দরকার না হয় তাহলে `~/.config/hypr/execs.conf` তে ibus জনিত সকল কিছু কমেন্ট বানান। যদি দরকার হয় তাহলে আপনি হয়তো fcitx5 ব্যাবহার করতে চাবেন (যদিও এটা বার এ থাকা আইকন এর সাথে একীভূত হবে না)
   - যদি আপনি চান ব্রাউসার থেকে মিডিয়া থাম্বনেল দেখতে চান তাহলে "plasma browser extension" নামক এক্সটেনশন নামান
     - [Chromium](https://chrome.google.com/webstore/detail/plasma-integration/cimiefiiaegbelhefglklhhakcgmhkai) এর জন্য
     - [Firefox](https://addons.mozilla.org/en-US/firefox/addon/plasma-integration/) এর জন্য

