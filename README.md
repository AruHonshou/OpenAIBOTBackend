# 🤖 OpenAI BOT — Backend

> API REST construida con NestJS y TypeScript que actúa como intermediario entre el frontend y la API de OpenAI.

---

## 📋 Tabla de Contenidos

- [Descripción](#-descripción)
- [Stack Tecnológico](#-stack-tecnológico)
- [Requisitos Previos](#-requisitos-previos)
- [Instalación](#-instalación)
- [Configuración](#-configuración)
- [Uso](#-uso)
- [Estructura del Proyecto](#-estructura-del-proyecto)
- [Scripts Disponibles](#-scripts-disponibles)

---

## 📖 Descripción

**OpenAI BOT Backend** es el servidor que gestiona las peticiones del frontend, se comunica con la API de OpenAI y devuelve las respuestas del chatbot. Está construido sobre **NestJS**, un framework de Node.js orientado a módulos que facilita el desarrollo de APIs escalables y mantenibles.

---

## 🛠 Stack Tecnológico

| Tecnología | Descripción |
|---|---|
| [NestJS](https://nestjs.com/) | Framework principal del servidor |
| [TypeScript](https://www.typescriptlang.org/) | Tipado estático |
| [Node.js](https://nodejs.org/) | Entorno de ejecución |
| [ESLint](https://eslint.org/) + [Prettier](https://prettier.io/) | Linting y formateo de código |

---

## ✅ Requisitos Previos

- **Node.js** v18 o superior
- **npm** v9 o superior
- Una **API Key de OpenAI** activa

---

## 🚀 Instalación

1. Clona el repositorio:

```bash
git clone https://github.com/AruHonshou/OpenAIBOTBackend.git
cd OpenAIBOTBackend
```

2. Instala las dependencias:

```bash
npm install -f
```

---

## ⚙️ Configuración

1. Copia el archivo de variables de entorno:

```bash
cp .env.template .env
```

2. Edita el `.env` con tus credenciales:

```env
OPENAI_API_KEY=tu_api_key_aqui
PORT=3000
```

> ⚠️ **Nunca subas tu `.env` al repositorio.** Está incluido en `.gitignore` por defecto.

---

## 💻 Uso

### Modo desarrollo (con hot-reload)

```bash
npm run start:dev
```

El servidor estará disponible en [http://localhost:3000](http://localhost:3000).

### Modo producción

```bash
npm run build
npm run start:prod
```

---

## 📁 Estructura del Proyecto

```
OpenAIBOTBackend/
├── .vscode/              # Configuración del editor
├── generated/            # Archivos generados automáticamente
├── src/                  # Código fuente principal
│   ├── app.module.ts     # Módulo raíz de NestJS
│   └── main.ts           # Punto de entrada del servidor
├── .env.template         # Plantilla de variables de entorno
├── .eslintrc.js          # Configuración de ESLint
├── .prettierrc           # Configuración de Prettier
├── nest-cli.json         # Configuración del CLI de NestJS
├── package.json          # Dependencias y scripts
├── tsconfig.json         # Configuración de TypeScript
└── tsconfig.build.json   # Configuración de TypeScript para build
```

---

## 📜 Scripts Disponibles

| Script | Descripción |
|---|---|
| `npm run start:dev` | Inicia el servidor en modo desarrollo con hot-reload |
| `npm run start:prod` | Inicia el servidor en modo producción |
| `npm run build` | Compila el proyecto TypeScript |
| `npm run lint` | Ejecuta ESLint sobre el código fuente |
| `npm run format` | Formatea el código con Prettier |

---

## 👤 Autor

**AruHonshou**  
GitHub: [@AruHonshou](https://github.com/AruHonshou)
