# Artemis 2.0 - Ajuste de distribuciones de probabilidad

Aplicación web hecha por el equipo **Artemis 2.0** para el Concurso Académico de Simulación 2026A.
Funciona en el navegador (computadora y celular), sin instalar nada y sin enviar los datos a ningún servidor.

## Qué hace
- Carga de datos: pegar desde Excel, archivo CSV/TXT o datos de ejemplo.
- Estadísticos descriptivos (media, desviación, cuartiles, asimetría, curtosis).
- Ajuste de 10 distribuciones: Normal, Lognormal, Exponencial, Weibull, Gamma, Uniforme, Triangular, Logística, Gumbel y Beta.
- Pruebas de bondad de ajuste: Kolmogorov-Smirnov, Anderson-Darling y Chi-cuadrado, con ranking por puntaje.
- Histograma con PDF ajustada y gráfica de la CDF.
- Generador de números aleatorios (por inversión numérica de la CDF) con exportación a CSV y fórmula equivalente en Excel.

## Método
- Normal, Lognormal, Exponencial, Uniforme: máxima verosimilitud (estimadores cerrados).
- Weibull y Gamma: máxima verosimilitud resuelta por bisección.
- Triangular, Logística, Gumbel y Beta: método de momentos.
- Las funciones especiales (gamma incompleta, beta incompleta, erf) están programadas en el propio código.
- Los valores p de K-S y Chi-cuadrado son aproximados porque los parámetros se estiman con los mismos datos.

## Cómo publicarla en GitHub Pages
1. Crear un repositorio público y subir todos los archivos de esta carpeta.
2. Settings > Pages > Branch `main` / carpeta `/ (root)` > Save.
3. El link queda como `https://usuario.github.io/nombre-del-repositorio/`.

## Instalar en el celular
Abrir el link en Chrome (Android) o Safari (iPhone) y elegir "Añadir a pantalla de inicio" / "Instalar app".

## Archivos
- `index.html`: toda la aplicación (HTML, CSS y JavaScript).
- `manifest.json`, `sw.js`, `icon-*.png`: permiten instalarla como app y usarla sin conexión.

## Autores
Equipo Artemis 2.0.
