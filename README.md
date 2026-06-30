# 🌎 Terremotos Venezuela — Análisis de Daño Estructural

Análisis rápido del dataset elaborado por **Microsoft AI for Good - Building Damage Visualizer** para detectar edificios e infraestructuras colapsadas o con daños severos, a los fines de coordinar las acciones de respuesta inmediata de los equipos de rescate y atención médica a las víctimas. 24 Junio 2026.

🔗 **Fuente de datos:** [Humanitarian Data Exchange - Venezuela Earthquake](https://data.humdata.org/event/venezuela-earthquake)

---

## 📋 Criterios de Clasificación

La severidad fue derivada mediante reglas basadas en:

- `damage_pct_0m` — daño sobre la huella del edificio
- `damage_pct_10m` — daño en buffer de 10m
- `damage_pct_20m` — daño en buffer de 20m
- `unknown_pct` — porcentaje indeterminado

**Clasificación resultante:**

| Clasificación | Descripción |
|---|---|
| 🔴 Severo | Valores altos de daño sobre la huella del edificio |
| 🟠 Moderado | Valores altos en buffers cercanos |
| 🟡 Leve | Valores intermedios en buffers cercanos |
| ⚪ Incierto | Cobertura nubosa sobre el edificio |

---

## ⚠️ Limitaciones y Advertencias

- El análisis depende de la **calidad y cobertura** de las imágenes satelitales.
- La **presencia de nubes** puede reducir la confiabilidad del resultado.
- Los **buffers capturan daño cercano**, pero no siempre implican daño directo sobre el edificio.
- Los resultados deben considerarse como **apoyo a la toma de decisiones** y no como sustituto de verificación de campo, la cual es fundamental.

---

## 🎯 Uso Recomendado

Este producto está realizado para:

- Priorización de inspecciones de campo
- Apoyo a equipos de rescate
- Análisis espacial de daños
- Generación de mapas operativos
- Reportes rápidos de situación

---

## 🛠️ Tecnologías

> *(Acá podés completar con las herramientas que usaste, por ejemplo:)*

- Python / GeoPandas
- QGIS
- Leaflet
- QGIS2WEB

---

## 📄 Licencia

- **Código:** [MIT License](LICENSE)
- **Datos:** [Creative Commons Attribution 4.0 International (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/)

Se permite el uso, modificación y redistribución del código y los datos, incluyendo fines comerciales, siempre que se otorgue el crédito correspondiente.

---

## 👤 Autor

**Rafael Zerpa / GeckoGISP** — [GitHub](https://github.com/rafateamzp)

*Análisis ambiental y geoespacial*
