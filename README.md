# AI-for-caveman

Yes. If you know **Transformer (2017)**, here's the evolution you should know for the main model families used in modern AI video/search systems:

| Model type              | Evolution                                                                                                      |
| ----------------------- | -------------------------------------------------------------------------------------------------------------- |
| **LLM**                 | RNN/LSTM → Transformer (2017) → BERT/GPT → GPT-3 → instruction tuning → ChatGPT/GPT-4 → multimodal LLMs        |
| **ASR**                 | HMM/GMM → DNN-HMM → CTC → Attention/Seq2Seq → Transformer ASR → Whisper / Conformer / Paraformer               |
| **Speaker Recognition** | i-vectors → x-vectors → speaker embeddings → ECAPA-TDNN → modern multimodal speaker models                     |
| **Text Embeddings**     | TF-IDF → Word2Vec (2013) → GloVe → contextual embeddings (BERT) → Sentence-BERT → modern embedding models      |
| **Computer Vision**     | CNN → ResNet → Vision Transformer (ViT, 2020) → CLIP → VLMs                                                    |
| **Image Embeddings**    | CNN features → ResNet embeddings → CLIP → SigLIP / modern multimodal embeddings                                |
| **Video Understanding** | CNN + optical flow → 3D CNN → Two-Stream → I3D → Video Transformers → Video-VLMs                               |
| **Video Embeddings**    | handcrafted features → CNN/3D-CNN → video transformers → CLIP-based video models → multimodal video embeddings |
| **Object Detection**    | R-CNN → Fast/Faster R-CNN → YOLO → SSD → DETR → modern YOLO/DETR variants                                      |
| **Action Recognition**  | Optical flow → 2D/3D CNN → Two-Stream → I3D → SlowFast → Video Transformers                                    |
| **OCR**                 | Template/feature methods → CNN+RNN → CTC → Transformer OCR → vision-language OCR                               |
| **TTS**                 | Concatenative → parametric → WaveNet → Tacotron → Tacotron 2 → FastSpeech → neural codec/LLM-based TTS         |
| **Video Segmentation**  | traditional CV → CNN segmentation → U-Net/Mask R-CNN → Video Segmentation Transformers → SAM/video-SAM         |
| **Vector Search**       | inverted index → KD/Ball trees → ANN → HNSW → FAISS → vector databases                                         |
| **Reranking**           | TF-IDF/BM25 → learning-to-rank → cross-encoders → BERT rerankers → LLM/VLM reranking                           |

### The most important evolution for **semantic video search**

Focus especially on this chain:

**2017** Transformer
↓
**2018–20** BERT / Sentence-BERT
↓
**2021** CLIP
↓
**2021–23** Video Transformers + video-text models
↓
**2023–25** multimodal/VLMs
↓
**2024–26** large video-language models + multimodal embeddings
↓
**Today:**

`Text → embedding ←→ Video/clip embedding → Vector DB → relevant timestamp`

That's the core technology behind modern **semantic video retrieval**.
