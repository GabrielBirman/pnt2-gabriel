# Farmacity 24/7 💊

Aplicación web de farmacia online con tienda para clientes y panel de administración, hecha con **Vue 3**.

El back-end está en [farmacia-online-api](https://github.com/GabrielBirman/farmacia-online-api).

## Funcionalidades

### Clientes
- Registro e inicio de sesión
- Catálogo de medicamentos
- Carrito de compras con estado persistente
- Checkout en 4 pasos, con elección del método de pago
- Perfil de usuario

### Administración
- ABM de medicamentos
- Gestión de usuarios
- Seguimiento de pedidos por estado
- **Dashboard de ventas** con gráficos: ventas por día, por día de la semana, productos con y sin receta, y mapa de calor de actividad

## Tecnologías

- **Vue 3** + **Vite**
- **Vue Router**, con rutas separadas para clientes y administradores
- **Pinia** para el estado global (auth, carrito, productos), con persistencia
- **Axios** para consumir APIs REST (simuladas con MockAPI)
- **Chart.js** / vue-chartjs para los gráficos
- **Tailwind CSS**

## Estructura

```
src/
├── components/    # Componentes reutilizables (cards, carrito, pasos del checkout, gráficos)
├── pages/         # Vistas: Login, Home, Carrito, Checkout, Admin, Dashboard...
├── store/         # Stores de Pinia: auth, carrito, product
├── services/      # Llamadas a la API (usuarios y productos)
└── composables/   # Lógica reutilizable
```

## Cómo correrlo

```sh
npm install
npm run dev
```
