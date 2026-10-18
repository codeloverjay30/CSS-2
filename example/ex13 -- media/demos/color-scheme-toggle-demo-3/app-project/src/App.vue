<script setup lang="js">
import { watchEffect  } from 'vue';
import { useRef } from 'react';
// https://stackoverflow.com/questions/56393880/how-do-i-detect-dark-mode-using-javascript

//var isDarkMode = window.matchMedia('(prefers-color-scheme: dark)').matches;

const props = defineProps({
    isDarkMode: Boolean,
});

props.isDarkMode = window.matchMedia('(prefers-color-scheme: dark)').matches;

function toggleColorMode() {
  props.isDarkMode = !isDarkMode;
  console.group('toggleColorMode');
  console.log('isDarkMode: '+(isDarkMode?'truthy':'falsey') + ' value.');
  console.groupEnd();
}

watchEffect(()=>{
  //console.group('isDarkMode');
  console.log('isDarkMode: '+(isDarkMode?'truthy':'falsey') + ' value.');
  //console.groupEnd();
});

</script>
<template>
        <div class="grid-container resize">
            <header>User Name</header>
            <main>
                <div class="msg">
                    <span>上午 12:52</span>
                    <p>Lorem, ipsum dolor.</p>
                </div>
                <div class="msg">
                    <span>上午 12:52</span>
                    <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Laborum doloremque tempora molestias repellat, ad unde reprehenderit, sint cumque libero quam similique reiciendis aperiam id aliquam, tempore earum nemo sequi recusandae.</p>
                </div>
                <div class="msg">
                    <span>上午 12:52</span>
                    <p>Lorem ipsum dolor sit amet.</p>
                </div>
                <div class="msg">
                    <span>上午 12:52</span>
                    <p>Lorem </p>
                </div>
                <div class="msg">
                    <span>上午 12:52</span>
                    <p>Lorem, ipsum dolor.</p>
                </div>
                <div class="msg">
                    <span>上午 12:52</span>
                    <p>Lorem </p>
                </div>
            </main>
            <footer>
                <textarea placeholder="輸入訊息"></textarea>
            </footer>
        </div>
        <button id="color-scheme-toggle" @click="toggleColorMode()">
            <span id="toggle-icon" class="material-icons">{{ (isDarkMode? 'dark':'light') + '_mode' }}</span>
            <span id="toggle-text">{{ 'Switch to ' + (isDarkMode ? 'Dark': 'Light') + ' mode '}}</span>
        </button>
</template>