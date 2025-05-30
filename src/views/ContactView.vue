<template>
  <section class="max-w-5xl mx-auto px-6 py-12">
    <h2 class="text-3xl font-bold text-center text-sky-700 mb-10">Entre em Contato</h2>

    <div class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 gap-8 text-center mb-12">
      <!-- GitHub -->
      <a
        href="https://github.com/ZezoDebug"
        target="_blank"
        class="bg-stone-400 rounded-xl p-6 shadow transition transform hover:-translate-y-2 hover:bg-gray-900 hover:text-white duration-300">
        <i class="fab fa-github text-4xl mb-4"></i>
        <h3 class="text-xl font-semibold">GitHub</h3>
        <p class="text-sm mt-2">Veja meus projetos e códigos.</p>
      </a>

      <!-- LinkedIn -->
      <a
        href="https://www.linkedin.com/in/josé-vitor-a-lima-890421270/"
        target="_blank"
        class="bg-stone-400 rounded-xl p-6 shadow transition transform hover:-translate-y-2 hover:bg-blue-600 hover:text-white duration-300">
        <i class="fab fa-linkedin text-4xl mb-4"></i>
        <h3 class="text-xl font-semibold">LinkedIn</h3>
        <p class="text-sm mt-2">Conecte-se comigo no LinkedIn.</p>
      </a>

      <!-- Email -->
      <a
        href="#"
        class="bg-stone-400 rounded-xl p-6 shadow transition transform hover:-translate-y-2 hover:bg-red-600 hover:text-white duration-300">
        <i class="fas fa-envelope text-4xl mb-4"></i>
        <h3 class="text-xl font-semibold">E-mail</h3>
        <p class="text-sm mt-2">Envie um e-mail direto para mim.</p>
      </a>
    </div>

    <!-- Formulário de sugestões -->
    <form class="bg-stone-400 p-8 rounded-xl shadow-md max-w-lg mx-auto space-y-6">
      <h3 class="text-2xl font-semibold mb-4 text-center text-gray-800">Envie suas sugestões</h3>

      <input
        type="text"
        placeholder="Seu nome"
        class="w-full border border-gray-300 p-3 rounded-md focus:outline-none focus:ring-2 focus:ring-cyan-600"/>

      <input
        type="email"
        placeholder="Seu e-mail"
        class="w-full border border-gray-300 p-3 rounded-md focus:outline-none focus:ring-2 focus:ring-cyan-600"/>

      <textarea
        placeholder="Sua sugestão ou mensagem"
        rows="5"
        class="w-full border border-gray-300 p-3 rounded-md focus:outline-none focus:ring-2 focus:ring-cyan-600 resize-none"></textarea>

      <button
        type="submit"
        class="w-full bg-cyan-700 hover:bg-cyan-800 text-white py-3 rounded-md transition-colors duration-300">
        Enviar sugestão
      </button>
    </form>
  </section>
</template>