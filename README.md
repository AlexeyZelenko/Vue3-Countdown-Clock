<snippet>
  <content>
  
##  [Vue3-Countdown-Clock]() with Vue3.

<p align="center">
    <a href="https://www.npmjs.com/package/vue-button-up">
      <img alt="codebeat badge" src="https://img.shields.io/badge/version-1.0.5%20-44cc11.svg" />
    </a>
    <a href="https://www.npmjs.com/package/tiptap-vuetify">
      <img alt="codebeat badge" src="https://img.shields.io/badge/license-ISC%20-44cc11.svg" />
    </a>
    <a href="https://standardjs.com/">
      <img alt="codebeat badge" src="https://badgen.net/badge/code%20style/standard/f2a" />
    </a>
    <a href="https://www.npmjs.com/package/tiptap-vuetify">
      <img alt="codebeat badge" src="https://img.shields.io/badge/size-15%20kB-44cc11.svg" />
    </a>
  </p>
  
  Button with the functionality of scrolling the page up for Vue.
  [DEMO on codesanbox]()
  
  ## Navigation  
  <!-- TOC -->
  
  - [Features](#features)
  - [Installation](#installation)
  - [Usage](#Usage)
  <!-- /TOC -->
  
  ## Features
  
  - used vue3
  - easy to install
  - Easy application
  - Using provide, inject, ref
  - Ability to customize your own styles
  - Ability to customize your own time zone
  - Ability to customize your own language
  - Ability to customize the end time
  - Completion message
  - TS
 
  
  ## Installation
  
    ```
     npm install --save vue3-countdown-clock
    ```

## Usage
 #default
```
<template>
    <Vue3CountdownClock/>
<template/>


 <script lang="ts">
 import { defineComponent, ref, provide } from '@vue/composition-api'
 import Vue3CountdownClock from 'vue3-countdown-clock'
 
 export default defineComponent({
   name: 'HelloWorld',
   components: {
     Vue3CountdownClock
   },
   setup () {
     const deadLine = ref('2020/12/06 10:00:00 GMT-0200')
     provide('deadline', deadLine)
 
     const Title = ref('Online service will be honored through:')
     provide('title', Title)
 
     const timerStyle = ref({
       'text-align': 'center',
       'font-family': 'sans-serif',
       'font-weight': 100
     })
     provide('timerStyle', timerStyle)
 
     const h1Style = ref({
       color: '#396',
       'font-weight': 100,
       'font-size': '40px',
       margin: '40px 0px 20px'
     })
     provide('h1Style', h1Style)
 
     const clockdiv = ref({
       'font-family': 'sans-serif',
       color: '#fff',
       display: 'inline-block',
       'font-weight': 100,
       'text-align': 'center',
       'font-size': '30px'
     })
     provide('clockdiv', clockdiv)
 
     const clockdivDiv = ref({
       padding: '10px',
       'border-radius': '3px',
       background: '#00BF96',
       display: 'inline-block',
       margin: '1px'
     })
     provide('clockdivDiv', clockdivDiv)
 
     const clockdivDivSpan = ref({
       padding: '15px',
       'border-radius': '3px',
       background: '#00816A',
       display: 'inline-block'
     })
     provide('clockdivDivSpan', clockdivDivSpan)
 
     const styleEndTime = ref({
       color: '#fff'
     })
     provide('styleEndTime', styleEndTime)
 
     const smalltext = ref({
       'padding-top': '5px',
       'font-size': '16px'
     })
     provide('smalltext', smalltext)
 
     const titleDays = ref('Days')
     provide('titleDays', titleDays)
 
     const titleHours = ref('Hours')
     provide('titleHours', titleHours)
 
     const titleMinutes = ref('Minutes')
     provide('titleMinutes', titleMinutes)
 
     const titleSeconds = ref('Seconds')
     provide('titleSeconds', titleSeconds)
 
     const titleEndTime = ref('End Time!')
     provide('titleEndTime', titleEndTime)
   }
 })
 </script>
```
#description
Enter your date and time zone
```
const deadLine = ref('2020/12/06 10:00:00 GMT-0200')
     provide('deadline', deadLine)
```

Change styles

timerStyle, h1Style, clockdiv, clockdivDiv, clockdivDivSpan, styleEndTime, smalltext  
```
const timerStyle = ref({
       'text-align': 'center',
       'font-family': 'sans-serif',
       'font-weight': 100
     })
     provide('timerStyle', timerStyle)
...
```
Change the names

Days, Hours, Minutes, Seconds, End Time!

```
const Title = ref('Online service will be honored through:')
     provide('title', Title)
```
change to...
```
const Title = ref('在线服务将通过以下方式兑现:')
     provide('title', Title)
```
...
```
const titleDays = ref('Days')
     provide('titleDays', titleDays)
```
...





#Donate (creating code at your request out of turn)
💰 I can do some feature for you out of turn and at a fast pace or solve your problem, give a quick answers. To do this, you can pay me one-time or make a subscription. We can discuss the details by email, it is written in my profile.
></content>
><tabTrigger>readme</tabTrigger>
</snippet>