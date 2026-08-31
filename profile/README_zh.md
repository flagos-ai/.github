# FlagOS：统一的开源AI系统软件栈

[![GitHub License](https://img.shields.io/github/license/flagos-ai/.github?style=flat-square)](https://github.com/flagos-ai/.github/blob/main/LICENSE) [![Ask DeepWiki](../assets/deepwiki.svg)](https://flagos-wiki.baai.ac.cn/)

**语言:** [English](README.md) | [中文](README_zh.md)

---

## 📖 关于 FlagOS

为解决不同 AI 芯片大规模落地应用，北京智源研究院联合众多科研机构、芯片企业、系统厂商、算法和软件相关单位等国内外机构共同发起并创立了 FlagOS 开源社区。

FlagOS 社区致力于打造面向多种 AI 芯片的统一、开源的系统软件栈，包括大型算子库、统一AI编译器、并行训推框架、统一通信库等核心开源项目，
构建「模型-系统-芯片」三层贯通的开放技术生态，通过“一次开发跨芯迁移”释放硬件计算潜力，打破不同芯片软件栈之间生态隔离，有效降低开发者的迁移成本。
FlagOS 社区构建人工智能软硬件生态，突破单一闭源垄断，推动AI硬件技术大范围落地发展，立足中国、拥抱全球合作。

---

## 🎯 核心组件

组件按归属的 SIG 分组。各 SIG 的章程、负责人与例会安排见 [SIG 总览](https://github.com/flagos-ai/community/tree/main/sigs)。

| SIG | 用途 | 代码仓 |
|-----|------|--------|
| [**sig-operator**](https://github.com/flagos-ai/community/tree/main/sigs/sig-operator) | 算子库：算子实现、性能优化与多芯片适配 | [FlagGems](https://github.com/flagos-ai/FlagGems)、[FlagAttention](https://github.com/flagos-ai/FlagAttention)、[FlagFFT](https://github.com/flagos-ai/FlagFFT)、[FlagSparse](https://github.com/flagos-ai/FlagSparse)、[FlagDNN](https://github.com/flagos-ai/FlagDNN)、[FlagBLAS](https://github.com/flagos-ai/FlagBLAS)、[FlagTensor](https://github.com/flagos-ai/FlagTensor)、[FlagAudio](https://github.com/flagos-ai/FlagAudio) |
| [**sig-compiler**](https://github.com/flagos-ai/community/tree/main/sigs/sig-compiler) | 统一AI编译器：IR 设计、优化 pass 与多芯片代码生成 | [FlagTree](https://github.com/flagos-ai/FlagTree) |
| [**sig-network**](https://github.com/flagos-ai/community/tree/main/sigs/sig-network) | 统一通信库：集合通信与多芯片、多机通信调优 | [FlagCX](https://github.com/flagos-ai/FlagCX) |
| [**sig-framework**](https://github.com/flagos-ai/community/tree/main/sigs/sig-framework) | 框架适配层：PyTorch、vLLM、SGLang、TransformerEngine、Megatron-LM、veRL | [Torch-FL](https://github.com/flagos-ai/Torch-FL)、[vllm-plugin-FL](https://github.com/flagos-ai/vllm-plugin-FL)、[sglang-plugin-FL](https://github.com/flagos-ai/sglang-plugin-FL)、[TransformerEngine-FL](https://github.com/flagos-ai/TransformerEngine-FL)、[Megatron-LM-FL](https://github.com/flagos-ai/Megatron-LM-FL)、[verl-FL](https://github.com/flagos-ai/verl-FL) |
| [**sig-training**](https://github.com/flagos-ai/community/tree/main/sigs/sig-training) | 训推编排：并行策略、训练配方与 Hugging Face 生态集成 | [FlagScale](https://github.com/flagos-ai/FlagScale) |
| [**sig-kernelgen**](https://github.com/flagos-ai/community/tree/main/sigs/sig-kernelgen) | 大模型辅助算子代码生成及其评测 | [KernelGen](https://github.com/flagos-ai/KernelGen)、[KernelGenBench](https://github.com/flagos-ai/KernelGenBench) |
| [**sig-chip**](https://github.com/flagos-ai/community/tree/main/sigs/sig-chip) | 数据中心芯片适配：厂商 SDK 集成、芯片使能与多芯片 CI | 无独立代码仓，适配工作落在上述各模块仓库 |
| [**wg-embodied**](https://github.com/flagos-ai/community/tree/main/wg/wg-embodied) *(孵化中)* | 机器人与具身智能 | [FlagOS-Robo](https://github.com/flagos-ai/FlagOS-Robo) |
| [**wg-ai4s**](https://github.com/flagos-ai/community/tree/main/wg/wg-ai4s) *(孵化中)* | AI for Science，含量子模拟 | [FlagQuantum](https://github.com/flagos-ai/FlagQuantum) |
| [**sig-tools**](https://github.com/flagos-ai/community/blob/main/sigs/_planned/sig-tools.md) *(筹备中)* | 发布管理工具链 | [FlagRelease](https://github.com/flagos-ai/FlagRelease) |
| [**sig-agent**](https://github.com/flagos-ai/community/blob/main/sigs/_planned/sig-agent.md) *(筹备中)* | 支持 Agent 在特定领域完成任务的技能包 | [skills](https://github.com/flagos-ai/skills) |
| [**sig-benchmark**](https://github.com/flagos-ai/community/blob/main/sigs/_planned/sig-benchmark.md) *(筹备中)* | 多芯片性能基准评测 | [FlagPerf](https://github.com/flagos-ai/FlagPerf) |

---

## 🚀 扩展生态组件

### 开发者工具与实用程序

- **[KernelGenBench](https://github.com/flagos-ai/KernelGenBench) **: 用于跨多芯片平台评估 LLM 和基于 Agent 的 Triton 算子生成的基准测试框架

- **[libtriton_jit](https://github.com/flagos-ai/libtriton_jit)**: Triton JIT C++ 运行时，用于降低 Python 开销

### 框架增强

- **[Megatron-LM-FL](https://github.com/flagos-ai/Megatron-LM-FL)**: 大规模 Transformer 模型训练的 GPU 优化库

- **[TransformerEngine-FL](https://github.com/flagos-ai/TransformerEngine-FL)**: Transformer 模型的 FP8 混合精度训练

- **[verl-FL](https://github.com/flagos-ai/verl-FL)**: verl 的一个派生版本，在 FlagOS 之上实现对多种 AI 加速器的支持

- **[Torch-FL](https://github.com/flagos-ai/Torch-FL)**: 基于 `PrivateUse` 扩展机制实现的一款定制的 PyTorch 设备插件，将 FlagGems 所实现的高性能 Triton 算子注册为 flagos 设备后端，进而支持多款 AI 芯片。


### 推理与服务

- **[vllm-plugin-FL](https://github.com/flagos-ai/vllm-plugin-FL)**: 增强型 vLLM 插件，提供更好的多芯片支持

- **[sglang-plugin-FL](https://github.com/flagos-ai/sglang-plugin-FL)**: SGLang 的一款树外（Out-of-tree，OOT）插件，基于 FlagOS 的统一多芯片支持能力构建

### 特定领域算子库

- **[FlagDNN](https://github.com/flagos-ai/FlagDNN)**：面向多种后端芯片的神经网络计算库。

- **[FlagBLAS](https://github.com/flagos-ai/FlagBLAS)**：面向多种后端芯片的计算库，遵从 BLAS 标准接口。

- **[FlagFFT](https://github.com/flagos-ai/FlagFFT)**：针对多种后端芯片开发的一组算法，用于将跨时域/空域与频域完成信号或数据的转换。

- **[FlagSparse](https://github.com/flagos-ai/FlagSparse)**：稀疏矩阵运算算子（如 SpMV, gather, scatter, sparse formats 等），用于多种芯片后端。

- **[FlagTensor](https://github.com/flagos-ai/FlagTensor)**：面向多芯片后端开发的一组高性能张量操作算子。

- **[FlagAudio](https://github.com/flagos-ai/FlagAudio)**：可运行于多种芯片之上的一组高性能的音频数据处理算子。

- **[FlagAttention](https://github.com/flagos-ai/FlagAttention)**：包含高效访存注意力算子的一个软件包，起源于对多头注意力机制的扩展。
- 
- **[FlagGems-vLLM](https://github.com/flagos-ai/FlagGems-vllm)**：对常用 vLLM 算子的优化实现集合，支持多种常用模型的高性能推理与部署。

### 社区与资源

- **[EasyOfUse](https://github.com/flagos-ai/EasyOfUse)**: 为开放计算简化开发 - 即插即用的解决方案和最佳实践

- **[Community](https://github.com/flagos-ai/community)**: FlagOS社区治理、贡献指南和交流枢纽

---

## 📚 文档与资源

### 知识库
- **FlagOS Wiki & 文档**: [DeepWiki门户](https://flagos-wiki.baai.ac.cn/)
- **最新v1.5版本**: [发布公告](https://mp.weixin.qq.com/s/BCryw30j_eMwe0Pr80VtcA)

### 模型仓库
- **ModelScope**: [FlagRelease模型](https://modelscope.cn/organization/FlagRelease)
- **Hugging Face**: [FlagRelease模型](https://huggingface.co/FlagRelease/models)
- **WiseModel**: [FlagRelease模型](https://www.wisemodel.cn/organization/FlagRelease)

### 社区频道
- **微信公众号**: FlagOpen
- **微信视频号**: FlagOpen

---

## 🌐 加入社区

**准备好做贡献或想了解更多?** 访问 [FlagOS 社区仓库](https://github.com/flagos-ai/community) 获取：
- 📖 完整的贡献指南
- 💬 社区讨论和支持
- 🤝 参与方式
- 📚 资源和文档

---

## 💕 参与贡献

我们欢迎来自社区的贡献！无论是点星、Fork还是提交Pull Request，您的参与都能帮助FlagOS变得更好。

- ⭐ **点击Star** - 表示您的支持！
- 🔔 **Watch** - 获取我们最新版本的更新
- 🍴 **Fork** - 开始贡献！

### 行为准则
请阅读并遵守我们的行为准则：
- **[行为准则](https://github.com/flagos-ai/community/blob/main/CODE_OF_CONDUCT_CN.MD)** (中文)

---

## 📄 许可证

FlagOS及其所有组件均遵循Apache License 2.0许可。详见各代码仓。

---

## 🤝 合作伙伴与贡献者

FlagOS由芯片制造、系统软件和AI研究领域的领先组织联合支持。这一合作努力证明了构建一个开放、统一的AI系统软件生态，跨越多样化硬件平台的承诺。

---

**加入我们，共同构建AI系统软件的未来！🚀**
