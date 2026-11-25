# Hola 👋, soy Lucas Haberles

**Desarrollador Full Stack · Web y Mobile** · Corrientes, Argentina 🇦🇷

Construyo sistemas de gestión y apps móviles de punta a punta: frontend, backend, base de datos y publicación. Me gusta resolver problemas reales con software que funcione donde la gente lo necesita, aunque no haya señal.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-lucas--haberles-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://linkedin.com/in/lucas-haberles)
[![Email](https://img.shields.io/badge/Email-haberleslucas.unne%40gmail.com-EA4335?style=flat-square&logo=gmail&logoColor=white)](mailto:haberleslucas.unne@gmail.com)

---

## 💼 Actualmente

- 🏛️ **Desarrollador de Software** en la Contaduría General de la Provincia de Corrientes (Ministerio de Hacienda), desde febrero de 2026.
  - Desarrollo desde cero de un módulo del **SIIF** para digitalizar Órdenes de Provisión y Actas de Recepción: análisis, diseño e implementación con **Angular, Node.js y PL/SQL**.
  - Antes, en el mismo sistema: módulo de notificaciones por correo a usuarios externos con **Java, PL/SQL y Angular**.
- 🎓 Terminando la **Licenciatura en Sistemas de Información** (UNNE, ~90 % de avance).
- 🤝 Abierto a propuestas de desarrollo **full stack** y **mobile**.

---

## 🚀 Proyecto destacado

### 🐄 Rumbeador — gestión ganadera offline-first

App Android y panel web para productores ganaderos argentinos (dueños de estancias, encargados y veterinarios). La hice de punta a punta: app, backend, panel web, reglas de seguridad, publicación en Google Play y marca.

<!-- TODO: reemplazar por el link cuando la app esté publicada -->
<!-- [![Google Play](https://img.shields.io/badge/Google_Play-Descargar-414141?style=flat-square&logo=googleplay&logoColor=white)](LINK_DE_GOOGLE_PLAY) -->

<!-- TODO: capturas. Tres en fila quedan bien en el perfil:
<p align="center">
  <img src="URL_CAPTURA_1" alt="Recuento por potrero" width="230"/>
  <img src="URL_CAPTURA_2" alt="Decilo con tus palabras" width="230"/>
  <img src="URL_CAPTURA_3" alt="Ficha del animal" width="230"/>
</p>
-->

**Lo interesante en lo técnico**

- **Offline-first de verdad.** En el campo casi nunca hay cobertura, así que SQLite es la fuente de verdad: migraciones versionadas, triggers que marcan cambios pendientes, borrado lógico y sincronización incremental con Firestore (los conflictos se resuelven con "última edición gana").
- **Dictado sin IA ni internet.** El usuario dice *"vacuné con aftosa a las vacas del Bajo"* y la app arma el evento. Parser por reglas propias, tolerante a errores de dictado con comparación fonética y distancia de edición.
- **Trámites rurales resueltos.** Controles previos a la guía de ganado y el DTe (retiro sanitario, caravana electrónica, aftosa, título de marca) con los datos listos para copiar en los sistemas oficiales, y la manifestación anual de Rentas Corrientes calculada desde los datos, con control contra el año anterior y PDF de una hoja.
- **Eventos que actualizan la ficha solos.** Un tacto anota la preñez, un parto da de alta la cría, una castración cambia la categoría. Individuales o por lote.
- **Seguridad y multiusuario.** Invitaciones con código, roles (dueño, carga datos, solo mira) y reglas de Firestore probadas con el emulador.
- **Backend del panel.** Fastify + MySQL con Drizzle, con un proceso que replica Firestore a MySQL de forma incremental. Generador de `.xlsx` propio, sin dependencias.

<details>
<summary><b>Más funcionalidades</b></summary>
<br>

- Recuento por potrero: tomar asistencia y ver quién falta (así nació la app).
- Ficha completa del animal: caravana visual y electrónica, pelaje, genealogía, categoría sugerida, partos y castración.
- Avisos locales: partos, fin del retiro sanitario, destete, celo después del servicio y pendientes sanitarios.
- Compras y ventas con precio por kilo o por cabeza, desbaste, comisión y gastos.
- Informes en PDF y Excel con la marca del productor, y marca del ganado dibujada con el dedo.
- Respaldos locales y en Google Drive.
- Diseño para leerse a pleno sol: contraste ≥ 6:1, botones grandes y estados siempre con ícono + texto.
- Panel web (planes pagos): indicadores reproductivos, curva de peso, resultado comercial, informes por período y manifestación. Planes por cantidad de cabezas; la app nunca bloquea los datos ya cargados.
- Pruebas: datos con `node:sqlite`, reglas con el emulador de Firebase y pruebas del backend.

</details>

**Stack**

![Expo](https://img.shields.io/badge/Expo_SDK_54-000020?style=flat-square&logo=expo&logoColor=white)
![React Native](https://img.shields.io/badge/React_Native_0.81-20232A?style=flat-square&logo=react&logoColor=61DAFB)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![SQLite](https://img.shields.io/badge/SQLite-003B57?style=flat-square&logo=sqlite&logoColor=white)
![Firebase](https://img.shields.io/badge/Firebase-FFCA28?style=flat-square&logo=firebase&logoColor=black)
![NativeWind](https://img.shields.io/badge/NativeWind-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-5FA04E?style=flat-square&logo=nodedotjs&logoColor=white)
![Fastify](https://img.shields.io/badge/Fastify-000000?style=flat-square&logo=fastify&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white)
![Drizzle](https://img.shields.io/badge/Drizzle_ORM-C5F74F?style=flat-square&logo=drizzle&logoColor=black)
![React](https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB)
![Vite](https://img.shields.io/badge/Vite-646CFF?style=flat-square&logo=vite&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white)

> 🔒 Código en repositorios privados.

---

## 📂 Otros proyectos

| Proyecto | Descripción |
|---|---|
| [**Tarefero**](https://play.google.com/store/apps/details?id=com.haberleslucas.yerbaapp) · Google Play | App móvil para el cultivo de yerba mate: funcionamiento offline/online, sincronización y reportes. |
| **streeamtech.com** | Aplicación web completa: diseño UI/UX, frontend, backend y estructura de datos. |
| [**Vaca Manager App**](https://github.com/HaberlesLucas/Vaca-Manager-App/blob/main/README.pdf) | Gestión ganadera en Android nativo con Kotlin y SQLite. |
| [**App Android**](https://github.com/HaberlesLucas/App-Android) | App práctica en Android nativo con RecyclerView y persistencia de datos. |

---

## 🛠️ Tecnologías

**Frontend y mobile**

![React](https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB)
![React Native](https://img.shields.io/badge/React_Native-20232A?style=flat-square&logo=react&logoColor=61DAFB)
![Expo](https://img.shields.io/badge/Expo-000020?style=flat-square&logo=expo&logoColor=white)
![Angular](https://img.shields.io/badge/Angular-DD0031?style=flat-square&logo=angular&logoColor=white)
![Vue.js](https://img.shields.io/badge/Vue.js-4FC08D?style=flat-square&logo=vuedotjs&logoColor=white)
![Kotlin](https://img.shields.io/badge/Kotlin-7F52FF?style=flat-square&logo=kotlin&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white)
![Bootstrap](https://img.shields.io/badge/Bootstrap-7952B3?style=flat-square&logo=bootstrap&logoColor=white)

**Backend**

![Node.js](https://img.shields.io/badge/Node.js-5FA04E?style=flat-square&logo=nodedotjs&logoColor=white)
![Java](https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white)
![PHP](https://img.shields.io/badge/PHP-777BB4?style=flat-square&logo=php&logoColor=white)
![Laravel](https://img.shields.io/badge/Laravel-FF2D20?style=flat-square&logo=laravel&logoColor=white)
![Firebase](https://img.shields.io/badge/Firebase-FFCA28?style=flat-square&logo=firebase&logoColor=black)

**Bases de datos**

![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white)
![SQL Server](https://img.shields.io/badge/SQL_Server-CC2927?style=flat-square)
![SQLite](https://img.shields.io/badge/SQLite-003B57?style=flat-square&logo=sqlite&logoColor=white)
![PL/SQL](https://img.shields.io/badge/PL%2FSQL-F80000?style=flat-square)

**Herramientas**

![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)
![Postman](https://img.shields.io/badge/Postman-FF6C37?style=flat-square&logo=postman&logoColor=white)
![Selenium](https://img.shields.io/badge/Selenium-43B02A?style=flat-square&logo=selenium&logoColor=white)
![Figma](https://img.shields.io/badge/Figma-F24E1E?style=flat-square&logo=figma&logoColor=white)
![Trello](https://img.shields.io/badge/Trello-0052CC?style=flat-square&logo=trello&logoColor=white)

---

## 🎓 Formación

- **Licenciatura en Sistemas de Información** · UNNE · 2020 – actualidad (~90 %)
- **Analista Programador Universitario** · UNNE · título intermedio
- **Técnico Superior en Infraestructura Informática** · ISFD Bella Vista, Corrientes · 2017 – 2019

**Cursos y certificaciones**

- **Talentos Digitales** · TelCo – UNNE – Polo IT Corrientes · 1 año, full stack con Laravel + Vue.js
- **Programación de IA** · Ubatec, Facultad de Derecho, UBA
- **Desarrollo Móvil** · Start Coding IA

🌐 Español nativo · Inglés técnico (lectura y escritura)
