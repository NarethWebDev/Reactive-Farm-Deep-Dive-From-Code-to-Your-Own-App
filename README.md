# Análisis de My Reactive Farm

## Propósito del proyecto

El proyecto **My Reactive Farm** tiene como objetivo desarrollar una aplicación web interactiva utilizando **React y Vite**, que permita gestionar información relacionada con animales mediante el consumo de una API externa. La aplicación aplica conceptos fundamentales de React como componentes, manejo de estado, efectos, consumo de APIs y formularios, además de una correcta organización del proyecto y el uso de estilos modernos.

---

## Estructura del proyecto

El proyecto sigue una estructura típica de una Single Page Application (SPA) con React:

* **Raíz del proyecto**:

  * `.env`: contiene la configuración de la API.
  * `package.json` y `package-lock.json`: gestión de dependencias.
  * `vite.config.js`: configuración de Vite.
  * `eslint.config.js`: reglas de linting.
  * `folder-structure.txt`: descripción de la organización del proyecto.
  * `index.html`: punto de entrada de la aplicación.

* **Carpeta `src/`**:

  * `components/`: componentes reutilizables de la aplicación.
  * `hooks/`: contiene el archivo `useFetchAnimals.js`, preparado para lógica personalizada.
  * `pages/`: incluye `Farm.jsx`, que funciona como la página principal de la aplicación.
  * `services/`: contiene `animalApi.js`, encargado del consumo de la API.
  * `App.jsx`, `main.jsx`, `App.css` e `index.css`: inicialización y renderizado de la aplicación.

---

## Manejo del estado (`useState`)

El hook `useState` se utiliza para manejar el estado de la aplicación, principalmente en:

* El control de los filtros.
* El almacenamiento de los datos obtenidos desde la API.
* El manejo de errores y estados internos.

Esto permite que la interfaz se actualice de forma dinámica según las acciones del usuario.

---

## Uso de efectos (`useEffect`)

El hook `useEffect` se emplea para manejar efectos secundarios, como:

* La carga inicial de datos desde la API.
* La ejecución de lógica cuando el estado cambia.
* La interacción con servicios externos.

De esta forma, la aplicación responde correctamente al ciclo de vida de los componentes.

---

## Consumo de API con Axios y MockAPI

La aplicación consume una API creada en **MockAPI** para obtener y manipular datos relacionados con animales.

El consumo de la API se realiza mediante **Axios**, implementado en el archivo `animalApi.js`, donde se manejan operaciones como:

* `GET` para obtener datos.
* `UPDATE` para actualizar registros.
* `DELETE` para eliminar información.

Esto permite mantener separada la lógica de negocio del resto de la aplicación.

---

## Manejo de formularios y validaciones

El manejo de formularios se realiza en el componente `AnimalForm.jsx`. Este formulario incluye validaciones básicas que evitan el envío de información incompleta o incorrecta, garantizando datos válidos antes de enviarlos a la API.

Además, se controla el envío de datos y la limpieza de los campos del formulario.

---

## Uso de Tailwind CSS

El proyecto utiliza **Tailwind CSS** como framework de estilos. Está configurado de forma global y se usa a lo largo de toda la aplicación para:

* Diseñar la interfaz de usuario.
* Aplicar estilos responsivos.
* Mantener consistencia visual y facilitar el desarrollo.

---

## Nareth Tatiana Ramírez Fuentes
