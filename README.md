# 🏆 App Móvil: Consulta de Torneos de Fútbol

## 🌟 Visión General del Proyecto

Esta es una aplicación móvil desarrollada con React Native (Expo) diseñada para ser el punto de consulta oficial de los torneos de fútbol organizados por la administración de canchas.

La aplicación opera bajo un modelo de solo lectura (Read-Only), donde el administrador ingresa los datos de partidos y resultados en la base de datos, y los espectadores acceden a la información actualizada en tiempo real sin necesidad de registrarse.

Objetivo: Proporcionar a los jugadores y espectadores una fuente de información centralizada, rápida y siempre actualizada sobre los partidos, la clasificación del torneo y las estadísticas individuales.

## 🚀 Pila Tecnológica (Tech Stack)

Este proyecto se desarrolla utilizando herramientas modernas y robustas para garantizar estabilidad, rendimiento y escalabilidad (dentro de los límites del plan gratuito).

| Componente    | Tecnologia          | Uso                                                                                         |
| ------------- | ------------------- | ------------------------------------------------------------------------------------------- |
| Frontend      | React Native (Expo) | Desarrollo multiplataforma (iOS y Android) desde una única base de código.                  |
| Navegación    | React Navigation    | Gestión de las transiciones entre pestañas (Tabs) y pantallas de detalle (Stacks).          |
| Base de Datos | Firebase Firestore  | Base de datos NoSQL en tiempo real para almacenamiento de partidos, equipos y estadísticas. |
| Lenguaje      | JavaScript (ES6+)   | Lenguaje principal del proyecto.                                                            |

## 📐 Estructura de la Aplicación (Screens)

La aplicación utiliza un Tab Navigator como raíz con cuatro pantallas principales, y utiliza Stack Navigators internos para manejar las vistas de detalle.

### Tab Navigator (Pestañas Principales)

1. ⚽ Partidos (MatchListScreen): Muestra el listado de los partidos más próximos, ordenados cronológicamente por fecha y hora.
2. 📈 Clasificación (StandingsScreen): Muestra la tabla de posiciones calculada automáticamente: Puntos, PJ, PG, PP, PE, Goles a Favor (GF) y Goles en Contra (GC).
3. 👟 Goleadores (TopScorersScreen): Listado de jugadores ordenados por la cantidad de goles anotados.
4. 🛡️ Equipos (TeamListScreen): Muestra el listado completo de los equipos participantes en el torneo.

### Stack Navigators (Vistas de Detalle)

- `MatchDetailsScreen`: Accedido desde la lista de partidos para ver detalles como la cancha, árbitro y el resumen de goles.

- `TeamDetailsScreen`: Accedido desde la tabla de clasificación o la lista de equipos para ver la plantilla, el historial de partidos y las estadísticas de un equipo específico.
