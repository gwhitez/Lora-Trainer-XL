# 🚀 Entrenamiento de LoRA XL y Auto Tagger
Repositorio con cuadernos para entrenar LoRA XL y procesar datasets de imágenes con auto-tagging usando los modelos de Waifu Diffusion.

>🏠 **Original Proyect** [![GitHub](https://raw.githubusercontent.com/hollowstrawberry/kohya-colab/main/assets/github.svg)](https://github.com/hollowstrawberry/kohya-colab) <p>
**Modified By WhiteZ** [![GitHub](https://raw.githubusercontent.com/hollowstrawberry/kohya-colab/main/assets/github.svg)](https://github.com/gwhitez/Lora-Trainer-XL) <p>

## ✨ Características Principales

Este repositorio contiene un conjunto de notebooks de Google Colab especializados en:
- **Entrenamiento de LoRA XL** con implementaciones actualizadas
- **Procesamiento de datasets** con auto-etiquetado usando los modelos de Waifu diffusion
- Compatibilidad con diferentes versiones de modelos XL (XL base, Animagine, Finetuning, Pony, Illustrious, NoobAI, Vpred etc...)
- Enlacé a Google Drive por defecto.
- Uso fácil con una configuración por defecto que funciona en la mayoría de los casos.
- **auto off**: apaga el entorno automáticamente al terminar el entrenamiento evitando el desperdicio de horas de gpu gratuita, relajate y tomate un café ☕ mientras el lora se entrena.

### Entrenamiento LoRA XL
- Dos variantes de entrenamiento:
  
  `Fix_Lora_Trainer.ipynb` [![Open in Colab](https://raw.githubusercontent.com/hollowstrawberry/kohya-colab/main/assets/colab-badge.svg)](https://colab.research.google.com/github/gwhitez/Lora-Trainer-XL/blob/main/Fix_Lora_Trainer_XL.ipynb) :
  - Scripts de entrenamiento más recientes.
  - Mejor manejo de los recursos de Colab.
  - Soporte para entrenamiento Vpred.
  - ⚡ Instalación rapida. ⚡
  - Entrenamiento con modelos `.safetensors o .ckpt` en colab gratuito.
  - Entrenamiento con Optimizador CAME+REX ¡especialmente bueno con datasets pequeños!
    
  `Old_Fix_Lora_Trainer.ipynb` [![Open in Colab](https://raw.githubusercontent.com/hollowstrawberry/kohya-colab/main/assets/colab-badge.svg)](https://colab.research.google.com/github/gwhitez/Lora-Trainer-XL/blob/main/Old_Fix_Lora_Trainer_XL.ipynb) :
  - ~Scrips de entrenamiento más antiguo (2023)~ Scrips de entrenamiento actualizados.
  - ¡Ahora soporta entrenamiento de lora Vpred!
  -  ⚡ Instalación rapida. ⚡
  - requiere uso de modelo en formato Diffusers para entrenamiento en Colab gratuito. <p>
  
  ## ⚠️ **Advertencia: Los resultados pueden variar dependiendo del cuaderno usado. ⚠️** 

### Auto-Tagging de Datasets
`Dataset_Maker_By_WhiteZ.ipynb` [![Open in Colab](https://raw.githubusercontent.com/hollowstrawberry/kohya-colab/main/assets/colab-badge.svg)](https://colab.research.google.com/github/gwhitez/Lora-Trainer-XL/blob/main/Dataset_Maker_By_WhiteZ.ipynb) :
- Etiquetado con los modelos Waifu Diffusion V3.
- ⚡ Instalación rapida (1 minuto aproximadamente.) ⚡
- Funciona en gpu y cpu (en cpu el proceso de etiquetado sera más lento.) Ideal si te quedas sin tiempo de GPU.
- Uso doble de modelos large para mejor precisión en el etiquetado.
- Editor de etiquetas (agregar, eliminar etiquetas.)
- Visualizador de etiquetas.
- crear captions usando el modelo BLIP de lenguaje natural.
  
`Waifu_Diffusion_V3_Dataser_Maker.ipynb`  [![Open in Colab](https://raw.githubusercontent.com/hollowstrawberry/kohya-colab/main/assets/colab-badge.svg)](https://colab.research.google.com/github/gwhitez/Lora-Trainer-XL/blob/main/Waifu_Diffusion_V3_Dataser_Maker.ipynb) :
- Etiquetado con los modelos Waifu Diffusion V3 y modelos Large.
- Editor de etiquetas (agregar, eliminar etiquetas.)
- Funciona en gpu y cpu (en cpu el proceso de etiquetado sera más lento.) Ideal si te quedas sin tiempo de GPU.
- Visualizador de etiquetas.
- modelos de etiquetado mejorados para contenido furry (Z3d) y danbooru (ML).


## 🛠 Requisitos

- Cuenta de Google Colab (para ejecutar los notebooks)
- Acceso a GPU preferiblemente `T4` (en colab gratuito), o `A100/L100` (en colab Pro)
- Cuenta de Google Drive con al menos 1gb de espacio libre.

