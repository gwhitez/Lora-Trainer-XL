# 🚀 Entrenamiento de LoRA XL y Auto Tagger
Repositorio con notebooks para entrenar LoRA XL y procesar datasets de imágenes con auto-tagging usando los modelos de Waifu Diffusion.

🏠 **Original Project** [![GitHub](https://raw.githubusercontent.com/hollowstrawberry/kohya-colab/main/assets/github.svg)](https://github.com/hollowstrawberry/kohya-colab) <p>
🏠 **Modified By WhiteZ** [![GitHub](https://raw.githubusercontent.com/hollowstrawberry/kohya-colab/main/assets/github.svg)](https://github.com/gwhitez/Lora-Trainer-XL) <p>

## ✨ Características Principales

Este repositorio contiene un conjunto de notebooks de Google Colab especializados en:
- **Entrenamiento de LoRA XL** con implementaciones actualizadas
- **Procesamiento de datasets** con auto-etiquetado usando los modelos de Waifu Diffusion
- Compatibilidad con diferentes versiones de modelos XL (XL base, Animagine, Finetuning, Pony, Illustrious, NoobAI, Vpred, etc.)
- Enlace a Google Drive por defecto
- Uso fácil con una configuración por defecto que funciona en la mayoría de los casos
- **Auto off**: apaga el entorno automáticamente al terminar el entrenamiento evitando el desperdicio de horas de GPU gratuita, relájate y tómate un café ☕ mientras el LoRA se entrena

### Entrenamiento LoRA XL
- ## **⚠️ Ambos cuadernos tienen las mismas características pero el resultado final aún puede ser distinto dependiendo del cuaderno usado y la configuración. ⚠️**
  
`WhiteZ LoRA Trainer SDXL` [![Open in Colab](https://raw.githubusercontent.com/hollowstrawberry/kohya-colab/main/assets/colab-badge.svg)](https://colab.research.google.com/github/gwhitez/Lora-Trainer-XL/blob/main/WhiteZ_Lora_Trainer_SDXL.ipynb) <p>
`WhiteZ LoRA Trainer SDXL v2` [![Open in Colab](https://raw.githubusercontent.com/hollowstrawberry/kohya-colab/main/assets/colab-badge.svg)](https://colab.research.google.com/github/gwhitez/Lora-Trainer-XL/blob/main/WhiteZ_Lora_Trainer_SDXL_v2.ipynb) <p>
  - Scripts de entrenamiento más recientes
  - Mejor manejo de los recursos de Colab
  - Soporte para entrenamiento Vpred
  - ⚡ Instalación rápida ⚡
  - Entrenamiento con modelos `.safetensors o .ckpt` en Colab gratuito usando full FP16
  - Entrenamiento en FP16 (solo con modelos diffusers en Colab gratuito)
  - Entrenamiento con Prodigy funcional y configuraciones óptimas para Colab gratuito
  - Entrenamiento con Optimizador CAME+REX ¡especialmente bueno con datasets pequeños!
  - Uso de venv (entorno virtual) para evitar errores cuando Google hace cambios en Colab &lt;p&gt;

  
### Auto-Tagging de Datasets
`Dataset_Maker_By_WhiteZ.ipynb` [![Open in Colab](https://raw.githubusercontent.com/hollowstrawberry/kohya-colab/main/assets/colab-badge.svg)](https://colab.research.google.com/github/gwhitez/Lora-Trainer-XL/blob/main/Dataset_Maker_By_WhiteZ.ipynb) :
- Etiquetado con los modelos Waifu Diffusion V3
- ⚡ Instalación rápida (1 minuto aproximadamente) ⚡
- Funciona en GPU y CPU (en CPU el proceso de etiquetado será más lento). Ideal si te quedas sin tiempo de GPU
- Uso doble de modelos Large para mejor precisión en el etiquetado
- Editor de etiquetas (agregar, eliminar etiquetas)
- Visualizador de etiquetas
- Crear captions usando el modelo BLIP de lenguaje natural
  
`Waifu_Diffusion_V3_Dataset_Maker.ipynb`  [![Open in Colab](https://raw.githubusercontent.com/hollowstrawberry/kohya-colab/main/assets/colab-badge.svg)](https://colab.research.google.com/github/gwhitez/Lora-Trainer-XL/blob/main/Waifu_Diffusion_V3_Dataser_Maker.ipynb) :
- Etiquetado con los modelos Waifu Diffusion V3 y modelos Large
- Editor de etiquetas (agregar, eliminar etiquetas)
- Funciona en GPU y CPU (en CPU el proceso de etiquetado será más lento)
- Visualizador de etiquetas
- Modelos de etiquetado mejorados para contenido furry (Z3d) y Danbooru (ML)


## 🛠 Requisitos

- Cuenta de Google Colab (para ejecutar los notebooks)
- Acceso a GPU preferiblemente `T4` (en Colab gratuito), o `A100/L4` (en Colab Pro)
- Cuenta de Google Drive con al menos 1 GB de espacio libre
