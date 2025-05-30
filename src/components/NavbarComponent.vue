<template>
  <nav class="bg-gray-900 text-white py-4 px-8 flex justify-evenly items-center">
    <h1 class="text-lg font-bold">José Vitor</h1>
    <ul class="flex gap-6">
        <li>
          <button class="bg-sky-800 px-4 py-2 rounded hover:bg-cyan-900 transition-colors duration-700">
            <router-link to="/">Home</router-link>
          </button>
        </li>
        <li>
          <button class="bg-sky-800 px-4 py-2 rounded hover:bg-cyan-900 transition-colors duration-700">
            <router-link to="/about">Sobre</router-link>
          </button>
        </li>
        <li>
          <button class="bg-sky-800 px-4 py-2 rounded hover:bg-cyan-900 transition-colors duration-700">
            <router-link to="/contact">Contatos</router-link>
          </button>
        </li>
    </ul>
  </nav>
</template>
