<template>
  <div class="min-h-screen bg-gray-50">
    <!-- Sección Hero -->
    <section class="bg-gradient-to-r from-blue-600 to-purple-600 text-white py-20">
      <UContainer class="text-center">
        <h1 class="text-5xl font-bold mb-4">Plantilla Nuxt + Tauri</h1>
        <p class="text-xl mb-8 max-w-2xl mx-auto">
          Una plantilla moderna de aplicación web que combina Nuxt 4, Tauri y Nuxt UI
        </p>
        <div class="flex gap-4 justify-center">
          <UButton size="lg" color="white" variant="solid">
            Comenzar
          </UButton>
          <UButton size="lg" color="gray" variant="ghost">
            Documentación
          </UButton>
        </div>
      </UContainer>
    </section>

    <!-- Sección de Características -->
    <section class="py-16">
      <UContainer>
        <h2 class="text-3xl font-bold text-center mb-12 text-gray-800">Características Principales</h2>
        <div class="grid md:grid-cols-3 gap-8">
          <!-- Característica Nuxt -->
          <UCard>
            <template #header>
              <div class="flex items-center gap-2">
                <UIcon name="i-logos-nuxt-icon" class="w-6 h-6 text-green-500" />
                <h3 class="text-xl font-semibold">Nuxt 4</h3>
              </div>
            </template>
            <p class="text-gray-600">
              Última versión de Nuxt con Vue 3, enrutamiento basado en archivos y potentes convenciones
            </p>
          </UCard>

          <!-- Característica Tauri -->
          <UCard>
            <template #header>
              <div class="flex items-center gap-2">
                <UIcon name="i-logos-tauri" class="w-6 h-6 text-orange-500" />
                <h3 class="text-xl font-semibold">Tauri</h3>
              </div>
            </template>
            <p class="text-gray-600">
              Construye aplicaciones de escritorio seguras con backend en Rust y tamaño de binario mínimo
            </p>
          </UCard>

          <!-- Característica Nuxt UI -->
          <UCard>
            <template #header>
              <div class="flex items-center gap-2">
                <UIcon name="i-heroicons-paint-brush" class="w-6 h-6 text-blue-500" />
                <h3 class="text-xl font-semibold">Nuxt UI</h3>
              </div>
            </template>
            <p class="text-gray-600">
              Hermosos componentes de UI responsivos construidos con Tailwind CSS
            </p>
          </UCard>
        </div>
      </UContainer>
    </section>

    <!-- Stack Tecnológico -->
    <section class="bg-white py-16">
      <UContainer>
        <h2 class="text-3xl font-bold text-center mb-12 text-gray-800">Stack Tecnológico</h2>
        <div class="flex flex-wrap justify-center gap-4">
          <UBadge variant="subtle" size="lg" color="green">
            <UIcon name="i-logos-nuxt-icon" class="w-4 h-4 mr-1" />
            Nuxt 4
          </UBadge>
          <UBadge variant="subtle" size="lg" color="orange">
            <UIcon name="i-logos-tauri" class="w-4 h-4 mr-1" />
            Tauri
          </UBadge>
          <UBadge variant="subtle" size="lg" color="blue">
            <UIcon name="i-logos-vue" class="w-4 h-4 mr-1" />
            Vue 3
          </UBadge>
          <UBadge variant="subtle" size="lg" color="cyan">
            <UIcon name="i-logos-tailwindcss-icon" class="w-4 h-4 mr-1" />
            Tailwind CSS
          </UBadge>
          <UBadge variant="subtle" size="lg" color="red">
            <UIcon name="i-logos-rust" class="w-4 h-4 mr-1" />
            Rust
          </UBadge>
        </div>
      </UContainer>
    </section>

    <!-- Comenzar -->
    <section class="py-16">
      <UContainer>
        <h2 class="text-3xl font-bold text-center mb-12 text-gray-800">Cómo Comenzar</h2>
        <div class="max-w-3xl mx-auto">
          <UAlert title="Instalación" color="blue" variant="soft" class="mb-6">
            <template #description>
              <p>Instala las dependencias e inicia el servidor de desarrollo:</p>
              <pre class="bg-gray-100 p-3 rounded mt-2 overflow-x-auto">pnpm install
pnpm tauri dev</pre>
            </template>
          </UAlert>

          <UAlert title="Compilar para Producción" color="green" variant="soft" class="mb-6">
            <template #description>
              <p>Crea una compilación para producción y ejecútala:</p>
              <pre class="bg-gray-100 p-3 rounded mt-2 overflow-x-auto">pnpm build
pnpm tauri build</pre>
            </template>
          </UAlert>

          <UAlert title="Aprende Más" color="purple" variant="soft">
            <template #description>
              <p>Consulta la documentación para más detalles:</p>
              <ul class="list-disc list-inside mt-2 space-y-1">
                <li><a href="https://nuxt.com/docs" class="text-blue-600 hover:underline">Documentación de Nuxt</a></li>
                <li><a href="https://tauri.app/v1/guides/" class="text-blue-600 hover:underline">Guías de Tauri</a></li>
                <li><a href="https://ui.nuxt.com/" class="text-blue-600 hover:underline">Componentes Nuxt UI</a></li>
              </ul>
            </template>
          </UAlert>
        </div>
      </UContainer>
    </section>

    <!-- Pie de página -->
    <footer class="bg-gray-800 text-white py-8">
      <UContainer class="text-center">
        <p class="mb-2">Plantilla Nuxt + Tauri</p>
        <p class="text-sm text-gray-400">
          Construido con ❤️ usando Nuxt 4, Tauri y Nuxt UI
        </p>
      </UContainer>
    </footer>
  </div>
</template>