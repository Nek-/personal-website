---
title: Gangbowl
date: 2018-09-14 02:00:00 +0200
categories: []
description: Gangbowl is a game I'm working on. Challenges are physics and realtime
  playing.
banner_image: "/uploads/COVER  _Social media.jpg"
sub_heading: A soccer game
tags: []
slug: ''

---
# Gangbowl

_Friends and me like so much the game Haxball, but this game suffer of_ insufficient _investment by its creator (no fun stuff, complicated UI, lag...). That's why we decided to make a concurrent that get rid of this drawbacks._

I don't want to spoil too much on this game we're working on. So I will just expose some points which are interesting to know about technologies we use and/or tried.

## What front-end tools ?

* Typescript: no discussions. We hate JavaScript, so we love TypeScript. I let you see their [official website](https://www.typescriptlang.org/) and [try it](https://www.typescriptlang.org/play/index.html) to convince yourself about the benefices of TypeScript.
* Pixi.js & Box2d: pixi is a nice wrapper for canvasjs features and Box2d is probably the best physic engine for 2d stuff. Speaking of Box2d, we are using the awesome work of flyover: [https://github.com/flyover/box2d.ts](https://github.com/flyover/box2d.ts "https://github.com/flyover/box2d.ts")
* Angular: it's coded in TypeScript, it's opensource and maintained, we know how it work and it's not bad... I guess it's a good choice.

**What we test**

* Phaser: considering the code quality and the poor maintainance strategy of Phaser, I strongly disagree on using it at first gland. But we were new at games. Using Phaser was an easy step. And it was working! But we had to drop it because of its hardcoded methods and because of our part related to networking (Phaser will be better at single player games).
* Unity: this was looking great, but expensive for server features ! It also comes with 300MB to load in the browser before your code. When we currently have 100KB to load.