# Lecti - Descarga del ejecutable

Lecti es una aplicación de apoyo a la lectura para estudiantes, con pruebas de
comprensión lectora, análisis semántico de voz y seguimiento de progreso por
estudiante. El código fuente completo del proyecto (Godot + servidor Python)
está en [CarvajalMax/Lecti](https://github.com/CarvajalMax/Lecti).

Este repositorio solo contiene el **ejecutable listo para usar** (ver la
sección [Releases](../../releases) de este repositorio para descargarlo).

## Contenido de la descarga

- `Lecti.exe` — la aplicación. Se entrega sin estudiantes, cuentos ni
  progresos cargados: arranca completamente limpia.
- `Lecti_Completo.zip` — lo mismo más la carpeta `Servidor` con el servicio
  de voz y análisis de texto (Whisper + spaCy) que necesitan las pruebas de
  lectura, semántica y preguntas abiertas.

## Cómo usarlo

1. Descomprime `Lecti_Completo.zip` (o descarga `Lecti.exe` solo si únicamente
   quieres navegar por la interfaz sin las pruebas que usan voz/análisis).
2. Abre `Servidor\Iniciar_Servidor.bat` y espera a que diga que el servidor
   quedó escuchando en `http://127.0.0.1:8000`. La primera vez necesita
   internet para instalar dependencias de Python y el modelo de español
   (puede tardar varios minutos).
3. Abre `Lecti.exe`.

### Requisitos

- Windows 10/11 de 64 bits.
- Python 3.10 o superior instalado (con la opción "Add python.exe to PATH"
  marcada al instalarlo) si vas a usar las pruebas que dependen del servidor.
