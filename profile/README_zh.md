# FlagOS：统一的开源AI系统软件栈

[![GitHub License](https://img.shields.io/github/license/flagos-ai/.github?style=flat-square)](https://github.com/flagos-ai/.github/blob/main/LICENSE) [![Ask DeepWiki](../assets/deepwiki.svg)](https://flagos-wiki.baai.ac.cn/)

**语言:** [English](README.md) | [中文](README_zh.md)

---

## 📖 关于 FlagOS

为解决不同 AI 芯片大规模落地应用，北京智源研究院联合众多科研机构、芯片企业、系统厂商、算法和软件相关单位等国内外机构共同发起并创立了 FlagOS 开源社区。

FlagOS 社区致力于打造面向多种 AI 芯片的统一、开源的系统软件栈，包括大型算子库、统一AI编译器、并行训推框架、统一通信库等核心开源项目，构建「模型-系统-芯片」三层贯通的开放技术生态，通过“一次开发跨芯迁移”释放硬件计算潜力，打破不同芯片软件栈之间生态隔离，有效降低开发者的迁移成本。FlagOS 社区构建人工智能软硬件生态，突破单一闭源垄断，推动AI硬件技术大范围落地发展，立足中国、拥抱全球合作。

---

## 🎯 核心组件

| 组件 | 用途 | 代码仓 |
|------|------|--------|
| **FlagGems** | 高性能通用AI算子库 | [FlagGems](https://github.com/flagos-ai/FlagGems) |
| **FlagTree** | 统一AI编译器 | [FlagTree](https://github.com/flagos-ai/flagtree) |
| **FlagScale** | 统一并行训练和推理框架 | [FlagScale](https://github.com/flagos-ai/FlagScale) |
| **FlagCX** | 统一通信库 | [FlagCX](https://github.com/flagos-ai/FlagCX) |
| **FlagPerf** | 多芯片评测工具 | [FlagPerf](https://github.com/flagos-ai/FlagPerf) |
| **FlagRelease** | 大模型发布平台 | [FlagRelease](https://github.com/flagos-ai/FlagRelease) |
| **Triton-Copilot** | 大模型辅助算子开发工具 | [Triton-Copilot](https://triton-copilot.flagos.io) |

---

## 🚀 扩展生态组件

### 开发者工具与实用程序
- **TritonCopilot**: 为多芯片系统设计的下一代AI辅助内核工程工具
  → [TritonCopilot](https://github.com/flagos-ai/triton-copilot)

- **libtriton_jit**: Triton JIT C++运行时，用于降低Python开销
  → [libtriton_jit](https://github.com/flagos-ai/libtriton_jit)

### 框架增强
- **Megatron-LM-FL**: 大规模Transformer模型训练的GPU优化库
  → [Megatron-LM-FL](https://github.com/flagos-ai/Megatron-LM-FL)

- **TransformerEngine-FL**: Transformer模型的FP8混合精度训练
  → [TransformerEngine-FL](https://github.com/flagos-ai/TransformerEngine-FL)

### 推理与服务
- **vllm-FL**: 基于FlagOS统一多芯片后端的vLLM插件，用于LLM服务
  → [vllm-FL](https://github.com/flagos-ai/vllm-FL)

- **vllm-plugin-FL**: 增强型vLLM插件，提供更好的多芯片支持
  → [vllm-plugin-FL](https://github.com/flagos-ai/vllm-plugin-FL)

### 社区与资源
- **EasyOfUse**: 为开放计算简化开发 - 即插即用的解决方案和最佳实践
  → [EasyOfUse](https://github.com/flagos-ai/EasyOfUse)

- **Community**: FlagOS社区治理、贡献指南和交流枢纽
  → [Community](https://github.com/flagos-ai/community)

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
