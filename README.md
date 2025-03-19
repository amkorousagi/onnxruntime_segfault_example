### to reproduce

1. `npm ci`
2. `node index.js`


### desciription of the issue

when importing onnxruntime-node and @huggingface/transformers, onnxruntime makes segmentation fault or bus error and prints the following error message
```
libc++abi: terminating due to uncaught exception of type onnxruntime::OnnxRuntimeException: /Users/runner/work/1/s/onnxruntime/core/session/ort_env.cc:92 static void OrtEnv::Release(OrtEnv *) env_ptr == p_instance_.get() was false. 

zsh: abort      node index.js
```

 screenshots(only import):

![Image](https://github.com/user-attachments/assets/fa2d9058-32d6-4488-985e-6dae6015ddc0)

![Image](https://github.com/user-attachments/assets/e83fe688-3c5c-4f91-ad02-bf4e459ece72)

 screenshots(load model after import):

![Image](https://github.com/user-attachments/assets/51bfaa17-2cb1-4ca5-8d93-4cf28cd9a1b5)

![Image](https://github.com/user-attachments/assets/725428e4-b8e9-4a52-a57d-3c834d493fa5)
