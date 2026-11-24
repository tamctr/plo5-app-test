# Camera card reader – third-party files

These files are loaded only when the camera button is opened.

## cards.onnx
- 52-class playing-card corner detector (YOLOv8n), exported to ONNX and quantised to int8 for this app (3.4 MB).
- Weights: https://huggingface.co/mustafakemal0146/playing-cards-yolov8 (`playing_cards_model_0_playing-cards-colab.pt`).
  The Hugging Face card lists the licence as MIT.
- The model was fine-tuned from Ultralytics YOLOv8n (`yolov8n.pt`), whose code and pretrained weights are
  AGPL-3.0 (https://ultralytics.com/license); the checkpoint itself records `license: AGPL-3.0`.
  We therefore treat this file as AGPL-3.0. The full source of this app (the code that loads and runs the model)
  is public at https://github.com/tamctr/plo5-app-test.
- Training data: Playing Cards dataset by Augmented Startups / Roboflow
  (https://universe.roboflow.com/augmented-startups/playing-cards-ow27d), CC BY 4.0.

## ort.wasm.min.js, ort-wasm-simd-threaded.mjs, ort-wasm-simd-threaded.wasm
- onnxruntime-web 1.31.1, © Microsoft Corporation, MIT licence (https://github.com/microsoft/onnxruntime).
