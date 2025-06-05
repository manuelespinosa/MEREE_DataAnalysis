# MEREE DataAnalysis

Notebook docente para análisis de datos climatológicos en la asignatura **Metodología de la Investigación** del **Máster en Energías Renovables y Eficiencia Energética**, Universidad de Cádiz.

## Descripción
Este repositorio contiene un notebook de Jupyter en Python (`MetodologiaDeLaInvestigacion.ipynb`) desarrollado para la docencia de la asignatura **Metodología de la Investigación** durante el curso 2024-2025. El notebook permite recolectar, procesar y analizar datos climatológicos diarios (temperatura media y precipitación) de la estación de Tarifa (Cádiz) desde 1945 hasta 2025, utilizando la API de AEMET OpenData. Fue utilizado en **prácticas de laboratorio** para enseñar a los estudiantes técnicas de adquisición de datos, procesamiento con pandas y análisis para investigaciones en energías renovables.

El notebook realiza las siguientes funciones:  
- Recolecta datos climatológicos históricos vía la API de AEMET, dividiendo las consultas en tramos de 6 meses para optimizar la obtención.  
- Procesa datos (temperatura media, precipitación) en un DataFrame con pandas, limpiando y normalizando valores.  
- Genera un archivo CSV (`datosTarifa.csv`) y agrupa datos por año para análisis anual.  

## Uso Docente
Los scripts se emplearon en **prácticas regladas** de Metodología de la Investigación para:  
- Introducir a los estudiantes en la obtención de datos abiertos para investigación científica.  
- Enseñar técnicas de procesamiento y análisis de datos climatológicos con Python y pandas.  
- Desarrollar habilidades en metodología de investigación aplicada a energías renovables, como la preparación de datos para estudios de viabilidad de proyectos energéticos.  

Los estudiantes usaron el notebook para analizar tendencias climáticas, interpretar datos y aplicar resultados en proyectos de investigación.

## Instalación y Ejecución
### Requisitos
- Python 3.8 o superior  
- Bibliotecas: `requests`, `pandas`, `matplotlib`, `tqdm`  
  ```bash
  pip install requests pandas matplotlib tqdm
  ```
- API Key de AEMET OpenData (regístrate en https://opendata.aemet.es)

### Instrucciones
1. Clona el repositorio:  
   ```bash
   git clone https://github.com/manuelespinosa/MEREE_DataAnalysis.git
   ```
2. Navega al directorio:  
   ```bash
   cd MEREE_DataAnalysis
   ```
3. Abre el notebook en Jupyter o Google Colab:  
   - Local:  
     ```bash
     jupyter notebook MetodologiaDeLaInvestigacion.ipynb
     ```
   - Colab: Abre el enlace en el notebook o súbelo a https://colab.research.google.com.  
4. Configura la API Key:  
   - Reemplaza `"INSERTA_AQUI_API_KEY_DE_AEMET"` en el notebook con tu clave de AEMET.  
5. Ejecuta las celdas para recolectar, procesar y exportar datos a `datosTarifa.csv`.

## Estructura del Repositorio
- `MetodologiaDeLaInvestigacion.ipynb`: Notebook principal para análisis de datos climatológicos.  
- `README.md`: Documentación del proyecto.  
- `LICENSE`: Licencia MIT.  
- `.zenodo.json`: Metadatos para Zenodo.  
- `/data/datosTarifa.csv` (opcional): Ejemplo de datos generados.

## Autoría
- **Manuel Jesús Espinosa Gavira**  
  Docente e investigador, Universidad de Cádiz  
  Correo: manuel.espinosa@uca.es  

## Licencia
Este proyecto está licenciado bajo la **Licencia MIT**. Consulta el archivo [LICENSE](LICENSE) para más detalles.

## Citación
Si usas este software en un contexto académico, cita el repositorio:  
Espinosa Gavira, M. J.
