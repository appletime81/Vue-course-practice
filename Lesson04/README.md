初始化工程大改造
===============

## 知识点

* 初始化工程大改造

## 实战演习/说明讲解

>画面演示

+ 初始化工程结构一览
+ 初始化工程大改造

## 操作步骤

### 初始化工程结构一览

+ src
  - App.vue
  - assets
  - components
  - main.js
  - router
  - stores
  - views

### 初始化工程大改造(简化工程)

*删除*

+ components/icons
+ components/HelloWorld.vue
+ components/TheWelcome.vue
+ components/WelcomeItem.vue

*修改*

+ views/AboutView.vue
+ views/HomeView.vue
+ App.vue

__views/AboutView.vue__

```js
<template>
  <div class="about">
    <h1>关于页面</h1>
  </div>
</template>

<style>
@media (min-width: 1024px) {
  .about {
    min-height: 100vh;
    display: flex;
    align-items: center;
  }
}
</style>
```

__views/HomeView.vue__

```js
<script setup>
</script>

<template>
  <main>
    <h1>欢迎来到 Vue3 世界.</h1>
  </main>
</template>
```

__App.vue__

```html
<script setup>
import { RouterLink, RouterView } from 'vue-router'
</script>

<template>
  <header>
    <div class="wrapper">
      <nav>
        <RouterLink to="/">主页</RouterLink>
        <RouterLink to="/about">关于</RouterLink>
      </nav>
    </div>
  </header>

  <RouterView />
</template>

<style scoped>
header {
  line-height: 1.5;
  max-height: 100vh;
}

nav {
  width: 100%;
  font-size: 14px;
  text-align: center;
}

nav a.router-link-exact-active {
  color: var(--color-text);
}

nav a.router-link-exact-active:hover {
  background-color: transparent;
}

nav a {
  display: inline-block;
  padding: 0 1rem;
  border-left: 1px solid var(--color-border);
}

nav a:first-of-type {
  border: 0;
}
</style>
```

## 小马部落

https://discord.gg/VSKw72P

## 课程文件

+ 小马部落Discord专区共享(四级会员)

## 小马视频频道

https://komavideo.com

## 深学AWS

https://deeplearnaws.com

## 深学Azure

https://deeplearnazure.com/

## 深学GCP

https://deeplearngcp.com/

## Youtube

https://youtube.com/@deeplearncloud

