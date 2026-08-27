# Web oficial · CD Unión Popular de Palencia

**Archivo:** `upp-web-v51.html` · **Versión:** v51 · **Última actualización:** 27-08-2026

Web autocontenida en un único archivo HTML (CSS, JS e imágenes incrustadas en base64, sin dependencias externas salvo Google Fonts). Para publicarla basta subir el archivo al hosting renombrado como `index.html`, junto a `sitemap.xml` y `robots.txt`.

---

## Última actualización

- **Resultado del amistoso vs CD Becerril (26-08):** UP Palencia 2–4 CD Becerril, Sergio Asenjo. Goles del UPP: Sergio y Marco.
- El panel **"Último resultado"** del calendario muestra este partido con escudos y goleadores.
- La **agenda de pretemporada** registra los tres amistosos jugados con marcador y goleadores:
  - UP Palencia 2–1 Betis B (Valladolid) — Marco y Aitor
  - Cristo Atlético 0–3 UP Palencia — Aitor (2) y Dela
  - UP Palencia 2–4 CD Becerril — Sergio y Marco
- Próximos compromisos visibles: sábado 29 vs AD Villada y Memorial Ana García Gil (5 de septiembre).

## Estado general de la web

- **Portada:** hero con cuenta atrás, panel de último resultado, calendario mensual multi-mes, agenda de partidos (contraída, expandible) y clasificación 26/27 con los 18 equipos.
- **Calendario liguero 26/27:** 34 jornadas, contraído por defecto con filtros casa/fuera.
- **Plantilla 26/27:** fichas con foto procesada (fondo blanco, 270×338). Fichajes recientes: Adrián Pereira (dorsal 18), Aitor Fernández (19, con foto), Dela (20, sin foto aún).
- **Muro social:** perfiles incrustados reales de Instagram y Facebook tras el consentimiento de cookies (X no permite incrustado sin sesión; enlace directo). *No cargan en local (`file://`): requieren servirse desde el dominio.*
- **Hemeroteca:** "¿Te acuerdas de…?" con 12 vídeos + sección "Los directos de Elviphotoss" con 8 partidos completos, temporadas verificadas.
- **Histórico:** 8 temporadas con clasificaciones completas y todos los escudos (28 rivales), primera fase del ascenso 21/22, estadísticas de plantilla por temporada (122 jugadores) y récords de todos los tiempos con clasificaciones desplegables.
- **Patrocinadores principales (6):** Roams, Anklaas, Taberna La Herrada, Tecnicampo, Bella Luna Escuela de Danza (enlace a Instagram), Palestine Drinks España. Colaboradores en rejilla aparte (con Ayuntamiento · Patronato Municipal de Deportes).
- **Selector de vista:** botón en la barra superior para alternar vista móvil / escritorio, con memoria de la elección.
- **SEO:** título, meta description, Open Graph, JSON-LD SportsTeam y canonical unificado a `https://www.unionpopularpalencia.com/`.

## Pendiente

1. **Publicación correcta en el hosting:** subir el archivo como `index.html` en la raíz (no pegarlo en el constructor, que rompe el SEO y muestra el título "Club de futbol Union Popular Palencia" duplicado).
2. Subir también `sitemap.xml` y `robots.txt`; dar de alta la web en **Google Search Console** y crear el **Perfil de Empresa de Google**.
3. Foto de **Dela** y confirmación de posiciones/dorsales de los tres fichajes.
4. Enlace del vídeo del **gol de Calvillo** si aparece; más directos de Elviphotoss si los localizas en su pestaña "Directos".
5. Resultado del amistoso vs AD Villada (29-08) cuando se juegue.
6. Conversión de la cuenta de Instagram a profesional para activar el carrusel de Behold.

## Cómo actualizar resultados de amistosos

En `const EVENTOS`, añadir al partido jugado: `resultado:"2–4", goles:"Sergio y Marco"` — la agenda lo marca como Final automáticamente. El panel "Último resultado" se edita en el bloque `panel-ultimo` (equipo local a la izquierda).
