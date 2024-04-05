<template>
  <div class="intro-y flex flex-col sm:flex-row items-center mt-8">
    <i class="fas fa-mouse-pointer fa-lg text-xl mr-2"></i>
    <!-- <i class="fa-sharp fa-solid fa-square-arrow-up-left"></i> -->
  <div>
    <h2 class="text-lg font-medium mr-auto">ChatBot Settings</h2>
    <h1 class="text-sm font-medium mr-auto">Setup your Chatbox below</h1>
  </div>
</div>

<div class="intro-y chat grid grid-cols-12 gap-5 mt-5">
  <!-- BEGIN: Chat Side Menu -->
  <TabGroup class="col-span-12 lg:col-span-12 2xl:col-span-12">
    <div class="intro-y pr-1">
      <div class="box p-2">
        <TabList class="nav-pills">
          <Tab class="w-full py-2" tag="button">Chats</Tab>
          <Tab class="w-full py-2" tag="button">Friends</Tab>
          <Tab class="w-full py-2" tag="button">Profile</Tab>
        </TabList>
      </div>
    </div>
  </TabGroup>
</div>

<div class="intro-y flex flex-col sm:flex-row items-center mt-8">
  <div>
    <h2 class="text-sm font-medium mr-auto">ChatBot Setup</h2>
    <!-- Radio buttons -->
    <div class="mt-2 space-y-2">
      <div class="flex items-center mt-4">
        <input type="radio" id="option1" name="options" value="option1" class="form-radio h-5  w-5 text-indigo-600">
        <label for="option1" class="ml-2 mx-5">Use Instructions</label>
      
        <input type="radio" id="option2" name="options" value="option2" class="form-radio h-5 w-5 text-indigo-600">
        <label for="option2" class="ml-2">Use Existing Assistant</label>
      </div>
    </div>
  </div>
</div>
<!-- dropdowns start here-->
<div class="flex flex-col mt-6">
  <div class="flex w-full">
    <label for="gptAccount" class="mb-2 w-1/2">Select GPT Account</label>
    <label for="gptModel" class="w-1/2 ml-6">Choose GPT Model</label>
  </div>
  <div class="flex">
    <select id="gptAccount" class="form-select mr-4">
      <option>Select Account</option>
      <option>Option 1</option>
      <option>Option 2</option>
      <option>Option 3</option>
    </select>

    
    <select id="gptModel" class="form-select ml-2">
      <!-- Options for the GPT Model dropdown -->
    </select>
  </div>
</div>
<div class="flex flex-col mt-6">
  <label for="chatBox" class="mb-2">ChatBot Headline</label>
  <input type="text" id="chatBox" class="form-input w-full">
</div>

<div class="flex flex-col mt-6">
  <label for="chatBox" class="mb-2">Greeting Text</label>
  <input type="text" id="chatBox" class="form-input w-full">
</div>

<div class="flex flex-col mt-6">
  <label for="chatBox" class="mb-2">User Input Placeholder</label>
  <input type="text" id="chatBox" class="form-input w-full">
</div>

<div class="flex flex-col mt-6">
  <label for="chatBox" class="mb-2">Disclosure Message</label>
  <input type="text" id="chatBox" class="form-input w-full" value="This is an automated chatbot response. (Learn More)">
</div>

<!--Last buttons on the page here-->

<div class="flex justify-end mt-6">
  <button class="btn btn-secondary mr-4">Cancel</button>
  <button class="btn btn-primary">Save Settings</button>
</div>
</template>

<script setup>
import { ref } from "vue";

const chatBox = ref(false);
const showChatBox = () => {
  chatBox.value = !chatBox.value;
};
</script>
