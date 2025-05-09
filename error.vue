<template>
    <NuxtLayout name="404">
      <main class="min-h-screen flex items-center justify-center 
        bg-gray-100 dark:bg-black 
        bg-[radial-gradient(rgba(0,0,0,0.15)_1px,transparent_1px)] 
        dark:bg-[radial-gradient(rgba(255,255,255,0.10)_1px,transparent_1px)] 
        bg-[size:22px_22px] bg-repeat bg-fixed">
        <div class="text-center">
          <h1 class="text-6xl sm:text-8xl font-bold text-primary-500 mb-4">404</h1>
          <h2 class="text-2xl sm:text-3xl font-semibold text-gray-800 dark:text-gray-200 mb-6">
            Oups ! Page non trouvée
          </h2>
          <p class="text-gray-600 dark:text-gray-400 mb-8 max-w-md mx-auto">
            Désolé, la page que vous recherchez n'existe pas ou a été déplacée.
          </p>
          <NuxtLink 
            to="/"
            class="inline-block px-6 py-3 bg-primary-500 text-white rounded-lg hover:bg-primary-600 transition-colors duration-300"
          >
            Retour à l'accueil
          </NuxtLink>
        </div>
      </main>
    </NuxtLayout>
  </template>
  
  <script setup lang="ts">
  const config = useRuntimeConfig();
  const description = "La page que vous recherchez n'existe pas ou a été déplacée.";
  
  useSeoMeta({
    title: "404 Not Found",
    description,
  });
  </script>