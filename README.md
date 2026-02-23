# Plantilla Nuxt + Tauri 🚀

Una plantilla moderna para aplicaciones de escritorio que combina lo mejor de **Nuxt 4**, **Tauri** y **Nuxt UI**. Perfecta para crear aplicaciones rápidas, seguras y con interfaz profesional.

## 🎯 Características

✅ **Nuxt 4** - Última versión con Vue 3, enrutamiento basado en archivos y potentes convenciones
✅ **Tauri** - Aplicaciones de escritorio seguras con backend en Rust y tamaño mínimo
✅ **Nuxt UI** - Componentes de interfaz profesionales y responsivos
✅ **Tailwind CSS** - Estilos modernos y personalizables
✅ **Vite** - Compilación rápida y desarrollo ágil
✅ **TypeScript** - Soporte completo para tipado estático

## 🛠 Requisitos Previos

Asegúrate de tener instalado:

- Node.js (v18+ recomendado)
- pnpm (recomendado) o npm/yarn
- Rust (para Tauri)
- Tauri CLI

## 🚀 Instalación

1. Clona este repositorio:

```bash
git clone https://github.com/SpicyDogWings/Nuxtri.git
cd Nuxtri
```

2. Instala las dependencias:

```bash
# Con pnpm (recomendado)
pnpm install
```

## 📱 Desarrollo

Inicia el servidor de desarrollo con Tauri:

```bash
# Desarrollo web + escritorio
pnpm tauri dev
```

El servidor se iniciará en:
- **Web**: `http://localhost:3000`
- **Desktop**: Ventana de Tauri

## 🔨 Compilación para Producción

### Compilar aplicación de escritorio:

```bash
# Compilar aplicación Tauri
pnpm tauri build
```

Los binarios se generarán en `src-tauri/target/release/`

## 📦 Estructura del Proyecto

```
nuxt-tauri-template/
├── app/                  # Código de Nuxt (frontend)
│   ├── app.vue          # Landing page principal
│   └── assets/          # Recursos estáticos
├── src-tauri/            # Código de Tauri (backend Rust)
│   ├── src/             # Código Rust
│   └── tauri.conf.json  # Configuración de Tauri
├── public/              # Archivos públicos
├── package.json         # Dependencias de Node.js
└── README.md             # Este archivo
```

## 🎨 Personalización

### Cambiar el nombre de la aplicación:

1. Edita `package.json`:
```json
{
  "name": "mi-nueva-app",
  "version": "1.0.0"
}
```

2. Edita `src-tauri/tauri.conf.json`:
```json
{
  "package": {
    "productName": "MiNuevaApp",
    "version": "1.0.0"
  }
}
```

### Cambiar la landing page:

Edita `app/app.vue` para modificar el contenido de la página principal.

## 📚 Documentación

- [Documentación de Nuxt](https://nuxt.com/docs)
- [Guías de Tauri](https://tauri.app/v1/guides/)
- [Componentes Nuxt UI](https://ui.nuxt.com/)
- [Tailwind CSS](https://tailwindcss.com/docs)

## 🤝 Contribución

No soportadas por el momento

## 📜 Licencia

MIT License - Usa este template libremente para tus proyectos personales y comerciales.

---

**¡Gracias por usar esta plantilla!** 🚀
