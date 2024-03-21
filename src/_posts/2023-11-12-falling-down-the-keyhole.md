---
layout: post
title: "Falling down the keyhole"
date: 2023-11-12 20:40:20 -0800
categories: updates
---

# [Falling down the keyhole](#falling-down-the-keyhole)

In my previous post, I talked about my history with keyboards. This journey has not led me to the bottom of the keyboard optimization hole. Like with most rabbit holes, the deeper you go, the more you realize could possibly be below. There are some topics I haven't touch too much, like [chorded keyboards](https://en.wikipedia.org/wiki/Chorded_keyboard) (although I do use some chording on my current keyboard). However, I have found some tools and ideas that I love to use and would love to share.

## Table of Contents

[Kyria keyboard](#kyria-keyboard)
[QMK](#qmk)
[Neovim](#neovim)
[Yabai with skhd](#yabai-with-skhd)
[Tmux](#tmux)

## [Kyria keyboard](https://blog.splitkb.com/introducing-the-kyria/)

The kyria keyboard is a custom keyboard sold by splitkb.com in parts for you to assemble. It has multiple modifications to the classic keyboard that I like for ergonomics.

- Split board: This allows you to adjust the two halves of the keyboard to be more in line with your shoulders.
- Column Staggered: On a regular keyboard, the keys align in rows but the rows stagger so the columns do not align. `A`, `S`, `D`, and `F` are all parallel but `Q`, `A`, and `Z` are not. The kyria reverses this, so that each finger follows its column. Look at your hand and notice how each finger is a different length. This column stagger makes resting your fingers on the home-row of your keyboard more comfortable, and your finger simply extends or retracts to hit keys up and down the column.
- Thumb keys: I realized at some point in both gaming and typing, my thumb mostly stayed on space. Compare this to the index finger which I had pressing 8 different keys! The pinky, the weakest finger also covered about 8 keys. Where is the justice in that?! The kyria lets your have all the keys the thumb deserves.
- [QMK](#qmk)

## QMK

You may have noticed, there are other things different with the kyria compared to a regular keyboard. Things are missing... Many things. How do you type numbers on this thing?

The kyria keyboard layout is completely customizable with a tool called [QMK](https://docs.qmk.fm/#/) (quantum mechanical keyboard). This means the output from pressing any key on it is customizable. This customization is not limited to changing pressing `A` to outputting `1`. It is much more powerful than that.

For example, the key that you would typically find at `D` when pressed on my Kyria outputs the following:

- Tap key: `t`
- Hold key: `T`
- Tap while holding down the spacebar: `Down-arrow`
- Hold while holding down the spacebaer: `Repeats down-arrow`
- Tap while holding NUM (number) layer key: `4`
- Tap while holding FUNC (function) layer key: `F4`
- Tap while holding SHRT (shortcut) layer key: `CMD + D`
- Much more depending on other combinations!

I could go on and on about all the customizations I have done. However, they are almost all inspired from [this blog post by Jonas Hietala](https://www.jonashietala.se/series/t-34/). I also copied some of his code for implementing functions such as the _repeater key_.

## Neovim

All of this customization from QMK just built my craving to use the keyboard as much as possible. One of the biggest annoyances I had previously working as an engineer was swapping between my keyboard and mouse constantly while working between spreadsheets and drawing in AutoCAD.

I realized I could avoid swapping as much as possible

## Yabai with skhd

## Tmux
