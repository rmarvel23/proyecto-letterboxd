# 🎬 Watchlist App (Supabase + REST API)

Aplicación para gestionar una watchlist de películas utilizando Supabase como backend y una API REST generada automáticamente.

---

## 🚀 Descripción

Este proyecto permite:
- Crear una lista de películas (watchlist)
- Consultar registros almacenados en Supabase
- Actualizar y eliminar elementos
- Gestionar datos mediante una API REST automática

---

## 🧠 Arquitectura

- **Backend:** Supabase (PostgreSQL + REST API)
- **API:** PostgREST (auto-generada por Supabase)
- **Frontend:** (añade aquí tu stack si aplica: React, Next.js, etc.)

---

## 📡 Base de datos / API

La API se genera automáticamente desde Supabase:
https://bsnxxxvvcphwarfkyocq.supabase.co/rest/v1/

Ejemplo de endpoint:
/watchlist

---

## 🔐 Autenticación

Todas las peticiones requieren headers. Para más información, leer documentación.

📦 Endpoints principales
📍 GET /watchlist

Obtiene todos los elementos.

📍 POST /watchlist

Crea un nuevo elemento.

📍 PATCH /watchlist?id=eq.x

Actualiza un registro existente.

📍 DELETE /watchlist?id=eq.x

Elimina un registro.

📚 Documentación completa

Toda la documentación detallada de la API, ejemplos y estructura del proyecto está disponible aquí:

👉 Ver documentación en Notion
https://www.notion.so/34533546561e805784c9df04ef1547f8?source=copy_link

🧪 Ejemplo de uso (JavaScript)
fetch("https://bsnxxxvvcphwarfkyocq.supabase.co/rest/v1/watchlist", {
  headers: {
    apikey: "YOUR_ANON_KEY",
    Authorization: "Bearer YOUR_ANON_KEY"
  }
})
  .then(res => res.json())
  .then(data => console.log(data))

🔎 Filtros útiles
?select=* → seleccionar campos
?id=eq.1 → filtrar por ID
?user_id=eq.xxx → filtrar por usuario
?order=id.desc → ordenar resultados
?limit=10 → limitar resultados
🛠️ Tecnologías utilizadas
Supabase
PostgreSQL
REST API (PostgREST)
JavaScript (Fetch API)


📌 Autor
Rocío Martínez Veloso
rmartinezveloso@gmail.com
Data Engineer, QA y Tech Instructor
