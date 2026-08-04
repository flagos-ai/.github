# FlagOS: A Unified, Open-Source AI System Software Stack

[![GitHub License](https://img.shields.io/github/license/flagos-ai/.github?style=flat-square)](https://github.com/flagos-ai/.github/blob/main/LICENSE) 

**Language:** [English](README.md) | [中文](README_zh.md)

---

## 📖 About FlagOS

FlagOS is a unified, open-source AI system software stack designed for multi-chip scenarios. It was jointly initiated and established by over ten domestic and international organizations, including chip companies, system manufacturers, algorithm and software-related entities, non-profit organizations, and research institutions.

Addressing core pain points in utilizing diverse AI chips, FlagOS builds a comprehensive system software ecosystem that demonstrates the potential to break down ecosystem barriers between different chip software stacks, effectively reducing migration costs for developers.

---

## 🎯 Core Components

| Component | Purpose | Repository |
|-----------|---------|-----------|
| **FlagGems** | High-performance universal AI operator library | [FlagGems](https://github.com/flagos-ai/FlagGems) |
| **FlagTree** | Unified AI compiler | [FlagTree](https://github.com/flagos-ai/flagtree) |
| **FlagScale** | Unified parallel training and inference framework | [FlagScale](https://github.com/flagos-ai/FlagScale) |
| **FlagCX** | Unified communication library | [FlagCX](https://github.com/flagos-ai/FlagCX) |
| **FlagPerf** | Multi-chip evaluation tool | [FlagPerf](https://github.com/flagos-ai/FlagPerf) |
| **FlagRelease** | Large model release platform | [FlagRelease](https://github.com/flagos-ai/FlagRelease) |
| **KernelGen** | AI enabled operator develop tool | [KernelGen](https://github.com/flagos-ai/kernelgen) |
| **FlagOS-Robo** | End-to-end toolkit for embodied intelligence | [FlagOS-Robo](https://github.com/flagos-ai/FlagOS-Robo) |
| **FlagQuantum** | A high-performance distributed quantum statevector simulator | [FlagQuantum](https://github.com/flagos-ai/FlagQuantum) |
| **FlagOS skills** | Skill packages for agents to complete tasks in a specific domain. | [FlagOS skills](https://github.com/flagos-ai/skills) |

---

## 🚀 Extended Ecosystem Components

### Developer Tools & Utilities

- **[KernelGenBench](https://github.com/flagos-ai/KernelGenBench)**: A benchmark framework for evaluating LLM and agent-based Triton kernel generation across multiple hardware platforms.

- **[libtriton_jit](https://github.com/flagos-ai/libtriton_jit)**: Triton JIT C++ runtime for reduced Python overhead.

### Framework Enhancements

- **[Megatron-LM-FL](https://github.com/flagos-ai/Megatron-LM-FL)**: GPU-optimized library for training transformer models at scale

- **[TransformerEngine-FL](https://github.com/flagos-ai/TransformerEngine-FL)**: FP8 mixed precision training for transformer models

- **[verl-FL](https://github.com/flagos-ai/verl-FL)**: A fork of verl designed to support diverse AI accelerators, built on top of FlagOS.

- **[PyTorch-Plugin-FL](https://github.com/flagos-ai/PyTorch-Plugin-FL))**: A custom PyTorch device plugin based on the `PrivateUse1` extension mechanism, registering FlagGems high-performance Triton operators as the flagos device backend for unified multi-chip support.

### Inference & Serving

- **[vLLM-plugin-FL](https://github.com/flagos-ai/vllm-plugin-FL)**: Advanced vLLM plugin for enhanced multi-chip support

- **[sglang-plugin-FL](https://github.com/flagos-ai/sglang-plugin-FL)**: An out-of-tree (OOT) plugin for SGLang, built on FlagOS's unified multi-chip backend 

### Domain-specific Operator Libraries

- **[FlagDNN](https://github.com/flagos-ai/FlagDNN)**: A deep neural network computing library oriented towards multiple chip backends.

- **[FlagBLAS](https://github.com/flagos-ai/FlagBLAS)**: A computing library that follows the BLAS standard interface and is oriented towards multiple chip backends.

- **[FlagFFT](https://github.com/flagos-ai/FlagFFT)**: Efficient algorithms that convert signals or data between the time/spatial domain and the frequency domain in
operations targeting multiple chip backends.

- **[FlagSparse](https://github.com/flagos-ai/FlagSparse)**: A package for sparse operations (SpMV, gather, scatter, sparse formats) targeting multiple chip backends.

- **[FlagTensor](https://github.com/flagos-ai/FlagTensor)**: A package for high-performance tensor operators targeting multiple chip backends.

- **[FlagAudio](https://github.com/flagos-ai/FlagAudio)**: A package for high-performance audio data processing targeting multiple chip backends.

- **[FlagAttention](https://github.com/flagos-ai/FlagAttention)**: A package for memory-efficient attention operators, initiated as an extension of multi-head attention.

- **[FlagGems-vLLM](https://github.com/flagos-ai/FlagGems-vllm)**: A collection of optimized implementations of common vLLM operators and supports high-performance inference and deployment for a variety of widely used models.

### Community & Resources

- **[EasyOfUse](https://github.com/flagos-ai/EasyOfUse)**: Simplify development for open compute - plug-and-play solutions and best practices.

- **[Community](https://github.com/flagos-ai/community)**: FlagOS community governance, contribution guides, and communication hub.

---

## 📚 Documentation & Resources

### Knowledge Base

- **FlagOS Wiki & Documentation**: [DeepWiki Portal](https://flagos-wiki.baai.ac.cn/)
- **Latest Release v1.5**: [Announcement](https://mp.weixin.qq.com/s/BCryw30j_eMwe0Pr80VtcA)

### Model Repositories

- **ModelScope**: [FlagRelease Models](https://modelscope.cn/organization/FlagRelease)
- **Hugging Face**: [FlagRelease Models](https://huggingface.co/FlagRelease/models)
- **WiseModel**: [FlagRelease Models](https://www.wisemodel.cn/organization/FlagRelease)

### Community Channels

- **WeChat Official Account**: FlagOpen
- **WeChat Channels Account**: FlagOpen

---

## 🌐 Join the Community

**Ready to contribute or learn more?** Visit the [FlagOS Community Repository](https://github.com/flagos-ai/community) for:
- 📖 Comprehensive contribution guidelines
- 💬 Community discussions and support
- 🤝 Ways to get involved
- 📚 Resources and documentation

---

## 💕 Contributing

We welcome contributions from the community! Whether through starring, forking, or submitting pull requests, your involvement helps make FlagOS better.

- ⭐ **Star** - Show your support!
- 🔔 **Watch** - Stay updated with our latest releases
- 🍴 **Fork** - Start contributing!

### Code of Conduct
Please read and respect our Code of Conduct:
- **[Code of Conduct](https://github.com/flagos-ai/community/blob/main/CODE_OF_CONDUCT.MD)** (English)

---

## 📄 License

FlagOS and its components are licensed under the Apache License 2.0. See individual repositories for details.

---

## 🤝 Partners & Contributors

FlagOS is jointly supported by leading organizations in chip manufacturing, system software, and AI research. This collaborative effort demonstrates the commitment to building an open, unified ecosystem for AI system software across diverse hardware platforms.

---

**Join us in building the future of AI system software! 🚀**
