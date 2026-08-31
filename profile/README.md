# FlagOS: A Unified, Open-Source AI System Software Stack

[![GitHub License](https://img.shields.io/github/license/flagos-ai/.github?style=flat-square)](https://github.com/flagos-ai/.github/blob/main/LICENSE) 

**Language:** [English](README.md) | [中文](README_zh.md)

---

## 📖 About FlagOS

FlagOS is a unified, open-source AI system software stack designed for multi-chip scenarios. It was jointly initiated and established by over ten domestic and international organizations, including chip companies, system manufacturers, algorithm and software-related entities, non-profit organizations, and research institutions.

Addressing core pain points in utilizing diverse AI chips, FlagOS builds a comprehensive system software ecosystem that demonstrates the potential to break down ecosystem barriers between different chip software stacks, effectively reducing migration costs for developers.

---

## 🎯 Core Components

Components are grouped by the SIG that owns them. See the [SIG overview](https://github.com/flagos-ai/community/tree/main/sigs) for charters, owners, and meeting calendars.

<table>
<thead>
<tr>
<th>SIG</th>
<th>Purpose</th>
<th>Repository</th>
</tr>
</thead>
<tbody>
<tr>
<td><a href="https://github.com/flagos-ai/community/tree/main/sigs/sig-operator"><strong>sig-operator</strong></a></td>
<td>Operator libraries: implementation, performance optimization, and multi-chip adaptation, including framework-facing fused operator packages</td>
<td>
<a href="https://github.com/flagos-ai/FlagGems">FlagGems</a><br />
<a href="https://github.com/flagos-ai/FlagGems-vllm">FlagGems-vllm</a><br />
<a href="https://github.com/flagos-ai/FlagGems-sglang">FlagGems-sglang</a><br />
<a href="https://github.com/flagos-ai/FlagAttention">FlagAttention</a><br />
<a href="https://github.com/flagos-ai/FlagFFT">FlagFFT</a><br />
<a href="https://github.com/flagos-ai/FlagSparse">FlagSparse</a><br />
<a href="https://github.com/flagos-ai/FlagDNN">FlagDNN</a><br />
<a href="https://github.com/flagos-ai/FlagBLAS">FlagBLAS</a><br />
<a href="https://github.com/flagos-ai/FlagTensor">FlagTensor</a><br />
<a href="https://github.com/flagos-ai/FlagAudio">FlagAudio</a>
</td>
</tr>
<tr>
<td><a href="https://github.com/flagos-ai/community/tree/main/sigs/sig-compiler"><strong>sig-compiler</strong></a></td>
<td>Unified AI compiler: IR design, optimization passes, and multi-chip code generation</td>
<td><a href="https://github.com/flagos-ai/FlagTree">FlagTree</a></td>
</tr>
<tr>
<td><a href="https://github.com/flagos-ai/community/tree/main/sigs/sig-network"><strong>sig-network</strong></a></td>
<td>Unified communication library: collective communication and multi-chip, multi-node tuning</td>
<td><a href="https://github.com/flagos-ai/FlagCX">FlagCX</a></td>
</tr>
<tr>
<td><a href="https://github.com/flagos-ai/community/tree/main/sigs/sig-framework"><strong>sig-framework</strong></a></td>
<td>Framework adapter layer for PyTorch, vLLM, SGLang, TransformerEngine, Megatron-LM, and veRL</td>
<td>
<a href="https://github.com/flagos-ai/Torch-FL">Torch-FL</a><br />
<a href="https://github.com/flagos-ai/vllm-plugin-FL">vllm-plugin-FL</a><br />
<a href="https://github.com/flagos-ai/sglang-plugin-FL">sglang-plugin-FL</a><br />
<a href="https://github.com/flagos-ai/TransformerEngine-FL">TransformerEngine-FL</a><br />
<a href="https://github.com/flagos-ai/Megatron-LM-FL">Megatron-LM-FL</a><br />
<a href="https://github.com/flagos-ai/verl-FL">verl-FL</a>
</td>
</tr>
<tr>
<td><a href="https://github.com/flagos-ai/community/tree/main/sigs/sig-training"><strong>sig-training</strong></a></td>
<td>Training and inference orchestration: parallelism strategies, recipes, and Hugging Face integration</td>
<td><a href="https://github.com/flagos-ai/FlagScale">FlagScale</a></td>
</tr>
<tr>
<td><a href="https://github.com/flagos-ai/community/tree/main/sigs/sig-kernelgen"><strong>sig-kernelgen</strong></a></td>
<td>AI-assisted kernel code generation and its evaluation</td>
<td>
<a href="https://github.com/flagos-ai/KernelGen">KernelGen</a><br />
<a href="https://github.com/flagos-ai/KernelGenBench">KernelGenBench</a>
</td>
</tr>
<tr>
<td><a href="https://github.com/flagos-ai/community/tree/main/sigs/sig-chip"><strong>sig-chip</strong></a></td>
<td>Datacenter chip adaptation: vendor SDK integration, bring-up, and multi-chip CI</td>
<td>No dedicated repository; adaptation lands in the module repositories above</td>
</tr>
<tr>
<td><a href="https://github.com/flagos-ai/community/tree/main/wg/wg-embodied"><strong>wg-embodied</strong></a> <em>(incubating)</em></td>
<td>Robotics and embodied intelligence</td>
<td><a href="https://github.com/flagos-ai/FlagOS-Robo">FlagOS-Robo</a></td>
</tr>
<tr>
<td><a href="https://github.com/flagos-ai/community/tree/main/wg/wg-ai4s"><strong>wg-ai4s</strong></a> <em>(incubating)</em></td>
<td>AI for Science, including quantum simulation</td>
<td><a href="https://github.com/flagos-ai/FlagQuantum">FlagQuantum</a></td>
</tr>
<tr>
<td><a href="https://github.com/flagos-ai/community/blob/main/sigs/_planned/sig-tools.md"><strong>sig-tools</strong></a> <em>(planned)</em></td>
<td>Release management toolchain</td>
<td><a href="https://github.com/flagos-ai/FlagRelease">FlagRelease</a></td>
</tr>
<tr>
<td><a href="https://github.com/flagos-ai/community/blob/main/sigs/_planned/sig-agent.md"><strong>sig-agent</strong></a> <em>(planned)</em></td>
<td>Skill packages for agents to complete tasks in a specific domain</td>
<td><a href="https://github.com/flagos-ai/skills">skills</a></td>
</tr>
<tr>
<td><a href="https://github.com/flagos-ai/community/blob/main/sigs/_planned/sig-benchmark.md"><strong>sig-benchmark</strong></a> <em>(planned)</em></td>
<td>Multi-chip performance benchmarking and evaluation</td>
<td><a href="https://github.com/flagos-ai/FlagPerf">FlagPerf</a></td>
</tr>
</tbody>
</table>

---

## 🚀 Extended Ecosystem Components

### Developer Tools & Utilities

- **[KernelGenBench](https://github.com/flagos-ai/KernelGenBench)**: A benchmark framework for evaluating LLM and agent-based Triton kernel generation across multiple hardware platforms.

- **[libtriton_jit](https://github.com/flagos-ai/libtriton_jit)**: Triton JIT C++ runtime for reduced Python overhead.

### Framework Enhancements

- **[Megatron-LM-FL](https://github.com/flagos-ai/Megatron-LM-FL)**: GPU-optimized library for training transformer models at scale

- **[TransformerEngine-FL](https://github.com/flagos-ai/TransformerEngine-FL)**: FP8 mixed precision training for transformer models

- **[verl-FL](https://github.com/flagos-ai/verl-FL)**: A fork of verl designed to support diverse AI accelerators, built on top of FlagOS.

- **[Torch-FL](https://github.com/flagos-ai/Torch-FL)**: A custom PyTorch device plugin based on the `PrivateUse1` extension mechanism, registering FlagGems high-performance Triton operators as the flagos device backend for unified multi-chip support.

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
