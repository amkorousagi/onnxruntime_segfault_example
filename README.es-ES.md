

### Para reproducir

1. `npm ci`
2. `node index.js`


### Descripción del problema

al importar onnxruntime-node y @huggingface/transformers, onnxruntime provoca un error de segmentación (segmentation fault) o un error de bus (bus error) e imprime el siguiente mensaje de error
```
libc++abi: terminating due to uncaught exception of type onnxruntime::OnnxRuntimeException: /Users/runner/work/1/s/onnxruntime/core/session/ort_env.cc:92 static void OrtEnv::Release(OrtEnv *) env_ptr == p_instance_.get() was false. 

zsh: abort      node index.js
```

 capturas de pantalla (solo importación):

![Image](https://github.com/user-attachments/assets/e83fe688-3c5c-4f91-ad02-bf4e459ece72)

 capturas de pantalla (carga del modelo después de la importación):

![Image](https://github.com/user-attachments/assets/51bfaa17-2cb1-4ca5-8d93-4cf28cd9a1b5)

![Image](https://github.com/user-attachments/assets/725428e4-b8e9-4a52-a57d-3c834d493fa5)

![Image](https://github.com/user-attachments/assets/fa2d9058-32d6-4488-985e-6dae6015ddc0)
