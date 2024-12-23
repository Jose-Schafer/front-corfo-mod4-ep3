# How to start
Install packages
```sh
nvm use 23
npm install
```

Start dev server
```sh
npm run dev
```

open `http://localhost:5173`

# Preguntas
1. Implementación de vistas complejas con ReactJS
- Ver el navbar
- En `src/views/medical-team/index.jsx` se agregó funcionalidad para filtrar doctores
- En `src/views/contact/form.tsx` se agregó formulario para agendar citas con validaciones

2. Optimización del DOM virtual y uso de fragmentos
Cuando cambia el estado o las props de un componente, React no actualiza inmediatamente el DOM. Lo que hace es actualizar el DOM Virtual, generando una nueva representación de la interfaz de usuario. Al comparar el DOM Virtual anterior con el nuevo se identifica que partes del árbol han cambiado. Una vez ya identificados los cambios, React actualiza las partes necesarias del DOM real, lo que es mucho más rápido que reconstruir todo el DOM.

Uso de fragmentos y contexto en ReactJS Se pude ver el uso de fragmentos en src/views/contact/index.jsx.

3. Uso de referencias y callbacks
Ver en `src/views/contact/form.tsx` el uso de useRef utilizado para enfocar automáticamente el primer input

4. Manejo de datos con API Rest simulada
Ver en `src/providers/DoctorsContex.tsx` como se llama a un json usando un fetch para simular una API

6. Comprobación de tipos con PropTypes
- src/views/home/services.jsx
- src/views/backoffice/appointments.jsx
- src/components/doctor-card/index.jsx
