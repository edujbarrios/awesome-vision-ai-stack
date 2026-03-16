# Awesome Vision AI Stack [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A curated, builder-first list of **Vision Language Models (VLMs)**, local runtimes, document AI tools, UI agents, robotics vision stacks, datasets, benchmarks, and production resources.
>
> The goal is not to collect every paper. The goal is to help developers **build with vision**.

## Why this list exists

Most multimodal lists are strong on papers but weak on execution.

This one is optimized for builders who want to answer questions like:

- Which VLMs can I run locally?
- Which models are good for documents, charts, OCR, and screenshots?
- What should I use for UI agents and computer-use workflows?
- Which stacks help with robotics, grounding, and action?
- How do I benchmark, fine-tune, and ship a multimodal product?

## Contents

- [Foundation VLMs](#foundation-vlms)
- [Local Inference and Serving](#local-inference-and-serving)
- [Document AI, OCR, and Chart Understanding](#document-ai-ocr-and-chart-understanding)
- [UI Understanding and Computer Use](#ui-understanding-and-computer-use)
- [Agents, Grounding, and Robotics](#agents-grounding-and-robotics)
- [Video and Long-Context Multimodality](#video-and-long-context-multimodality)
- [Training and Fine-Tuning](#training-and-fine-tuning)
- [Benchmarks and Evaluation](#benchmarks-and-evaluation)
- [Datasets](#datasets)
- [Applications and Demos](#applications-and-demos)
- [Learning Resources](#learning-resources)
- [Contributing](#contributing)

---

## Foundation VLMs

### General-purpose open models
- [LLaVA](https://github.com/haotian-liu/LLaVA) - One of the most influential open visual instruction-tuned models.
- [Qwen2-VL](https://github.com/QwenLM/Qwen2-VL) - Strong open multimodal family for image, document, and video understanding.
- [Qwen-VL](https://github.com/QwenLM/Qwen-VL) - Earlier Qwen multimodal line with broad ecosystem support.
- [InternVL](https://github.com/OpenGVLab/InternVL) - Strong family of open large vision-language models.
- [CogVLM](https://github.com/THUDM/CogVLM) - Open visual language model family from THUDM.
- [MiniGPT-4](https://github.com/Vision-CAIR/MiniGPT-4) - Early and influential image-chat system.
- [InstructBLIP](https://github.com/salesforce/LAVIS/tree/main/projects/instructblip) - Instruction-tuned extension of BLIP-style architectures.
- [BLIP-2](https://github.com/salesforce/LAVIS/tree/main/projects/blip2) - Efficient VLM architecture connecting frozen vision and language models.
- [IDEFICS](https://github.com/huggingface/smollm/tree/main/vision) - Hugging Face open multimodal family.
- [DeepSeek-VL](https://github.com/deepseek-ai/DeepSeek-VL) - Open multimodal reasoning models from DeepSeek.
- [Molmo](https://github.com/allenai/molmo) - Open multimodal assistant from Ai2 with strong grounding focus.
- [Phi-3 Vision](https://huggingface.co/microsoft/Phi-3-vision-128k-instruct) - Compact multimodal model useful for practical deployments.
- [Fuyu](https://huggingface.co/adept/fuyu-8b) - Multimodal autoregressive model with a distinct design.
- [SmolVLM](https://huggingface.co/collections/HuggingFaceTB/smolvlm-67531d47c514f6f87c3f448f) - Small multimodal models for lightweight use cases.

### Research landmarks
- [Flamingo](https://arxiv.org/abs/2204.14198) - Landmark few-shot visual language model.
- [Kosmos-1](https://arxiv.org/abs/2302.14045) - Early multimodal reasoning and grounding work.
- [PaLI](https://arxiv.org/abs/2209.06794) - Scalable multilingual vision-language model.
- [PaLI-X](https://arxiv.org/abs/2305.18565) - Larger multimodal extension of PaLI.
- [Kosmos-2](https://arxiv.org/abs/2306.14824) - Grounded multimodal large language model.
- [SEED-Bench ecosystem](https://github.com/AILab-CVC/SEED-Bench) - Useful benchmark family around multimodal reasoning.

### Models people actually test in products
- LLaVA-style models for rapid prototyping
- Qwen2-VL family for stronger general multimodal performance
- InternVL for competitive open performance
- Phi-3 Vision and SmolVLM for lighter deployments
- Molmo for grounding-heavy exploration

---

## Local Inference and Serving

### Run locally
- [Ollama](https://github.com/ollama/ollama) - Local model runtime with growing multimodal support.
- [LM Studio](https://lmstudio.ai/) - Desktop app for running local models with a friendly UI.
- [Jan](https://github.com/menloresearch/jan) - Open local AI runtime and desktop app.
- [llama.cpp](https://github.com/ggerganov/llama.cpp) - Core local inference stack; important for lightweight experimentation.
- [MLC-LLM](https://github.com/mlc-ai/mlc-llm) - Compile and deploy models on edge and mobile devices.
- [OpenVINO](https://github.com/openvinotoolkit/openvino) - Useful for Intel-optimized deployments.

### Serve at scale
- [vLLM](https://github.com/vllm-project/vllm) - High-throughput inference engine increasingly relevant for multimodal serving.
- [SGLang](https://github.com/sgl-project/sglang) - Fast serving and structured generation framework.
- [TensorRT-LLM](https://github.com/NVIDIA/TensorRT-LLM) - NVIDIA-optimized inference stack.
- [TGI](https://github.com/huggingface/text-generation-inference) - Hugging Face serving stack.
- [BentoML](https://github.com/bentoml/BentoML) - Production model serving and packaging.
- [Ray Serve](https://github.com/ray-project/ray) - Scalable service orchestration for model workloads.

### APIs and interfaces
- [Open WebUI](https://github.com/open-webui/open-webui) - Popular self-hosted chat UI for local models.
- [Lobe Chat](https://github.com/lobehub/lobe-chat) - Polished interface for model backends.
- [LibreChat](https://github.com/danny-avila/LibreChat) - Open chat UI with multi-backend support.
- [Flowise](https://github.com/FlowiseAI/Flowise) - Visual builder for LLM and multimodal pipelines.

---

## Document AI, OCR, and Chart Understanding

This is one of the biggest practical VLM opportunities.

### Models and tools
- [PaddleOCR](https://github.com/PaddlePaddle/PaddleOCR) - Strong OCR toolkit and a common baseline for document pipelines.
- [docTR](https://github.com/mindee/doctr) - OCR for document text detection and recognition.
- [Nougat](https://github.com/facebookresearch/nougat) - OCR-style document understanding for scientific PDFs.
- [Donut](https://github.com/clovaai/donut) - OCR-free document understanding model.
- [LayoutLM](https://github.com/microsoft/unilm/tree/master/layoutlm) - Important family for document layout understanding.
- [MinerU](https://github.com/opendatalab/MinerU) - Open document parsing and PDF extraction tooling.
- [Marker](https://github.com/VikParuchuri/marker) - PDF-to-markdown/document extraction workflow.
- [Surya](https://github.com/VikParuchuri/surya) - OCR and layout toolkit.
- [ChartOCR](https://github.com/zmykevin/ChartOCR) - Chart understanding reference.
- [ChartQA](https://github.com/vis-nlp/ChartQA) - Dataset and benchmark for chart reasoning.

### Practical stacks
- OCR + VLM reranking for robust document QA
- PDF-to-markdown + VLM summarization
- screenshot parsing for SaaS analytics and support tooling
- chart extraction + VLM reasoning for BI workflows

---

## UI Understanding and Computer Use

Another high-value gap: builders want models that can read screens and act.

### Projects and references
- [SeeAct](https://github.com/OSU-NLP-Group/SeeAct) - Visual web agent framework.
- [OpenHands](https://github.com/All-Hands-AI/OpenHands) - Software agent platform; relevant for multimodal and browser-use workflows.
- [Browser Use](https://github.com/browser-use/browser-use) - Browser automation with model control.
- [Stagehand](https://github.com/browserbase/stagehand) - Browser automation framework aimed at AI-native workflows.
- [OmniParser](https://github.com/microsoft/OmniParser) - Screen parsing for GUI grounding and action planning.
- [UI-TARS](https://github.com/bytedance/UI-TARS) - UI-centric agent/model direction.
- [GroundingDINO](https://github.com/IDEA-Research/GroundingDINO) - Key building block for screen and visual grounding.
- [SAM 2](https://github.com/facebookresearch/sam2) - Segmentation backbone useful for visual agents and annotation loops.

### Strong use cases
- support copilots that understand screenshots
- QA agents for web apps
- workflow automation over dashboards and back-office tools
- computer-use agents with grounding and action planning

---

## Agents, Grounding, and Robotics

### Grounding and perception
- [GroundingDINO](https://github.com/IDEA-Research/GroundingDINO) - Open-set detection from text prompts.
- [Segment Anything](https://github.com/facebookresearch/segment-anything) - Foundational segmentation model.
- [SAM 2](https://github.com/facebookresearch/sam2) - Video-capable segmentation and tracking direction.
- [OWL-ViT](https://github.com/google-research/scenic/tree/main/scenic/projects/owl_vit) - Open-vocabulary detection.
- [Detic](https://github.com/facebookresearch/Detic) - Detection with image-level supervision and open-vocabulary flavor.

### Robotics-oriented projects
- [OpenVLA](https://github.com/openvla/openvla) - Vision-language-action direction for robotics.
- [LeRobot](https://github.com/huggingface/lerobot) - Hugging Face robotics stack.
- [Open X-Embodiment](https://github.com/google-deepmind/open_x_embodiment) - Cross-robot learning ecosystem.
- [RT-1](https://robotics-transformer1.github.io/) - Robotics transformer reference.
- [RT-2](https://robotics-transformer2.github.io/) - Vision-language-action robotics reference.

### Why this section matters
Many “awesome VLM” repos ignore the path from seeing to acting.
This is where vision goes from demo to system.

---

## Video and Long-Context Multimodality

### Models and systems
- [Video-LLaVA](https://github.com/PKU-YuanGroup/Video-LLaVA) - Video extension of LLaVA-style instruction tuning.
- [VideoChat2](https://github.com/OpenGVLab/Ask-Anything) - Video multimodal conversation direction.
- [LLaVA-NeXT-Video](https://github.com/LLaVA-VL/LLaVA-NeXT) - Video-capable branch of the LLaVA family.
- [Qwen2-VL](https://github.com/QwenLM/Qwen2-VL) - Practical option for image and video understanding.
- [LongVU](https://github.com/Vision-CAIR/LongVU) - Long video understanding direction.

### Product opportunities
- meeting and call analysis
- industrial inspection
- sports video understanding
- security review
- agent memory over recorded workflows

---

## Training and Fine-Tuning

### Libraries
- [Transformers](https://github.com/huggingface/transformers) - The default ecosystem for many multimodal models.
- [TRL](https://github.com/huggingface/trl) - Preference optimization and instruction-tuning workflows.
- [PEFT](https://github.com/huggingface/peft) - Parameter-efficient fine-tuning.
- [Axolotl](https://github.com/axolotl-ai-cloud/axolotl) - Popular fine-tuning framework.
- [LLaMA-Factory](https://github.com/hiyouga/LLaMA-Factory) - Large fine-tuning platform with multimodal support.
- [DeepSpeed](https://github.com/microsoft/DeepSpeed) - Distributed training and optimization.
- [PyTorch Lightning](https://github.com/Lightning-AI/pytorch-lightning) - Structured model training workflows.
- [OpenFlamingo](https://github.com/mlfoundations/open_flamingo) - Open framework for Flamingo-style multimodal modeling.
- [LAVIS](https://github.com/salesforce/LAVIS) - Vision-language research and training toolkit.

### Common tuning patterns
- LoRA on the language model head
- projector tuning between vision encoder and language model
- instruction tuning on screenshot or document tasks
- synthetic data generation for niche workflows
- DPO or preference tuning for agent outputs

---

## Benchmarks and Evaluation

### General VLM evaluation
- [MMMU](https://mmmu-benchmark.github.io/) - Massive multitask multimodal reasoning benchmark.
- [MMBench](https://github.com/open-compass/MMBench) - Broad multimodal benchmark.
- [MM-Vet](https://github.com/yuweihao/MM-Vet) - Challenging evaluation for integrated multimodal capabilities.
- [SEED-Bench](https://github.com/AILab-CVC/SEED-Bench) - Foundation multimodal benchmark suite.
- [POPE](https://github.com/RUCAIBox/POPE) - Evaluates object hallucination.
- [HallusionBench](https://github.com/tianyi-lab/HallusionBench) - Hallucination-focused benchmark.
- [ScienceQA](https://github.com/lupantech/ScienceQA) - Science reasoning benchmark with multimodal settings.
- [TextVQA](https://textvqa.org/) - Text-centric visual QA.
- [VQAv2](https://visualqa.org/) - Classic visual question answering benchmark.
- [ChartQA](https://github.com/vis-nlp/ChartQA) - Chart reasoning benchmark.
- [DocVQA](https://www.docvqa.org/) - Document visual question answering benchmark.

### What to evaluate in real products
- hallucination on screenshots and documents
- OCR robustness on messy inputs
- grounding consistency
- latency and memory under real batch sizes
- action reliability for UI agents
- failure modes on out-of-domain images

---

## Datasets

### Image-text pretraining
- [LAION-5B](https://laion.ai/blog/laion-5b/) - Large-scale image-text resource.
- [Conceptual Captions](https://ai.google.com/research/ConceptualCaptions/) - Image-caption dataset.
- [COCO Captions](https://cocodataset.org/) - Standard image captioning dataset.
- [Visual Genome](https://homes.cs.washington.edu/~ranjay/visualgenome/index.html) - Dense visual annotations and relationships.
- [RedCaps](https://github.com/redcaps-dataset/redcaps) - Large image-text dataset from Reddit.
- [DataComp](https://www.datacomp.ai/) - Dataset curation benchmark ecosystem.

### Instruction and conversational multimodal data
- [LLaVA-Instruct-150K](https://huggingface.co/datasets/liuhaotian/LLaVA-Instruct-150K) - Foundational multimodal instruction dataset.
- [ShareGPT4V](https://huggingface.co/datasets/Lin-Chen/ShareGPT4V) - Large multimodal instruction-style dataset.
- [M3IT](https://github.com/MMInstruction/M3IT) - Multimodal instruction tuning data collection.

### Document and chart data
- [DocVQA](https://www.docvqa.org/)
- [InfographicVQA](https://www.docvqa.org/datasets/infographicvqa)
- [ChartQA](https://github.com/vis-nlp/ChartQA)
- [PubLayNet](https://github.com/ibm-aur-nlp/PubLayNet) - Document layout annotations.
- [FUNSD](https://guillaumejaume.github.io/FUNSD/) - Form understanding benchmark.

### Grounding and detection data
- [RefCOCO / RefCOCO+ / RefCOCOg](https://github.com/lichengunc/refer) - Referring expression benchmarks.
- [Objects365](https://www.objects365.org/) - Detection dataset.
- [Open Images](https://storage.googleapis.com/openimages/web/index.html) - Large detection and localization dataset.

---

## Applications and Demos

### Great categories to build in
- screenshot QA
- browser automation copilots
- invoice and contract extraction
- multimodal customer support
- chart analysis copilots
- accessibility tools
- robotics perception and action
- multimodal RAG for images, PDFs, and video

### Useful open projects
- [ComfyUI](https://github.com/comfyanonymous/ComfyUI) - Important ecosystem for visual model workflows.
- [InvokeAI](https://github.com/invoke-ai/InvokeAI) - Image generation stack, useful alongside multimodal systems.
- [Label Studio](https://github.com/HumanSignal/label-studio) - Data labeling for multimodal training loops.
- [FiftyOne](https://github.com/voxel51/fiftyone) - Dataset inspection and vision evaluation.
- [Unstructured](https://github.com/Unstructured-IO/unstructured) - Document preprocessing for multimodal pipelines.
- [Haystack](https://github.com/deepset-ai/haystack) - RAG framework adaptable to multimodal retrieval.
- [LlamaIndex](https://github.com/run-llama/llama_index) - Retrieval and agents, with multimodal extensions.
- [LangChain](https://github.com/langchain-ai/langchain) - Orchestration stack with multimodal integrations.

---

## Learning Resources

### Repositories and hubs
- [Papers with Code - Vision Language](https://paperswithcode.com/task/visual-question-answering)
- [Hugging Face Multimodal Tasks](https://huggingface.co/tasks)
- [OpenCompass](https://github.com/open-compass/opencompass) - Evaluation ecosystem.
- [LAVIS](https://github.com/salesforce/LAVIS) - Great for studying model families.

### Topics worth learning deeply
- projector-based multimodal alignment
- OCR-free vs OCR-plus-VLM document stacks
- visual grounding for action
- hallucination detection in VLMs
- long-context video reasoning
- multimodal retrieval and indexing

---

## Opinionated Starter Paths

### I want to build a local screenshot copilot
Start with:
- Qwen2-VL or LLaVA-style model
- Ollama or vLLM
- OmniParser or GroundingDINO for UI structure
- Playwright, Browser Use, or Stagehand for actions

### I want to build document AI
Start with:
- MinerU, Marker, Surya, PaddleOCR, or docTR
- Donut or a strong general VLM for semantic reasoning
- multimodal RAG over pages, tables, and extracted markdown

### I want to explore robotics
Start with:
- OpenVLA
- LeRobot
- GroundingDINO + SAM 2
- RT-1 and RT-2 papers for system design

### I want to benchmark models before choosing one
Start with:
- MMMU
- MMBench
- MM-Vet
- HallusionBench
- task-specific evals on your own screenshots or PDFs

---

## What makes a resource a good fit for this repo?

We prioritize resources that are:
- useful for builders, not only for citation graphs
- open or accessible enough to try
- relevant to local deployment, evaluation, or productization
- focused on image, document, video, UI, or grounded multimodal workflows

We do **not** aim to be a giant paper dump.

---

## Contributing

Please read [CONTRIBUTING.md](CONTRIBUTING.md).

Good additions include:
- practical VLM repos
- local runtimes with multimodal support
- document AI tooling
- UI agent frameworks
- evaluation suites
- strong tutorials and implementation guides

---

## License

[MIT](LICENSE)
