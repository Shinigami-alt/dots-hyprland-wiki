---
title: Eww (multiple)
layout: /src/layouts/autonum.astro
sidebar:
  badge:
    text: Deprecated
    variant: caution
lastUpdated: 2024-02-18
---

:::danger[সতর্কতা]
এই গুচ্ছ কনফিগ আর বজায় রাখা হচ্ছে না। আমরা এদের ব্যাবহার না করতে সুপারিশ করি।
:::

# বর্ণনা
কয়েক গুচ্ছ কনফিগ, এমনকি `windoes`, `hybrid` এবং `NovelKnock`, ইত্যাদি।
# Installation
- দিপেন্দেন্সিগুচ্ছ: শাখা নির্দিষ্ট দিপেন্দেন্সি তালিকা দেখুন।
- এগুলো কপি করুন
    - `.config`, `.local` আপনার গৃহ ফলদারে
    - `.local/share/icons` তে থাকা ফলদার আপনার `/usr/share/icons` তে
    - `Import manually`তে থাকা জিনিসপাতি যদি আপনার দরকার পরে

 ## দক্ষতা
|  ⌄  | ব্যাবহার করুন | রেকমেন্দ করি না | Notes                 |
| --- | ------ | ----------- | ------------------------- |
| Kernel |     | cachyos, xanmod | পাওয়ার সেভার উতিরিক্ত ব্যাবহার করিয়েন না। এবং আমি ঠিক বুঝতেসি না আমি কি বলতেছি - এটা সুধু আমার বাস্তপ অভিজ্ঞতা থেকে বলা। |
| Login shell  | bash/zsh | fish | টার্মিনাল এ ব্যাবহার করায় সমস্যা নেই - end_4 এটাই করে থাকে। |

 ## Setup
 - একমাত্র `~/.config/eww` তে ইউউ কনফিগগুলো কাজ করে
 - `eww daemon` দিয়ে ইউউ শুরু করুন
 - উপরের বার খলার জন্য: `eww open bar`
 - উইন্দস বার খলার জন্য: `eww open winbar` (`windoes`/`hybrid` শাখা)
 - নিম্ন লাইন খলার জন্য: `eww open bottomline` (যাতে আপনি স্ক্রিন এর নিম্ন অংশ ক্লিক করলে গান এর উইন্ডটা খুলে)
 - Open the overview (middle-click workspaces) and wait 10 seconds (for it to generate app search cache, or icons won't show properly)
 ## Usage
 - Music controls: Middle-click for Play/Pause, Right-click for Next track, scroll to change volume
 - To open the Overview, middle/right-click the workspace indicators or run `eww open overview`
 - In overview, type to search apps (see more below)
 ## Search
 - Type to search apps
 - Type math (must begin with number) to calculate using `qalc`
 - `>save THEME`: Saves current colorscheme, with THEME as the name.
 - `>load THEME`: Loads a saved theme. Available themes will be shown as you type.
 - `>music`: Get colorscheme from current media thumbnail
 - `>wall`: Get colorscheme from wallpaper located in `~/.config/eww/images/wallpaper/wallpaper`
 - `>light`: Remember to use light mode for next color generations
 - `>dark`: Remember to use dark mode for next color generations
 - `>one`: Remember to use only one color for bar icons for next color generations
 - `>multi`: Remember to use many colors for bar icons for next color generations
 - `>r`: Reload (kills and relaunches eww with the default bar)
