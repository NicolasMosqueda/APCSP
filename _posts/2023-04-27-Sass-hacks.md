---
toc: true
layout: post
description: Guide to SASS Hacks
categories: [Week 28]
title: Guide to SASS Hacks
---

# Guide to SASS Hacks

<style>
body.dark {
  background-color: #212121;
  color: #fff;
}
button.theme-toggle {
  background-color: #4caf50;
  color: #fff;
  border: none;
  padding: 10px;
  border-radius: 5px;
  cursor: pointer;
}
</style>

<button class="theme-toggle" onclick="toggleTheme()">Switch Theme</button>

<script>
function toggleTheme() {
  const body = document.querySelector('body');
  body.classList.toggle('dark');
}
</script>


