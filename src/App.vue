<script setup>
// This starter template is using Vue 3 <script setup> SFCs
// Check out https://vuejs.org/api/sfc-script-setup.html#script-setup
import HelloWorld from './components/HelloWorld.vue'
</script>

<template>
  <header class="text-gray-900 text-sm font-semibold">
    <nav class="bg-gray-900  px-8 py-3 flex items-center justify-between text-gray-50">
      <div class="flex items-center space-x-3">
        <!-- logo -->
        <a href="javascript:void(0)" class="hover:text-gray-400">
          <svg class="w-[32px] h-[32px] fill-current" aria-hidden="true" viewBox="0 0 16 16" data-view-component="true"><path fill-rule="evenodd" d="M8 0C3.58 0 0 3.58 0 8c0 3.54 2.29 6.53 5.47 7.59.4.07.55-.17.55-.38 0-.19-.01-.82-.01-1.49-2.01.37-2.53-.49-2.69-.94-.09-.23-.48-.94-.82-1.13-.28-.15-.68-.52-.01-.53.63-.01 1.08.58 1.23.82.72 1.21 1.87.87 2.33.66.07-.52.28-.87.51-1.07-1.78-.2-3.64-.89-3.64-3.95 0-.87.31-1.59.82-2.15-.08-.2-.36-1.02.08-2.12 0 0 .67-.21 2.2.82.64-.18 1.32-.27 2-.27.68 0 1.36.09 2 .27 1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.92.08 2.12.51.56.82 1.27.82 2.15 0 3.07-1.87 3.75-3.65 3.95.29.25.54.73.54 1.48 0 1.07-.01 1.93-.01 2.2 0 .21.15.46.55.38A8.013 8.013 0 0016 8c0-4.42-3.58-8-8-8z"></path></svg>
        </a>
        <!-- search -->
        <div class="relative">
          <input type="text" class="rounded w-[272px] bg-transparent border border-gray-600 placeholder:text-gray-200 px-3 py-1 focus:outline-none" placeholder="Search or jump to...">
          <div class="absolute top-0 right-0 flex items-center h-full">
            <div class="text-xs text-gray-600 px-1 mr-1 border border-gray-600 rounded">/</div>
          </div>
        </div>
        <!-- nav items -->
        <ul class="flex items-center space-x-2">
          <li class="hover:text-gray-400">Pull Requests</li>
          <li class="hover:text-gray-400">Issues</li>
          <li class="hover:text-gray-400">Marketplace</li>
          <li class="hover:text-gray-400">Explore</li>
        </ul>
      </div>
      <div class="flex items-center space-x-3">
        <!-- notification -->
        <a href="javascript:void(0)" class="hover:text-gray-400 relative">
          <svg class="w-4 fill-current" aria-hidden="true" viewBox="0 0 16 16" version="1.1"  data-view-component="true"><path d="M8 16a2 2 0 001.985-1.75c.017-.137-.097-.25-.235-.25h-3.5c-.138 0-.252.113-.235.25A2 2 0 008 16z"></path><path fill-rule="evenodd" d="M8 1.5A3.5 3.5 0 004.5 5v2.947c0 .346-.102.683-.294.97l-1.703 2.556a.018.018 0 00-.003.01l.001.006c0 .002.002.004.004.006a.017.017 0 00.006.004l.007.001h10.964l.007-.001a.016.016 0 00.006-.004.016.016 0 00.004-.006l.001-.007a.017.017 0 00-.003-.01l-1.703-2.554a1.75 1.75 0 01-.294-.97V5A3.5 3.5 0 008 1.5zM3 5a5 5 0 0110 0v2.947c0 .05.015.098.042.139l1.703 2.555A1.518 1.518 0 0113.482 13H2.518a1.518 1.518 0 01-1.263-2.36l1.703-2.554A.25.25 0 003 7.947V5z"></path></svg>
          <div class="bg-blue-600 w-2 h-2 rounded-full absolute top-0 right-0"></div>
        </a>
        <!-- create New -->
        <a href="javascript:void(0)" class="hover:text-gray-400 flex items-center">
            <svg class="w-4 fill-current" aria-hidden="true" viewBox="0 0 16 16" data-view-component="true">
              <path fill-rule="evenodd" d="M7.75 2a.75.75 0 01.75.75V7h4.25a.75.75 0 110 1.5H8.5v4.25a.75.75 0 11-1.5 0V8.5H2.75a.75.75 0 010-1.5H7V2.75A.75.75 0 017.75 2z"></path>
          </svg>

          <svg class="w-3 fill-current" viewBox="0 0 24 24">
            <path d="M6.1018 8C5.02785 8 4.45387 9.2649 5.16108 10.0731L10.6829 16.3838C11.3801 17.1806 12.6197 17.1806 13.3169 16.3838L18.8388 10.0731C19.5459 9.2649 18.972 8 17.898 8H6.1018Z"/>
          </svg>
        </a>

        <a href="javascript:void(0)" class="flex items-center">
          <img class="w-[20px] h-[20px] rounded-full" src="https://avatars.githubusercontent.com/u/20299519?s=96&v=4" alt="My Avatar">
          <!-- caret down -->
          <svg class="w-3 fill-current" viewBox="0 0 24 24">
            <path d="M6.1018 8C5.02785 8 4.45387 9.2649 5.16108 10.0731L10.6829 16.3838C11.3801 17.1806 12.6197 17.1806 13.3169 16.3838L18.8388 10.0731C19.5459 9.2649 18.972 8 17.898 8H6.1018Z"/>
          </svg>
        </a>
      </div>
    </nav>
    <div class="flex items-center justify-between px-8 py-3">
      <h2 class="flex items-center space-x-2">
        <svg class="w-[16px] fill-gray-500" aria-hidden="true"  viewBox="0 0 16 16" data-view-component="true">
            <path fill-rule="evenodd" d="M2 2.5A2.5 2.5 0 014.5 0h8.75a.75.75 0 01.75.75v12.5a.75.75 0 01-.75.75h-2.5a.75.75 0 110-1.5h1.75v-2h-8a1 1 0 00-.714 1.7.75.75 0 01-1.072 1.05A2.495 2.495 0 012 11.5v-9zm10.5-1V9h-8c-.356 0-.694.074-1 .208V2.5a1 1 0 011-1h8zM5 12.25v3.25a.25.25 0 00.4.2l1.45-1.087a.25.25 0 01.3 0L8.6 15.7a.25.25 0 00.4-.2v-3.25a.25.25 0 00-.25-.25h-3.5a.25.25 0 00-.25.25z"></path>
        </svg>
        <span class="text-lg text-blue-500 font-normal">
          <a href="javascript:void(0)">CodeCures</a>/
          <a href="javascript:void(0)" class="font-bold">github-clone</a>
        </span>
        <span class="border border-gray-400 text-gray-500 rounded-full px-1 text-xs py-0 font-normal">Public</span>
      </h2>
      <div class="flex items-center space-x-2">
        <!-- watch -->
        <button class="border px-2 py-0.5 border-gray-300 text-gray-700 text-[12px] font-semibold rounded-md flex items-center space-x-1">
            <svg class="w-4 fill-current" aria-hidden="true" viewBox="0 0 16 16" data-view-component="true">
              <path fill-rule="evenodd" d="M1.679 7.932c.412-.621 1.242-1.75 2.366-2.717C5.175 4.242 6.527 3.5 8 3.5c1.473 0 2.824.742 3.955 1.715 1.124.967 1.954 2.096 2.366 2.717a.119.119 0 010 .136c-.412.621-1.242 1.75-2.366 2.717C10.825 11.758 9.473 12.5 8 12.5c-1.473 0-2.824-.742-3.955-1.715C2.92 9.818 2.09 8.69 1.679 8.068a.119.119 0 010-.136zM8 2c-1.981 0-3.67.992-4.933 2.078C1.797 5.169.88 6.423.43 7.1a1.619 1.619 0 000 1.798c.45.678 1.367 1.932 2.637 3.024C4.329 13.008 6.019 14 8 14c1.981 0 3.67-.992 4.933-2.078 1.27-1.091 2.187-2.345 2.637-3.023a1.619 1.619 0 000-1.798c-.45-.678-1.367-1.932-2.637-3.023C11.671 2.992 9.981 2 8 2zm0 8a2 2 0 100-4 2 2 0 000 4z"></path>
          </svg>
            <span>Watch</span>
            <span class="px-1 rounded-full bg-gray-200">346</span>
            <svg class="w-3 fill-current" viewBox="0 0 24 24">
              <path d="M6.1018 8C5.02785 8 4.45387 9.2649 5.16108 10.0731L10.6829 16.3838C11.3801 17.1806 12.6197 17.1806 13.3169 16.3838L18.8388 10.0731C19.5459 9.2649 18.972 8 17.898 8H6.1018Z"/>
            </svg>
          </button>

          <!-- fork -->
          <button class="border px-2 py-0.5 border-gray-300 text-gray-700 text-[12px] font-semibold rounded-md flex items-center space-x-1">
            <svg class="w-4 fill-current" aria-hidden="true" viewBox="0 0 16 16" data-view-component="true">
                <path fill-rule="evenodd" d="M5 3.25a.75.75 0 11-1.5 0 .75.75 0 011.5 0zm0 2.122a2.25 2.25 0 10-1.5 0v.878A2.25 2.25 0 005.75 8.5h1.5v2.128a2.251 2.251 0 101.5 0V8.5h1.5a2.25 2.25 0 002.25-2.25v-.878a2.25 2.25 0 10-1.5 0v.878a.75.75 0 01-.75.75h-4.5A.75.75 0 015 6.25v-.878zm3.75 7.378a.75.75 0 11-1.5 0 .75.75 0 011.5 0zm3-8.75a.75.75 0 100-1.5.75.75 0 000 1.5z"></path>
            </svg>
            <span>Fork</span>
            <span class="px-1 rounded-full bg-gray-200 font-xs">2.8k</span>
            <svg class="w-3 fill-current" viewBox="0 0 24 24">
              <path d="M6.1018 8C5.02785 8 4.45387 9.2649 5.16108 10.0731L10.6829 16.3838C11.3801 17.1806 12.6197 17.1806 13.3169 16.3838L18.8388 10.0731C19.5459 9.2649 18.972 8 17.898 8H6.1018Z"/>
            </svg>
          </button>
        
        <!-- Star -->
          <div class="flex items-center">
            <button class="border px-2 py-0.5 border-gray-300 text-gray-700 text-[12px] font-semibold rounded-md rounded-r-none flex items-center space-x-1">
            <svg class="w-4 fill-current" aria-hidden="true" viewBox="0 0 16 16" data-view-component="true">
              <path fill-rule="evenodd" d="M8 .25a.75.75 0 01.673.418l1.882 3.815 4.21.612a.75.75 0 01.416 1.279l-3.046 2.97.719 4.192a.75.75 0 01-1.088.791L8 12.347l-3.766 1.98a.75.75 0 01-1.088-.79l.72-4.194L.818 6.374a.75.75 0 01.416-1.28l4.21-.611L7.327.668A.75.75 0 018 .25zm0 2.445L6.615 5.5a.75.75 0 01-.564.41l-3.097.45 2.24 2.184a.75.75 0 01.216.664l-.528 3.084 2.769-1.456a.75.75 0 01.698 0l2.77 1.456-.53-3.084a.75.75 0 01.216-.664l2.24-2.183-3.096-.45a.75.75 0 01-.564-.41L8 2.694v.001z"></path>
          </svg>
            <span>Star</span>
            <span class="px-1 rounded-full bg-gray-200">57k</span>
          </button>
          <a href="javascript:void(0)" class="border border-l-0 border-gray-300 text-gray-700 px-2 py-1.5 text-[12px] font-semibold rounded-md rounded-l-none">
            <svg class="w-3 fill-current" viewBox="0 0 24 24">
              <path d="M6.1018 8C5.02785 8 4.45387 9.2649 5.16108 10.0731L10.6829 16.3838C11.3801 17.1806 12.6197 17.1806 13.3169 16.3838L18.8388 10.0731C19.5459 9.2649 18.972 8 17.898 8H6.1018Z"/>
            </svg>
          </a>
          </div>
      </div>
    </div>
  </header>
</template>

