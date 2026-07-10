# 🦖 Rex Evolution 3D

Juego 3D de navegador: elige tu especie de dinosaurio, devora rivales más pequeños para ganar XP, evoluciona y conviértete en un ápex depredador — o incluso en un ápex volador.

**Jugar:** https://francovillalon1422-sys.github.io/dino-evolution-game/

## Cómo jugar

- **Mover:** WASD / Flechas (o el joystick táctil en móvil)
- **Comer:** choca con dinosaurios más pequeños o de tu mismo nivel
- **Peligro:** los dinosaurios de nivel mayor te quitan una vida si te tocan
- **Combo:** come rápido y seguido para multiplicar tus puntos
- **Mordisco Feroz:** ESPACIO (o el botón 🦷 en móvil) — durante unos segundos puedes comer un nivel por encima del tuyo
- **Meta:** evoluciona hasta el Nivel 4 (Volador Ápex) y consigue la mayor puntuación posible

## Especies jugables

| Especie | Estilo |
|---|---|
| Tiranosaurio Rex | Equilibrado |
| Velocirraptor | Ágil y rápido, más frágil |
| Triceratops | Grande y resistente, más lento |

Cada una evoluciona en 3 niveles propios (Cría → Juvenil → Alfa) y puede seguir evolucionando a un 4º nivel compartido: un ápex volador.

## Funcionalidades

- Mundo 3D real (Three.js) con sombras, niebla y 3 biomas aleatorios (Selva, Desierto, Nevado)
- Modelos 3D animados para las especies jugables
- Sistema de combos, power-ups y una habilidad especial con cooldown
- Rival Ápex: mini-jefe que persigue activamente al jugador
- Skins desbloqueables acumulando puntos entre partidas
- Tabla de puntuaciones local (top 5) y récord persistente
- Controles táctiles para móvil
- Instalable como PWA (Agregar a pantalla de inicio)
- Audio generado por código (Web Audio API), sin archivos de sonido externos

## Tecnología

- [three.js](https://threejs.org/) (r160) vía CDN — render 3D, luces, sombras
- JavaScript puro (ES modules), sin frameworks ni build step
- Web Audio API para efectos y música ambiental
- Service Worker + Web App Manifest para soporte PWA

## Créditos de modelos 3D

Los modelos del Tiranosaurio Rex, Velocirraptor y Triceratops son de **[Quaternius](https://quaternius.com/)**, obtenidos vía [Poly Pizza](https://poly.pizza/), bajo licencia **CC0 (dominio público)** — de uso libre, sin necesidad de atribución.

## Desarrollo local

Es un sitio estático, no requiere instalación. Para probarlo localmente con un servidor (necesario para que carguen los modelos 3D y el service worker):

```
python -m http.server 8000
```

Y abrir `http://localhost:8000/` en el navegador.
