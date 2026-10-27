# Lucas Pimentel

Estudiante de la **Licenciatura en Ingeniería de Datos e Inteligencia Artificial** en UTEC (LIDIA, Uruguay). Trabajo en proyectos de **machine learning, IA generativa e ingeniería de datos**, en equipo y con flujos de desarrollo asistido por agentes de IA (Claude Code): escribo el contexto y los prompts, reviso críticamente lo que se genera y decido qué se integra.

📫 lucas.pime941@gmail.com · [LinkedIn](https://www.linkedin.com/in/lucas-pimentel-barreto-939161212)

---

## 🤖 Machine Learning e IA

### Predicción de siniestros viales en Montevideo — Proyecto de Aprendizaje Automático
Pronóstico a 7 días de la cantidad de siniestros por municipio y día, a partir de la serie histórica de UNASEV (2021–2025). Se compararon GLM Poisson, binomial negativa y XGBoost contra modelos de referencia con **validación temporal en 47 cortes semanales** y reentrenamiento en cada corte. La solución elegida (GLM Poisson con calendario y feriados) superó a la referencia en los 8 municipios y se fijó **antes** de mirar el conjunto de test. Incluye intervalos de predicción del 80 % y 95 %, entrenamiento reproducido en el servidor institucional y una pestaña de predicción integrada en un dashboard en Streamlit.

- **Stack:** Python, pandas, statsmodels, scikit-learn, XGBoost, geopandas, Streamlit, pytest.
- **Buenas prácticas:** entorno con versiones fijadas, tests del pipeline de inferencia, modelo exportado en JSON (sin pickle), una rama por fase con code review antes de cada merge y registro de decisiones.
- **Repositorio:** [proyecto-machine-learning](https://github.com/victoruria-netizen/proyecto-machine-learning) · equipo de 2

### Clasificador de enfermedades foliares: del laboratorio al campo — *en curso*
Clasificador de imágenes entrenado sobre PlantVillage (fotos de laboratorio) y evaluado sobre PlantDoc (fotos de campo), para medir y reducir la brecha de rendimiento fuera de distribución. Deduplicado perceptual de imágenes, particiones congeladas, explicabilidad con CAM y un asistente que se abstiene cuando no tiene confianza suficiente.

- **Stack:** PyTorch, torchvision (MobileNetV3-Small), scikit-learn, imagehash, Gradio, Google Colab.
- **Repositorio:** [enfermedades-foliares](https://github.com/trajano-carballo/enfermedades-foliares) · equipo de 3

### Asistente virtual de orientación — Convenio IPPU × UTEC-LIDIA — *en curso*
Asistente conversacional basado en LLMs que orienta a familias y las deriva al servicio adecuado según el catálogo de servicios del instituto, con una capa de límites para que nunca dé diagnósticos. Llevo esta línea de forma individual.

- **Repositorio:** privado (convenio con una institución de salud).

---

## 🗄️ Ingeniería de datos y desarrollo

### Siniestros viales UY/BR/ES — Pipeline ETL y Data Warehouse híbrido
Integra y normaliza **9,2 millones de registros** de siniestralidad de Uruguay, Brasil y España (2018–2025) con enriquecimiento climático, y los sirve en un dashboard que responde diez preguntas de negocio. ETL idempotente con carga incremental, CDC por fuente y tests de calidad de datos.

- **Stack:** Python, PostgreSQL (modelo dimensional), MongoDB, Docker Compose, Streamlit + Plotly.
- **Repositorio:** [siniestros-viales-etl-dw](https://github.com/lucaspimentel-uy/siniestros-viales-etl-dw) · equipo de 3

### Historia Clínica Electrónica — Convenio IPPU × UTEC-LIDIA
API para la historia clínica de niños, niñas y adolescentes con TEA, con la cadena anual de evaluación y firma de módulos, y una demo web conectada. Hice el backend.

- **Stack:** Python, FastAPI, PostgreSQL, Alembic.
- **Repositorio:** privado (datos de salud de menores).

### Control de calidad de vivero — PWA
Aplicación web progresiva para digitalizar el control de calidad de plantines forestales: carga desde el celular con o sin señal, revisión del supervisor y planilla consolidada automática.

- **Stack:** Next.js, TypeScript, Supabase (PostgreSQL + RLS), Vercel.
- **Repositorio:** privado (proyecto con cliente).

### Otros
- [regresion-clustering-pacd](https://github.com/lucaspimentel-uy/regresion-clustering-pacd) — regresión y clustering k-means sobre siniestralidad en Montevideo, con pipeline reproducible e informe en Quarto (R, SQL).
- [mini-proyecto-series-temporales](https://github.com/lucaspimentel-uy/mini-proyecto-series-temporales) — análisis de series temporales (Jupyter).
- [playlist-migrator-yt-feature](https://github.com/lucaspimentel-uy/playlist-migrator-yt-feature) — migrador de playlists de Spotify a YouTube Music (Python).

---

## 🛠️ Tecnologías

| Área | Herramientas |
|---|---|
| Lenguajes | Python, SQL, R, TypeScript |
| ML e IA | scikit-learn, statsmodels, XGBoost, PyTorch, LLMs, Claude Code |
| Datos | pandas, PostgreSQL, MongoDB, ETL / Data Warehousing |
| Desarrollo | Git, GitHub, GitLab, Docker, FastAPI, Streamlit, pytest |

Formación previa en **Testing de Software** (CES): metodologías ágiles y Selenium IDE.
