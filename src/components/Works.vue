
<template>
<div id="work">
  <div class="tabs">
    <ul>
      <li v-bind:class="{ 'is-active': isActive == 'pictures' }"><a v-on:click="isActive = 'pictures'">Pictures</a></li>
      <li v-bind:class="{ 'is-active': isActive == 'music' }"><a v-on:click="isActive = 'music'">Music</a></li>
      <li v-bind:class="{ 'is-active': isActive == 'videos' }"><a v-on:click="isActive = 'videos'">Videos</a></li>
      <li v-bind:class="{ 'is-active': isActive == 'documents' }"><a v-on:click="isActive = 'documents'">Documents</a></li>
    </ul>
  </div>
  <div class="tab-contents">
    <div class="content" v-bind:class="{ 'is-active': isActive == 'pictures' }">
      Picture content
    </div>
    <div class="content" v-bind:class="{ 'is-active': isActive == 'music' }">
      Music content
    </div>
    <div class="content" v-bind:class="{ 'is-active': isActive == 'videos' }">
      Videos content
    </div>
    <div class="content" v-bind:class="{ 'is-active': isActive == 'documents' }">
      Documents content
    </div>
  </div>
</div>
</template>
<style>
.tab-contents .content {
  display: none;
}
.tab-contents .content.is-active {
  display: block;
}
</style>