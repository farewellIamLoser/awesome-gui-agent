<div align="center">
  <h1>Awesome GUI Agent</h1>
  <p>A curated collection of papers, benchmarks and resources for <b>GUI Agents</b> &amp; <b>Computer-Use Agents</b></p>
  <p>
    <a href="https://github.com/sindresorhus/awesome"><img src="https://awesome.re/badge.svg" alt="Awesome"></a>
  </p>
  <p>
    <a href="https://github.com/farewellIamLoser/awesome-gui-agent/stargazers"><img src="https://img.shields.io/github/stars/farewellIamLoser/awesome-gui-agent?style=flat&color=yellow" alt="Stars"></a>
    <a href="https://github.com/farewellIamLoser/awesome-gui-agent/commits/main"><img src="https://img.shields.io/github/last-commit/farewellIamLoser/awesome-gui-agent?style=flat" alt="Last commit"></a>
    <a href="https://github.com/farewellIamLoser/awesome-gui-agent/pulls"><img src="https://img.shields.io/badge/PRs-welcome-brightgreen?style=flat" alt="PRs welcome"></a>
    <img src="https://img.shields.io/badge/papers-274-blue?style=flat" alt="Papers">
  </p>
</div>

> A curated, regularly updated list of papers, code and benchmarks on **GUI agents**: (multimodal) LLM-based agents that perceive screens and operate **web, mobile and desktop** interfaces like humans do. It covers
> - Native GUI agent models and GUI grounding
> - Agent frameworks (prompting, multi-agent, memory) for Web / Mobile / Desktop
> - Reinforcement learning, data synthesis and world models for GUI agents
> - Benchmarks, datasets, and safety & security of computer-use agents
> - Backdoor attacks & defenses for GUI agents, LLM agents and VLMs
>
> 📌 An inline tag after a title, e.g. `Mobile`, marks the main platform. A grey badge, e.g. <sub>![ScreenSpot](https://img.shields.io/badge/ScreenSpot-grey)</sub>, names the dataset/benchmark that paper introduces. A plain **Code** without a link means the code has not been released (or we have not found it).
>
> 🔄 Updated regularly. Missing a paper? Open an issue or PR (see [CONTRIBUTING.md](CONTRIBUTING.md)).


<details>
<summary><strong>:loudspeaker: Latest Updates</strong></summary>

- 2026.11 · New section **Backdoor Attacks & Defenses** (110 papers): GUI-agent backdoors, data-free implantation, label-only poisoning, state-triggered backdoors, detection & benchmarks
- 2026.11 · Initial release: 163 papers covering surveys, models, grounding, frameworks, RL, data, world models, benchmarks and safety (up to ICLR 2026, AAAI 2026, CVPR 2026, ACL 2026)
</details>


--------------------------------------------------------------------------------------

<!--TOC-->

## 📋 Table of Contents
- [Recent Featured Papers](#-recent-featured-papers)
- [Survey Papers](#survey-papers)
- **Models**
  - [Native GUI Agent Models](#native-models)
  - [GUI Grounding & Screen Understanding](#gui-grounding)
- **Agent Systems**
  - [Agent Frameworks (Prompting / Multi-agent / Memory)](#agent-frameworks)
  - [World Models & Planning](#world-models)
- **Training**
  - [Reinforcement Learning & Self-Evolution](#reinforcement-learning)
  - [Data & Trajectory Synthesis](#data-synthesis)
- [Safety & Security](#safety)
- **Backdoor Attacks & Defenses**
  - [GUI / Mobile / Computer-Use Agents](#bd-gui)
  - [General LLM Agents & VLMs](#bd-agent)
  - [Implantation without Training Data](#bd-nodata)
  - [Clean-Input, Label-Only Poisoning](#bd-label)
  - [Triggers Beyond the Input](#bd-state)
  - [Detection, Defense & Benchmarks](#bd-defense)
- **Benchmarks & Datasets**
  - [Web](#bench-web)
  - [Mobile](#bench-mobile)
  - [Desktop / OS](#bench-desktop)
  - [Cross-platform](#bench-cross)
  - [GUI Grounding & Understanding](#bench-grounding)
- [Open-source Projects](#projects)
- [Commercial Systems](#products)
- [Related Awesome Lists](#reference)


--------------------------------------------------------------------------------------


## 🔥 Recent Featured Papers
<!-- Venue chip colours: NeurIPS bf3989 · ICML 8250df · ICLR 1f6feb · CVPR d1242f · ICCV e16f24 · ECCV a40e26 · ACL b8860b · AAAI 6e40c9 · TMLR 0e8a6b · COLM 1b7f8c · ACMMM c2410c -->

| **Venue** | **Paper** | **Links** |
| :------: | :----------------------------------------------------------- | :------: |
| ![arXiv 2025](https://img.shields.io/badge/arXiv-2025-b31b1b?style=flat-square) | **UI-TARS-2 Technical Report: Advancing GUI Agent with Multi-Turn Reinforcement Learning** `UI-TARS-2` <br><sub>Haoming Wang, Haoyang Zou, Huatong Song, Jiazhan Feng, Junjie Fang, Junting Lu, et al.</sub> | [Paper](https://arxiv.org/abs/2509.02544) · [Code](https://github.com/bytedance/UI-TARS) |
| ![NeurIPS 2025](https://img.shields.io/badge/NeurIPS-2025-bf3989?style=flat-square) | **OpenCUA: Open Foundations for Computer-Use Agents** `OpenCUA` <br><sub>Xinyuan Wang, Bowen Wang, Dunjie Lu, Junlin Yang, Tianbao Xie, Junli Wang, et al.</sub> | [Paper](https://arxiv.org/abs/2508.09123) · [Code](https://github.com/xlang-ai/OpenCUA) |
| ![TMLR 2026](https://img.shields.io/badge/TMLR-2026-0e8a6b?style=flat-square) | **Scaling Agents for Computer Use** `Agent S3` <br><sub>Gonzalo Gonzalez-Pumariega, Vincent Tu, Chih-Lun Lee, Jiachen Yang, Ang Li, Xin Eric Wang</sub> | [Paper](https://arxiv.org/abs/2510.02250) · [Code](https://github.com/simular-ai/Agent-S) |
| ![CVPR 2026](https://img.shields.io/badge/CVPR-2026-d1242f?style=flat-square) | **UI-AGILE: Advancing GUI Agents with Effective Reinforcement Learning and Precise Inference-Time Grounding** `UI-AGILE` <br><sub>Shuquan Lian, Yuhang Wu, Jia Ma, Yifan Ding, Zihan Song, Bingqi Chen, et al.</sub> | [Paper](https://arxiv.org/abs/2507.22025) · [Code](https://github.com/KDEGroup/UI-AGILE) |
| ![ICLR 2026](https://img.shields.io/badge/ICLR-2026-1f6feb?style=flat-square) | **CoAct-1: Computer-using Multi-Agent System with Coding Actions** `CoAct-1` <br><sub>Linxin Song, Yutong Dai, Viraj Prabhu, Jieyu Zhang, Taiwei Shi, Li Li, et al.</sub> | [Paper](https://arxiv.org/abs/2508.03923) · Code |
| ![ICLR 2026](https://img.shields.io/badge/ICLR-2026-1f6feb?style=flat-square) | **ScienceBoard: Evaluating Multimodal Autonomous Agents in Realistic Scientific Workflows** `ScienceBoard` <br><sub>Qiushi Sun, Zhoumianze Liu, Chang Ma, Zichen Ding, Fangzhi Xu, Zhangyue Yin, et al.</sub> | [Paper](https://arxiv.org/abs/2505.19897) · [Code](https://github.com/OS-Copilot/ScienceBoard) |
| ![arXiv 2025](https://img.shields.io/badge/arXiv-2025-b31b1b?style=flat-square) | **Mobile-Agent-v3: Fundamental Agents for GUI Automation** `GUI-Owl` <br><sub>Jiabo Ye, Xi Zhang, Haiyang Xu, Haowei Liu, Junyang Wang, Zhaoqing Zhu, et al.</sub> | [Paper](https://arxiv.org/abs/2508.15144) · [Code](https://github.com/X-PLUG/MobileAgent) |
| ![NeurIPS 2025](https://img.shields.io/badge/NeurIPS-2025-bf3989?style=flat-square) | **Scaling Computer-Use Grounding via User Interface Decomposition and Synthesis** `Jedi` <br><sub>Tianbao Xie, Jiaqi Deng, Xiaochuan Li, Junlin Yang, Haoyuan Wu, Jixuan Chen, et al.</sub> | [Paper](https://arxiv.org/abs/2505.13227) · [Code](https://github.com/xlang-ai/OSWorld-G) |
| ![NeurIPS 2025](https://img.shields.io/badge/NeurIPS-2025-bf3989?style=flat-square) | **GUI-Actor: Coordinate-Free Visual Grounding for GUI Agents** `GUI-Actor` <br><sub>Qianhui Wu, Kanzhi Cheng, Rui Yang, Chaoyun Zhang, Jianwei Yang, Huiqiang Jiang, et al.</sub> | [Paper](https://arxiv.org/abs/2506.03143) · [Code](https://github.com/microsoft/GUI-Actor) |
| ![ACM MM 2025](https://img.shields.io/badge/ACM_MM-2025-c2410c?style=flat-square) | **ScreenSpot-Pro: GUI Grounding for Professional High-Resolution Computer Use** `ScreenSpot-Pro` <br><sub>Kaixin Li, Ziyang Meng, Hongzhan Lin, Ziyang Luo, Yuchen Tian, Jing Ma, et al.</sub> | [Paper](https://arxiv.org/abs/2504.07981) · [Code](https://github.com/likaixin2000/ScreenSpot-Pro-GUI-Grounding) |


--------------------------------------------------------------------------------------


<details open>
<summary><h2 id="survey-papers">📚 Survey Papers</h2></summary>

| **Year** | **Pub.** | **Title**          | **Links**        |
| :------: | :------: | :----------------------------------------------------------- |  :----------------------------------------------------------- |
| 2026 | JAIR | A Comprehensive Survey of Agents for Computer Use: Foundations, Challenges, and Future Directions <br> <sup><sub>*Pascal J. Sager, Benjamin Meyer, Peng Yan, Rebekka von Wartburg-Kottler, Layan Etaiwi, Aref Enayati, Gabriel Nobel, Ahmed Abdulkadir, et al.*</sub></sup> | [Paper](https://arxiv.org/abs/2501.16150) |
| 2025 | ACL | OS Agents: A Survey on MLLM-based Agents for General Computing Devices Use <br> <sup><sub>*Xueyu Hu, Tao Xiong, Biao Yi, Zishu Wei, Ruixuan Xiao, Yurun Chen, Jiasheng Ye, Meiling Tao, et al.*</sub></sup> | [Paper](https://arxiv.org/abs/2508.04482)\|[Res.](https://github.com/OS-Agent-Survey/OS-Agent-Survey) |
| 2025 | ACL Findings | GUI Agents: A Survey <br> <sup><sub>*Dang Nguyen, Jian Chen, Yu Wang, Gang Wu, Namyong Park, Zhengmian Hu, Hanjia Lyu, Junda Wu, et al.*</sub></sup> | [Paper](https://arxiv.org/abs/2412.13501) |
| 2025 | arXiv | A Survey on (M)LLM-Based GUI Agents <br> <sup><sub>*Fei Tang, Haolei Xu, Hang Zhang, Siqi Chen, Xingyu Wu, Yongliang Shen, Wenqi Zhang, Guiyang Hou, et al.*</sub></sup> | [Paper](https://arxiv.org/abs/2504.13865) |
| 2025 | arXiv | Towards Trustworthy GUI Agents: A Survey <br> <sup><sub>*Yucheng Shi, Wenhao Yu, Jingyuan Huang, Wenlin Yao, Wenhu Chen, Ninghao Liu*</sub></sup> | [Paper](https://arxiv.org/abs/2503.23434) |
| 2024 | arXiv | Large Language Model-Brained GUI Agents: A Survey <br> <sup><sub>*Chaoyun Zhang, Shilin He, Jiaxu Qian, Bowen Li, Liqun Li, Si Qin, Yu Kang, Minghua Ma, et al.*</sub></sup> | [Paper](https://arxiv.org/abs/2411.18279)\|[Res.](https://github.com/vyokky/LLM-Brained-GUI-Agents-Survey) |
| 2024 | arXiv | GUI Agents with Foundation Models: A Comprehensive Survey <br> <sup><sub>*Shuai Wang, Weiwen Liu, Jingxuan Chen, Yuqi Zhou, Weinan Gan, Xingshan Zeng, Yuhan Che, Shuai Yu, et al.*</sub></sup> | [Paper](https://arxiv.org/abs/2411.04890) |
| 2024 | arXiv | Foundations and Recent Trends in Multimodal Mobile Agents: A Survey <br> <sup><sub>*Biao Wu, Yanda Li, Zhiwei Zhang, Yunchao Wei, Meng Fang, Ling Chen*</sub></sup> | [Paper](https://arxiv.org/abs/2411.02006) |
| 2024 | arXiv | Personal LLM Agents: Insights and Survey about the Capability, Efficiency and Security <br> <sup><sub>*Yuanchun Li, Hao Wen, Weijun Wang, Xiangyu Li, Yizhen Yuan, Guohong Liu, Jiacheng Liu, Wenxing Xu, et al.*</sub></sup> | [Paper](https://arxiv.org/abs/2401.05459)\|[Res.](https://github.com/MobileLLM/Personal_LLM_Agents_Survey) |


</details>


--------------------------------------------------------------------------------------

<details>
<summary><h2 id="native-models">🤖 Native GUI Agent Models</h2></summary>

> End-to-end (M)LLMs trained to perceive screenshots and output GUI actions directly.

<details open>
<summary><h3>2025</h3></summary>

| **Pub.** | **Model** | **Title**          | **Links**        |
| :------: | :------: | :----------------------------------------------------------- |  :----------------------------------------------------------- |
| NeurIPS<br><sup>2025</sup> | <sup>`OpenCUA`</sup> | OpenCUA: Open Foundations for Computer-Use Agents `Desktop` <sub>![AgentNet](https://img.shields.io/badge/AgentNet-grey)</sub> <br> <sup><sub>*Xinyuan Wang, Bowen Wang, Dunjie Lu, Junlin Yang, Tianbao Xie, Junli Wang, Jiaqi Deng, Xiaole Guo, et al.*</sub></sup> | [Paper](https://arxiv.org/abs/2508.09123)\|[Code](https://github.com/xlang-ai/OpenCUA) |
| ICML<br><sup>2025</sup> | <sup>`Aguvis`</sup> | Aguvis: Unified Pure Vision Agents for Autonomous GUI Interaction `Cross-platform` <br> <sup><sub>*Yiheng Xu, Zekun Wang, Junli Wang, Dunjie Lu, Tianbao Xie, Amrita Saha, Doyen Sahoo, Tao Yu, et al.*</sub></sup> | [Paper](https://arxiv.org/abs/2412.04454)\|[Code](https://github.com/xlang-ai/aguvis) |
| ICLR<br><sup>2025</sup> | <sup>`LiMAC`</sup> | Lightweight Neural App Control `Mobile` <br> <sup><sub>*Filippos Christianos, Georgios Papoudakis, Thomas Coste, Jianye Hao, Jun Wang, Kun Shao*</sub></sup> | [Paper](https://arxiv.org/abs/2410.17883)\|Code |
| CVPR<br><sup>2025</sup> | <sup>`SpiritSight`</sup> | SpiritSight Agent: Advanced GUI Agent with One Look `Cross-platform` <br> <sup><sub>*Zhiyuan Huang, Ziming Cheng, Junting Pan, Zhaohui Hou, Mingjie Zhan*</sub></sup> | [Paper](https://arxiv.org/abs/2503.03196)\|Code |
| CVPR<br><sup>2025</sup> | <sup>`Magma`</sup> | Magma: A Foundation Model for Multimodal AI Agents `UI+Robotics` <br> <sup><sub>*Jianwei Yang, Reuben Tan, Qianhui Wu, Ruijie Zheng, Baolin Peng, Yongyuan Liang, Yu Gu, Mu Cai, et al.*</sub></sup> | [Paper](https://arxiv.org/abs/2502.13130)\|[Code](https://github.com/microsoft/Magma) |
| CVPR<br><sup>2025</sup> | <sup>`ShowUI`</sup> | ShowUI: One Vision-Language-Action Model for GUI Visual Agent `Cross-platform` <br> <sup><sub>*Kevin Qinghong Lin, Linjie Li, Difei Gao, Zhengyuan Yang, Shiwei Wu, Zechen Bai, Weixian Lei, Lijuan Wang, et al.*</sub></sup> | [Paper](https://arxiv.org/abs/2411.17465)\|[Code](https://github.com/showlab/ShowUI) |
| arXiv<br><sup>2025</sup> | <sup>`ScaleCUA`</sup> | ScaleCUA: Scaling Open-Source Computer Use Agents with Cross-Platform Data `Cross-platform` <br> <sup><sub>*Zhaoyang Liu, Jingjing Xie, Zichen Ding, Zehao Li, Bowen Yang, Zhenyu Wu, Xuehui Wang, Qiushi Sun, et al.*</sub></sup> | [Paper](https://arxiv.org/abs/2509.15221)\|[Code](https://github.com/OpenGVLab/ScaleCUA) |
| arXiv<br><sup>2025</sup> | <sup>`UI-TARS-2`</sup> | UI-TARS-2 Technical Report: Advancing GUI Agent with Multi-Turn Reinforcement Learning `Cross-platform` <br> <sup><sub>*Haoming Wang, Haoyang Zou, Huatong Song, Jiazhan Feng, Junjie Fang, Junting Lu, Longxiang Liu, Qinyu Luo, et al.*</sub></sup> | [Paper](https://arxiv.org/abs/2509.02544)\|[Code](https://github.com/bytedance/UI-TARS) |
| arXiv<br><sup>2025</sup> | <sup>`GUI-Owl`</sup> | Mobile-Agent-v3: Fundamental Agents for GUI Automation `Cross-platform` <br> <sup><sub>*Jiabo Ye, Xi Zhang, Haiyang Xu, Haowei Liu, Junyang Wang, Zhaoqing Zhu, Ziwei Zheng, Feiyu Gao, et al.*</sub></sup> | [Paper](https://arxiv.org/abs/2508.15144)\|[Code](https://github.com/X-PLUG/MobileAgent) |
| arXiv<br><sup>2025</sup> | <sup>`UI-Venus`</sup> | UI-Venus Technical Report: Building High-performance UI Agents with RFT `Mobile` <br> <sup><sub>*Zhangxuan Gu, Zhengwen Zeng, Zhenyu Xu, Xingran Zhou, Shuheng Shen, Yunfei Liu, Beitong Zhou, Changhua Meng, et al.*</sub></sup> | [Paper](https://arxiv.org/abs/2508.10833)\|[Code](https://github.com/inclusionAI/UI-Venus) |
| arXiv<br><sup>2025</sup> | <sup>`Holo1`</sup> | Surfer-H Meets Holo1: Cost-Efficient Web Agent Powered by Open Weights `Web` <br> <sup><sub>*Mathieu Andreux, Breno Baldas Skuk, Hamza Benchekroun, Emilien Biré, Antoine Bonnet, Riaz Bordie, Nathan Bout, Matthias Brunel, et al.*</sub></sup> | [Paper](https://arxiv.org/abs/2506.02865)\|Code |
| arXiv<br><sup>2025</sup> | <sup>`UI-TARS`</sup> | UI-TARS: Pioneering Automated GUI Interaction with Native Agents `Cross-platform` <br> <sup><sub>*Yujia Qin, Yining Ye, Junjie Fang, Haoming Wang, Shihao Liang, Shizuo Tian, Junda Zhang, Jiahao Li, et al.*</sub></sup> | [Paper](https://arxiv.org/abs/2501.12326)\|[Code](https://github.com/bytedance/UI-TARS) |
| arXiv<br><sup>2025</sup> | <sup>`InfiGUIAgent`</sup> | InfiGUIAgent: A Multimodal Generalist GUI Agent with Native Reasoning and Reflection `Cross-platform` <br> <sup><sub>*Yuhang Liu, Pengxiang Li, Zishu Wei, Congkai Xie, Xueyu Hu, Xinchen Xu, Shengyu Zhang, Xiaotian Han, et al.*</sub></sup> | [Paper](https://arxiv.org/abs/2501.04575)\|[Code](https://github.com/Reallm-Labs/InfiGUIAgent) |

</details>

<details>
<summary><h3>2024</h3></summary>

| **Pub.** | **Model** | **Title**          | **Links**        |
| :------: | :------: | :----------------------------------------------------------- |  :----------------------------------------------------------- |
| ICLR<br><sup>2024</sup> | <sup>`WebAgent`</sup> | A Real-World WebAgent with Planning, Long Context Understanding, and Program Synthesis `Web` <br> <sup><sub>*Izzeddin Gur, Hiroki Furuta, Austin Huang, Mustafa Safdari, Yutaka Matsuo, Douglas Eck, Aleksandra Faust*</sub></sup> | [Paper](https://arxiv.org/abs/2307.12856)\|Code |
| ICLR<br><sup>2024</sup> | <sup>`WebGUM`</sup> | Multimodal Web Navigation with Instruction-Finetuned Foundation Models `Web` <br> <sup><sub>*Hiroki Furuta, Kuang-Huei Lee, Ofir Nachum, Yutaka Matsuo, Aleksandra Faust, Shixiang Shane Gu, Izzeddin Gur*</sub></sup> | [Paper](https://arxiv.org/abs/2305.11854)\|Code |
| CVPR<br><sup>2024</sup> | <sup>`CogAgent`</sup> | CogAgent: A Visual Language Model for GUI Agents `Cross-platform` <br> <sup><sub>*Wenyi Hong, Weihan Wang, Qingsong Lv, Jiazheng Xu, Wenmeng Yu, Junhui Ji, Yan Wang, Zihan Wang, et al.*</sub></sup> | [Paper](https://arxiv.org/abs/2312.08914)\|[Code](https://github.com/THUDM/CogAgent) |
| ACL<br><sup>2024</sup> | <sup>`CoCo-Agent`</sup> | CoCo-Agent: A Comprehensive Cognitive MLLM Agent for Smartphone GUI Automation `Mobile` <br> <sup><sub>*Xinbei Ma, Zhuosheng Zhang, Hai Zhao*</sub></sup> | [Paper](https://arxiv.org/abs/2402.11941)\|[Code](https://github.com/xbmxb/CoCo-Agent) |
| ACL Findings<br><sup>2024</sup> | <sup>`Auto-GUI`</sup> | You Only Look at Screens: Multimodal Chain-of-Action Agents `Mobile` <br> <sup><sub>*Zhuosheng Zhang, Aston Zhang*</sub></sup> | [Paper](https://arxiv.org/abs/2309.11436)\|[Code](https://github.com/cooelf/Auto-GUI) |
| KDD<br><sup>2024</sup> | <sup>`AutoWebGLM`</sup> | AutoWebGLM: A Large Language Model-based Web Navigating Agent `Web` <br> <sup><sub>*Hanyu Lai, Xiao Liu, Iat Long Iong, Shuntian Yao, Yuxuan Chen, Pengbo Shen, Hao Yu, Hanchen Zhang, et al.*</sub></sup> | [Paper](https://arxiv.org/abs/2404.03648)\|[Code](https://github.com/THUDM/AutoWebGLM) |
| arXiv<br><sup>2024</sup> | <sup>`Falcon-UI`</sup> | Falcon-UI: Understanding GUI Before Following User Instructions `Cross-platform` <br> <sup><sub>*Huawen Shen, Chang Liu, Gengluo Li, Xinlong Wang, Yu Zhou, Can Ma, Xiangyang Ji*</sub></sup> | [Paper](https://arxiv.org/abs/2412.09362)\|Code |
| arXiv<br><sup>2024</sup> | <sup>`AutoGLM`</sup> | AutoGLM: Autonomous Foundation Agents for GUIs `Web/Mobile` <br> <sup><sub>*Xiao Liu, Bo Qin, Dongzhu Liang, Guang Dong, Hanyu Lai, Hanchen Zhang, Hanlin Zhao, Iat Long Iong, et al.*</sub></sup> | [Paper](https://arxiv.org/abs/2411.00820)\|Code |

</details>

</details>


--------------------------------------------------------------------------------------

<details>
<summary><h2 id="gui-grounding">🎯 GUI Grounding & Screen Understanding</h2></summary>

> Locating UI elements from natural-language instructions, screen parsing and UI understanding.

<details open>
<summary><h3>2026</h3></summary>

| **Pub.** | **Model** | **Title**          | **Links**        |
| :------: | :------: | :----------------------------------------------------------- |  :----------------------------------------------------------- |
| ICLR<br><sup>2026</sup> | <sup>`GTA1`</sup> | GTA1: GUI Test-time Scaling Agent `Cross-platform` <br> <sup><sub>*Yan Yang, Dongxu Li, Yutong Dai, Yuhao Yang, Ziyang Luo, Zirui Zhao, Zhiyuan Hu, Junzhe Huang, et al.*</sub></sup> | [Paper](https://arxiv.org/abs/2507.05791)\|[Code](https://github.com/Yan98/GTA1) |

</details>

<details>
<summary><h3>2025</h3></summary>

| **Pub.** | **Model** | **Title**          | **Links**        |
| :------: | :------: | :----------------------------------------------------------- |  :----------------------------------------------------------- |
| NeurIPS<br><sup>2025</sup> | <sup>`GUI-Actor`</sup> | GUI-Actor: Coordinate-Free Visual Grounding for GUI Agents `Cross-platform` <br> <sup><sub>*Qianhui Wu, Kanzhi Cheng, Rui Yang, Chaoyun Zhang, Jianwei Yang, Huiqiang Jiang, Jian Mu, Baolin Peng, et al.*</sub></sup> | [Paper](https://arxiv.org/abs/2506.03143)\|[Code](https://github.com/microsoft/GUI-Actor) |
| NeurIPS<br><sup>2025</sup> | <sup>`Jedi`</sup> | Scaling Computer-Use Grounding via User Interface Decomposition and Synthesis `Desktop` <sub>![OSWorld-G](https://img.shields.io/badge/OSWorld--G-grey)</sub> <br> <sup><sub>*Tianbao Xie, Jiaqi Deng, Xiaochuan Li, Junlin Yang, Haoyuan Wu, Jixuan Chen, Wenjing Hu, Xinyuan Wang, et al.*</sub></sup> | [Paper](https://arxiv.org/abs/2505.13227)\|[Code](https://github.com/xlang-ai/OSWorld-G) |
| ICLR<br><sup>2025</sup> | <sup>`OS-Atlas`</sup> | OS-ATLAS: A Foundation Action Model for Generalist GUI Agents `Cross-platform` <sub>![ScreenSpot-v2](https://img.shields.io/badge/ScreenSpot--v2-grey)</sub> <br> <sup><sub>*Zhiyong Wu, Zhenyu Wu, Fangzhi Xu, Yian Wang, Qiushi Sun, Chengyou Jia, Kanzhi Cheng, Zichen Ding, et al.*</sub></sup> | [Paper](https://arxiv.org/abs/2410.23218)\|[Code](https://github.com/OS-Copilot/OS-Atlas) |
| ICLR<br><sup>2025</sup> | <sup>`Ferret-UI 2`</sup> | Ferret-UI 2: Mastering Universal User Interface Understanding Across Platforms `Cross-platform` <br> <sup><sub>*Zhangheng Li, Keen You, Haotian Zhang, Di Feng, Harsh Agrawal, Xiujun Li, Mohana Prasad Sathya Moorthy, Jeff Nichols, et al.*</sub></sup> | [Paper](https://arxiv.org/abs/2410.18967)\|Code |
| ICLR<br><sup>2025</sup> | <sup>`UGround`</sup> | Navigating the Digital World as Humans Do: Universal Visual Grounding for GUI Agents `Cross-platform` <br> <sup><sub>*Boyu Gou, Ruohan Wang, Boyuan Zheng, Yanan Xie, Cheng Chang, Yiheng Shu, Huan Sun, Yu Su*</sub></sup> | [Paper](https://arxiv.org/abs/2410.05243)\|[Code](https://github.com/OSU-NLP-Group/UGround) |
| ICCV<br><sup>2025</sup> | <sup>`RegionFocus`</sup> | Visual Test-time Scaling for GUI Agent Grounding `Cross-platform` <br> <sup><sub>*Tiange Luo, Lajanugen Logeswaran, Justin Johnson, Honglak Lee*</sub></sup> | [Paper](https://arxiv.org/abs/2505.00684)\|Code |
| ACL Findings<br><sup>2025</sup> | <sup>`Aria-UI`</sup> | Aria-UI: Visual Grounding for GUI Instructions `Cross-platform` <br> <sup><sub>*Yuhao Yang, Yue Wang, Dongxu Li, Ziyang Luo, Bei Chen, Chao Huang, Junnan Li*</sub></sup> | [Paper](https://arxiv.org/abs/2412.16256)\|[Code](https://github.com/AriaUI/Aria-UI) |
| arXiv<br><sup>2025</sup> | <sup>`Phi-Ground`</sup> | Phi-Ground Tech Report: Advancing Perception in GUI Grounding `Cross-platform` <br> <sup><sub>*Miaosen Zhang, Ziqiang Xu, Jialiang Zhu, Qi Dai, Kai Qiu, Yifan Yang, Chong Luo, Tianyi Chen, et al.*</sub></sup> | [Paper](https://arxiv.org/abs/2507.23779)\|[Code](https://github.com/zhangmiaosen2000/Phi-Ground) |

</details>

<details>
<summary><h3>2024</h3></summary>

| **Pub.** | **Model** | **Title**          | **Links**        |
| :------: | :------: | :----------------------------------------------------------- |  :----------------------------------------------------------- |
| ECCV<br><sup>2024</sup> | <sup>`Ferret-UI`</sup> | Ferret-UI: Grounded Mobile UI Understanding with Multimodal LLMs `Mobile` <br> <sup><sub>*Keen You, Haotian Zhang, Eldon Schoop, Floris Weers, Amanda Swearngin, Jeffrey Nichols, Yinfei Yang, Zhe Gan*</sub></sup> | [Paper](https://arxiv.org/abs/2404.05719)\|[Code](https://github.com/apple/ml-ferret) |
| ACL<br><sup>2024</sup> | <sup>`SeeClick`</sup> | SeeClick: Harnessing GUI Grounding for Advanced Visual GUI Agents `Cross-platform` <sub>![ScreenSpot](https://img.shields.io/badge/ScreenSpot-grey)</sub> <br> <sup><sub>*Kanzhi Cheng, Qiushi Sun, Yougang Chu, Fangzhi Xu, Yantao Li, Jianbing Zhang, Zhiyong Wu*</sub></sup> | [Paper](https://arxiv.org/abs/2401.10935)\|[Code](https://github.com/njucckevin/SeeClick) |
| IJCAI<br><sup>2024</sup> | <sup>`ScreenAI`</sup> | ScreenAI: A Vision-Language Model for UI and Infographics Understanding <br> <sup><sub>*Gilles Baechler, Srinivas Sunkara, Maria Wang, Fedir Zubach, Hassan Mansoor, Vincent Etter, Victor Cărbune, Jason Lin, et al.*</sub></sup> | [Paper](https://arxiv.org/abs/2402.04615)\|Code |
| arXiv<br><sup>2024</sup> | <sup>`Ponder & Press`</sup> | Ponder & Press: Advancing Visual GUI Agent towards General Computer Control `Cross-platform` <br> <sup><sub>*Yiqin Wang, Haoji Zhang, Jingqi Tian, Yansong Tang*</sub></sup> | [Paper](https://arxiv.org/abs/2412.01268)\|Code |
| arXiv<br><sup>2024</sup> | <sup>`OmniParser`</sup> | OmniParser for Pure Vision Based GUI Agent `Cross-platform` <br> <sup><sub>*Yadong Lu, Jianwei Yang, Yelong Shen, Ahmed Awadallah*</sub></sup> | [Paper](https://arxiv.org/abs/2408.00203)\|[Code](https://github.com/microsoft/OmniParser) |

</details>

<details>
<summary><h3>2023 & Earlier</h3></summary>

| **Pub.** | **Model** | **Title**          | **Links**        |
| :------: | :------: | :----------------------------------------------------------- |  :----------------------------------------------------------- |
| ICML<br><sup>2023</sup> | <sup>`Pix2Struct`</sup> | Pix2Struct: Screenshot Parsing as Pretraining for Visual Language Understanding <br> <sup><sub>*Kenton Lee, Mandar Joshi, Iulia Turc, Hexiang Hu, Fangyu Liu, Julian Eisenschlos, Urvashi Khandelwal, Peter Shaw, et al.*</sub></sup> | [Paper](https://arxiv.org/abs/2210.03347)\|[Code](https://github.com/google-research/pix2struct) |
| ICLR<br><sup>2023</sup> | <sup>`Spotlight`</sup> | Spotlight: Mobile UI Understanding using Vision-Language Models with a Focus `Mobile` <br> <sup><sub>*Gang Li, Yang Li*</sub></sup> | [Paper](https://arxiv.org/abs/2209.14927)\|Code |
| arXiv<br><sup>2023</sup> | <sup>`SoM`</sup> | Set-of-Mark Prompting Unleashes Extraordinary Visual Grounding in GPT-4V <br> <sup><sub>*Jianwei Yang, Hao Zhang, Feng Li, Xueyan Zou, Chunyuan Li, Jianfeng Gao*</sub></sup> | [Paper](https://arxiv.org/abs/2310.11441)\|[Code](https://github.com/microsoft/SoM) |

</details>

</details>


--------------------------------------------------------------------------------------

<details>
<summary><h2 id="agent-frameworks">🧩 Agent Frameworks</h2></summary>

> Prompt-based, modular and multi-agent systems built on top of (M)LLMs, including memory and self-improvement.

<details open>
<summary><h3>2026</h3></summary>

| **Pub.** | **Model** | **Title**          | **Links**        |
| :------: | :------: | :----------------------------------------------------------- |  :----------------------------------------------------------- |
| ICLR<br><sup>2026</sup> | <sup>`CoAct-1`</sup> | CoAct-1: Computer-using Multi-Agent System with Coding Actions `Desktop` <br> <sup><sub>*Linxin Song, Yutong Dai, Viraj Prabhu, Jieyu Zhang, Taiwei Shi, Li Li, Junnan Li, Silvio Savarese, et al.*</sub></sup> | [Paper](https://arxiv.org/abs/2508.03923)\|Code |
| MobiCom<br><sup>2026</sup> | <sup>`V-Droid`</sup> | Advancing Mobile GUI Agents: A Verifier-Driven Approach to Practical Deployment `Mobile` <br> <sup><sub>*Gaole Dai, Shiqi Jiang, Ting Cao, Yuanchun Li, Yuqing Yang, Rui Tan, Mo Li, Lili Qiu*</sub></sup> | [Paper](https://arxiv.org/abs/2503.15937)\|Code |
| TMLR<br><sup>2026</sup> | <sup>`Agent S3`</sup> | Scaling Agents for Computer Use `Desktop` <br> <sup><sub>*Gonzalo Gonzalez-Pumariega, Vincent Tu, Chih-Lun Lee, Jiachen Yang, Ang Li, Xin Eric Wang*</sub></sup> | [Paper](https://arxiv.org/abs/2510.02250)\|[Code](https://github.com/simular-ai/Agent-S) |

</details>

<details>
<summary><h3>2025</h3></summary>

| **Pub.** | **Model** | **Title**          | **Links**        |
| :------: | :------: | :----------------------------------------------------------- |  :----------------------------------------------------------- |
| ICML<br><sup>2025</sup> | <sup>`AWM`</sup> | Agent Workflow Memory `Web` <br> <sup><sub>*Zora Zhiruo Wang, Jiayuan Mao, Daniel Fried, Graham Neubig*</sub></sup> | [Paper](https://arxiv.org/abs/2409.07429)\|[Code](https://github.com/zorazrw/agent-workflow-memory) |
| ICML<br><sup>2025</sup> | <sup>`Cradle`</sup> | Cradle: Empowering Foundation Agents Towards General Computer Control `Desktop/Game` <br> <sup><sub>*Weihao Tan, Wentao Zhang, Xinrun Xu, Haochong Xia, Ziluo Ding, Boyu Li, Bohan Zhou, Junpeng Yue, et al.*</sub></sup> | [Paper](https://arxiv.org/abs/2403.03186)\|[Code](https://github.com/BAAI-Agents/Cradle) |
| ICLR<br><sup>2025</sup> | <sup>`AgentOccam`</sup> | AgentOccam: A Simple Yet Strong Baseline for LLM-Based Web Agents `Web` <br> <sup><sub>*Ke Yang, Yao Liu, Sapana Chaudhary, Rasool Fakoor, Pratik Chaudhari, George Karypis, Huzefa Rangwala*</sub></sup> | [Paper](https://arxiv.org/abs/2410.13825)\|[Code](https://github.com/amazon-science/AgentOccam) |
| ICLR<br><sup>2025</sup> | <sup>`Agent S`</sup> | Agent S: An Open Agentic Framework that Uses Computers Like a Human `Desktop` <br> <sup><sub>*Saaket Agashe, Jiuzhou Han, Shuyu Gan, Jiachen Yang, Ang Li, Xin Eric Wang*</sub></sup> | [Paper](https://arxiv.org/abs/2410.08164)\|[Code](https://github.com/simular-ai/Agent-S) |
| NAACL<br><sup>2025</sup> | <sup>`MobA`</sup> | MobA: Multifaceted Memory-Enhanced Adaptive Planning for Efficient Mobile Task Automation `Mobile` <br> <sup><sub>*Zichen Zhu, Hao Tang, Yansi Li, Dingye Liu, Hongshen Xu, Kunyao Lan, Danyang Zhang, Yixuan Jiang, et al.*</sub></sup> | [Paper](https://arxiv.org/abs/2410.13757)\|Code |
| NAACL<br><sup>2025</sup> | <sup>`UFO`</sup> | UFO: A UI-Focused Agent for Windows OS Interaction `Windows` <br> <sup><sub>*Chaoyun Zhang, Liqun Li, Shilin He, Xu Zhang, Bo Qiao, Si Qin, Minghua Ma, Yu Kang, et al.*</sub></sup> | [Paper](https://arxiv.org/abs/2402.07939)\|[Code](https://github.com/microsoft/UFO) |
| COLM<br><sup>2025</sup> | <sup>`Agent S2`</sup> | Agent S2: A Compositional Generalist-Specialist Framework for Computer Use Agents `Desktop` <br> <sup><sub>*Saaket Agashe, Kyle Wong, Vincent Tu, Jiachen Yang, Ang Li, Xin Eric Wang*</sub></sup> | [Paper](https://arxiv.org/abs/2504.00906)\|[Code](https://github.com/simular-ai/Agent-S) |
| CHI<br><sup>2025</sup> | <sup>`AppAgent`</sup> | AppAgent: Multimodal Agents as Smartphone Users `Mobile` <br> <sup><sub>*Chi Zhang, Zhao Yang, Jiaxuan Liu, Yanda Li, Yucheng Han, Xin Chen, Zebiao Huang, Bin Fu, et al.*</sub></sup> | [Paper](https://arxiv.org/abs/2312.13771)\|[Code](https://github.com/TencentQQGYLab/AppAgent) |
| MobiSys<br><sup>2025</sup> | <sup>`AutoDroid-V2`</sup> | AutoDroid-V2: Boosting SLM-based GUI Agents via Code Generation `Mobile` <br> <sup><sub>*Hao Wen, Shizuo Tian, Borislav Pavlov, Wenjie Du, Yixuan Li, Ge Chang, Shanhui Zhao, Jiacheng Liu, et al.*</sub></sup> | [Paper](https://arxiv.org/abs/2412.18116)\|Code |
| TMLR<br><sup>2025</sup> | <sup>`UFO²`</sup> | UFO2: The Desktop AgentOS `Windows` <br> <sup><sub>*Chaoyun Zhang, He Huang, Chiming Ni, Jian Mu, Si Qin, Shilin He, Lu Wang, Fangkai Yang, et al.*</sub></sup> | [Paper](https://arxiv.org/abs/2504.14603)\|[Code](https://github.com/microsoft/UFO) |
| arXiv<br><sup>2025</sup> | <sup>`PC-Agent`</sup> | PC-Agent: A Hierarchical Multi-Agent Collaboration Framework for Complex Task Automation on PC `Windows` <br> <sup><sub>*Haowei Liu, Xi Zhang, Haiyang Xu, Yuyang Wanyan, Junyang Wang, Ming Yan, Ji Zhang, Chunfeng Yuan, et al.*</sub></sup> | [Paper](https://arxiv.org/abs/2502.14282)\|[Code](https://github.com/X-PLUG/MobileAgent) |
| arXiv<br><sup>2025</sup> | <sup>`Mobile-Agent-E`</sup> | Mobile-Agent-E: Self-Evolving Mobile Assistant for Complex Tasks `Mobile` <br> <sup><sub>*Zhenhailong Wang, Haiyang Xu, Junyang Wang, Xi Zhang, Ming Yan, Ji Zhang, Fei Huang, Heng Ji*</sub></sup> | [Paper](https://arxiv.org/abs/2501.11733)\|[Code](https://github.com/X-PLUG/MobileAgent) |

</details>

<details>
<summary><h3>2024</h3></summary>

| **Pub.** | **Model** | **Title**          | **Links**        |
| :------: | :------: | :----------------------------------------------------------- |  :----------------------------------------------------------- |
| NeurIPS<br><sup>2024</sup> | <sup>`Mobile-Agent-v2`</sup> | Mobile-Agent-v2: Mobile Device Operation Assistant with Effective Navigation via Multi-Agent Collaboration `Mobile` <br> <sup><sub>*Junyang Wang, Haiyang Xu, Haitao Jia, Xi Zhang, Ming Yan, Weizhou Shen, Ji Zhang, Fei Huang, et al.*</sub></sup> | [Paper](https://arxiv.org/abs/2406.01014)\|[Code](https://github.com/X-PLUG/MobileAgent) |
| ICML<br><sup>2024</sup> | <sup>`SeeAct`</sup> | GPT-4V(ision) is a Generalist Web Agent, if Grounded `Web` <br> <sup><sub>*Boyuan Zheng, Boyu Gou, Jihyung Kil, Huan Sun, Yu Su*</sub></sup> | [Paper](https://arxiv.org/abs/2401.01614)\|[Code](https://github.com/OSU-NLP-Group/SeeAct) |
| ICLR<br><sup>2024</sup> | <sup>`Synapse`</sup> | Synapse: Trajectory-as-Exemplar Prompting with Memory for Computer Control `Web` <br> <sup><sub>*Longtao Zheng, Rundong Wang, Xinrun Wang, Bo An*</sub></sup> | [Paper](https://arxiv.org/abs/2306.07863)\|[Code](https://github.com/ltzheng/Synapse) |
| MobiCom<br><sup>2024</sup> | <sup>`AutoDroid`</sup> | AutoDroid: LLM-powered Task Automation in Android `Mobile` <br> <sup><sub>*Hao Wen, Yuanchun Li, Guohong Liu, Shanhui Zhao, Tao Yu, Toby Jia-Jun Li, Shiqi Jiang, Yunhao Liu, et al.*</sub></sup> | [Paper](https://arxiv.org/abs/2308.15272)\|[Code](https://github.com/MobileLLM/AutoDroid) |
| arXiv<br><sup>2024</sup> | <sup>`--`</sup> | The Dawn of GUI Agent: A Preliminary Case Study with Claude 3.5 Computer Use `Desktop` <br> <sup><sub>*Siyuan Hu, Mingyu Ouyang, Difei Gao, Mike Zheng Shou*</sub></sup> | [Paper](https://arxiv.org/abs/2411.10323)\|[Code](https://github.com/showlab/computer_use_ootb) |
| arXiv<br><sup>2024</sup> | <sup>`AppAgent v2`</sup> | AppAgent v2: Advanced Agent for Flexible Mobile Interactions `Mobile` <br> <sup><sub>*Yanda Li, Chi Zhang, Wenjia Jiang, Wanqi Yang, Bin Fu, Pei Cheng, Xin Chen, Ling Chen, et al.*</sub></sup> | [Paper](https://arxiv.org/abs/2408.11824)\|Code |
| arXiv<br><sup>2024</sup> | <sup>`Agent-E`</sup> | Agent-E: From Autonomous Web Navigation to Foundational Design Principles in Agentic Systems `Web` <br> <sup><sub>*Tamer Abuelsaad, Deepak Akkil, Prasenjit Dey, Ashish Jagmohan, Aditya Vempaty, Ravi Kokku*</sub></sup> | [Paper](https://arxiv.org/abs/2407.13032)\|[Code](https://github.com/EmergenceAI/Agent-E) |
| arXiv<br><sup>2024</sup> | <sup>`OS-Copilot`</sup> | OS-Copilot: Towards Generalist Computer Agents with Self-Improvement `Desktop` <br> <sup><sub>*Zhiyong Wu, Chengcheng Han, Zichen Ding, Zhenmin Weng, Zhoumianze Liu, Shunyu Yao, Tao Yu, Lingpeng Kong*</sub></sup> | [Paper](https://arxiv.org/abs/2402.07456)\|[Code](https://github.com/OS-Copilot/OS-Copilot) |
| arXiv<br><sup>2024</sup> | <sup>`Mobile-Agent`</sup> | Mobile-Agent: Autonomous Multi-Modal Mobile Device Agent with Visual Perception `Mobile` <br> <sup><sub>*Junyang Wang, Haiyang Xu, Jiabo Ye, Ming Yan, Weizhou Shen, Ji Zhang, Fei Huang, Jitao Sang*</sub></sup> | [Paper](https://arxiv.org/abs/2401.16158)\|[Code](https://github.com/X-PLUG/MobileAgent) |

</details>

<details>
<summary><h3>2023 & Earlier</h3></summary>

| **Pub.** | **Model** | **Title**          | **Links**        |
| :------: | :------: | :----------------------------------------------------------- |  :----------------------------------------------------------- |
| arXiv<br><sup>2023</sup> | <sup>`MM-Navigator`</sup> | GPT-4V in Wonderland: Large Multimodal Models for Zero-Shot Smartphone GUI Navigation `Mobile` <br> <sup><sub>*An Yan, Zhengyuan Yang, Wanrong Zhu, Kevin Lin, Linjie Li, Jianfeng Wang, Jianwei Yang, Yiwu Zhong, et al.*</sub></sup> | [Paper](https://arxiv.org/abs/2311.07562)\|[Code](https://github.com/zzxslp/MM-Navigator) |

</details>

</details>


--------------------------------------------------------------------------------------

<details>
<summary><h2 id="world-models">🌍 World Models & Planning</h2></summary>

> Model-based planning, environment dynamics modelling and search for GUI agents.

| **Pub.** | **Model** | **Title**          | **Links**        |
| :------: | :------: | :----------------------------------------------------------- |  :----------------------------------------------------------- |
| ICLR<br><sup>2025</sup> | <sup>`WMA`</sup> | Web Agents with World Models: Learning and Leveraging Environment Dynamics in Web Navigation `Web` <br> <sup><sub>*Hyungjoo Chae, Namyoung Kim, Kai Tzu-iunn Ong, Minju Gwak, Gwanwoo Song, Jihoon Kim, Sunghwan Kim, Dongha Lee, et al.*</sub></sup> | [Paper](https://arxiv.org/abs/2410.13232)\|[Code](https://github.com/kyle8581/WMA-Agents) |
| TMLR<br><sup>2025</sup> | <sup>`WebDreamer`</sup> | Is Your LLM Secretly a World Model of the Internet? Model-Based Planning for Web Agents `Web` <br> <sup><sub>*Yu Gu, Kai Zhang, Yuting Ning, Boyuan Zheng, Boyu Gou, Tianci Xue, Cheng Chang, Sanjari Srivastava, et al.*</sub></sup> | [Paper](https://arxiv.org/abs/2411.06559)\|[Code](https://github.com/OSU-NLP-Group/WebDreamer) |
| TMLR<br><sup>2025</sup> | <sup>`Tree Search`</sup> | Tree Search for Language Model Agents `Web` <br> <sup><sub>*Jing Yu Koh, Stephen McAleer, Daniel Fried, Ruslan Salakhutdinov*</sub></sup> | [Paper](https://arxiv.org/abs/2407.01476)\|[Code](https://github.com/kohjingyu/search-agents) |

</details>


--------------------------------------------------------------------------------------

<details>
<summary><h2 id="reinforcement-learning">🏋️ Reinforcement Learning & Self-Evolution</h2></summary>

> Offline / online RL, R1-style reinforcement fine-tuning, reward modelling and self-improvement.

<details open>
<summary><h3>2026</h3></summary>

| **Pub.** | **Model** | **Title**          | **Links**        |
| :------: | :------: | :----------------------------------------------------------- |  :----------------------------------------------------------- |
| CVPR<br><sup>2026</sup> | <sup>`UI-AGILE`</sup> | UI-AGILE: Advancing GUI Agents with Effective Reinforcement Learning and Precise Inference-Time Grounding `Cross-platform` <br> <sup><sub>*Shuquan Lian, Yuhang Wu, Jia Ma, Yifan Ding, Zihan Song, Bingqi Chen, Xiawu Zheng, Hui Li, et al.*</sub></sup> | [Paper](https://arxiv.org/abs/2507.22025)\|[Code](https://github.com/KDEGroup/UI-AGILE) |
| AAAI<br><sup>2026</sup> | <sup>`GUI-G²`</sup> | GUI-G$^2$: Gaussian Reward Modeling for GUI Grounding `Grounding` <br> <sup><sub>*Fei Tang, Zhangxuan Gu, Zhengxi Lu, Xuyang Liu, Shuheng Shen, Changhua Meng, Wen Wang, Wenqi Zhang, et al.*</sub></sup> | [Paper](https://arxiv.org/abs/2507.15846)\|[Code](https://github.com/zju-real/GUI-G2) |
| AAAI<br><sup>2026</sup> | <sup>`UI-R1`</sup> | UI-R1: Enhancing Efficient Action Prediction of GUI Agents by Reinforcement Learning `Mobile` <br> <sup><sub>*Zhengxi Lu, Yuxiang Chai, Yaxuan Guo, Xi Yin, Liang Liu, Hao Wang, Han Xiao, Shuai Ren, et al.*</sub></sup> | [Paper](https://arxiv.org/abs/2503.21620)\|[Code](https://github.com/lll6gg/UI-R1) |

</details>

<details>
<summary><h3>2025</h3></summary>

| **Pub.** | **Model** | **Title**          | **Links**        |
| :------: | :------: | :----------------------------------------------------------- |  :----------------------------------------------------------- |
| NeurIPS<br><sup>2025</sup> | <sup>`UI-Genie`</sup> | UI-Genie: A Self-Improving Approach for Iteratively Boosting MLLM-based Mobile GUI Agents `Mobile` <br> <sup><sub>*Han Xiao, Guozhi Wang, Yuxiang Chai, Zimu Lu, Weifeng Lin, Hao He, Lue Fan, Liuyang Bian, et al.*</sub></sup> | [Paper](https://arxiv.org/abs/2505.21496)\|[Code](https://github.com/Euphoria16/UI-Genie) |
| NeurIPS<br><sup>2025</sup> | <sup>`GUI-G1`</sup> | GUI-G1: Understanding R1-Zero-Like Training for Visual Grounding in GUI Agents `Grounding` <br> <sup><sub>*Yuqi Zhou, Sunhao Dai, Shuai Wang, Kaiwen Zhou, Qinglin Jia, Jun Xu*</sub></sup> | [Paper](https://arxiv.org/abs/2505.15810)\|[Code](https://github.com/Yuqi-Zhou/GUI-G1) |
| NeurIPS<br><sup>2025</sup> | <sup>`SE-GUI`</sup> | Enhancing Visual Grounding for GUI Agents via Self-Evolutionary Reinforcement Learning `Grounding` <br> <sup><sub>*Xinbin Yuan, Jian Zhang, Kaixin Li, Zhuoxuan Cai, Lujian Yao, Jie Chen, Enguang Wang, Qibin Hou, et al.*</sub></sup> | [Paper](https://arxiv.org/abs/2505.12370)\|[Code](https://github.com/YXB-NKU/SE-GUI) |
| ICLR<br><sup>2025</sup> | <sup>`WebRL`</sup> | WebRL: Training LLM Web Agents via Self-Evolving Online Curriculum Reinforcement Learning `Web` <br> <sup><sub>*Zehan Qi, Xiao Liu, Iat Long Iong, Hanyu Lai, Xueqiao Sun, Wenyi Zhao, Yu Yang, Xinyue Yang, et al.*</sub></sup> | [Paper](https://arxiv.org/abs/2411.02337)\|[Code](https://github.com/THUDM/WebRL) |
| ICLR<br><sup>2025</sup> | <sup>`DistRL`</sup> | DistRL: An Asynchronous Distributed Reinforcement Learning Framework for On-Device Control Agents `Mobile` <br> <sup><sub>*Taiyi Wang, Zhihao Wu, Jianheng Liu, Jianye Hao, Jun Wang, Kun Shao*</sub></sup> | [Paper](https://arxiv.org/abs/2410.14803)\|Code |
| arXiv<br><sup>2025</sup> | <sup>`MobileGUI-RL`</sup> | MobileGUI-RL: Advancing Mobile GUI Agent through Reinforcement Learning in Online Environment `Mobile` <br> <sup><sub>*Yucheng Shi, Wenhao Yu, Zaitang Li, Yonglin Wang, Hongming Zhang, Ninghao Liu, Haitao Mi, Dong Yu*</sub></sup> | [Paper](https://arxiv.org/abs/2507.05720)\|Code |
| arXiv<br><sup>2025</sup> | <sup>`GUI-Reflection`</sup> | GUI-Reflection: Empowering Multimodal GUI Models with Self-Reflection Behavior `Mobile` <br> <sup><sub>*Penghao Wu, Shengnan Ma, Bo Wang, Jiaheng Yu, Lewei Lu, Ziwei Liu*</sub></sup> | [Paper](https://arxiv.org/abs/2506.08012)\|Code |
| arXiv<br><sup>2025</sup> | <sup>`ZeroGUI`</sup> | ZeroGUI: Automating Online GUI Learning at Zero Human Cost `Desktop/Mobile` <br> <sup><sub>*Chenyu Yang, Shiqian Su, Shi Liu, Xuan Dong, Yue Yu, Weijie Su, Xuehui Wang, Zhaoyang Liu, et al.*</sub></sup> | [Paper](https://arxiv.org/abs/2505.23762)\|[Code](https://github.com/OpenGVLab/ZeroGUI) |
| arXiv<br><sup>2025</sup> | <sup>`ARPO`</sup> | ARPO:End-to-End Policy Optimization for GUI Agents with Experience Replay `Desktop` <br> <sup><sub>*Fanbin Lu, Zhisheng Zhong, Shu Liu, Chi-Wing Fu, Jiaya Jia*</sub></sup> | [Paper](https://arxiv.org/abs/2505.16282)\|[Code](https://github.com/dvlab-research/ARPO) |
| arXiv<br><sup>2025</sup> | <sup>`InfiGUI-R1`</sup> | InfiGUI-R1: Advancing Multimodal GUI Agents from Reactive Actors to Deliberative Reasoners `Cross-platform` <br> <sup><sub>*Yuhang Liu, Pengxiang Li, Congkai Xie, Xavier Hu, Xiaotian Han, Shengyu Zhang, Hongxia Yang, Fei Wu*</sub></sup> | [Paper](https://arxiv.org/abs/2504.14239)\|[Code](https://github.com/Reallm-Labs/InfiGUI-R1) |
| arXiv<br><sup>2025</sup> | <sup>`GUI-R1`</sup> | GUI-R1 : A Generalist R1-Style Vision-Language Action Model For GUI Agents `Cross-platform` <br> <sup><sub>*Run Luo, Lu Wang, Wanwei He, Longze Chen, Jiaming Li, Xiaobo Xia*</sub></sup> | [Paper](https://arxiv.org/abs/2504.10458)\|[Code](https://github.com/ritzz-ai/GUI-R1) |
| arXiv<br><sup>2025</sup> | <sup>`Digi-Q`</sup> | Digi-Q: Learning Q-Value Functions for Training Device-Control Agents `Mobile` <br> <sup><sub>*Hao Bai, Yifei Zhou, Li Erran Li, Sergey Levine, Aviral Kumar*</sub></sup> | [Paper](https://arxiv.org/abs/2502.15760)\|[Code](https://github.com/DigiRL-agent/digiq) |

</details>

<details>
<summary><h3>2024</h3></summary>

| **Pub.** | **Model** | **Title**          | **Links**        |
| :------: | :------: | :----------------------------------------------------------- |  :----------------------------------------------------------- |
| NeurIPS<br><sup>2024</sup> | <sup>`DigiRL`</sup> | DigiRL: Training In-The-Wild Device-Control Agents with Autonomous Reinforcement Learning `Mobile` <br> <sup><sub>*Hao Bai, Yifei Zhou, Mert Cemri, Jiayi Pan, Alane Suhr, Sergey Levine, Aviral Kumar*</sub></sup> | [Paper](https://arxiv.org/abs/2406.11896)\|[Code](https://github.com/DigiRL-agent/digirl) |
| arXiv<br><sup>2024</sup> | <sup>`Agent Q`</sup> | Agent Q: Advanced Reasoning and Learning for Autonomous AI Agents `Web` <br> <sup><sub>*Pranav Putta, Edmund Mills, Naman Garg, Sumeet Motwani, Chelsea Finn, Divyansh Garg, Rafael Rafailov*</sub></sup> | [Paper](https://arxiv.org/abs/2408.07199)\|Code |

</details>

</details>


--------------------------------------------------------------------------------------

<details>
<summary><h2 id="data-synthesis">🧪 Data & Trajectory Synthesis</h2></summary>

> Scaling GUI agent training data: exploration, tutorial replay, reverse task synthesis.

| **Pub.** | **Model** | **Title**          | **Links**        |
| :------: | :------: | :----------------------------------------------------------- |  :----------------------------------------------------------- |
| AAAI<br><sup>2026</sup> | <sup>`TongUI`</sup> | TongUI: Internet-Scale Trajectories from Multimodal Web Tutorials for Generalized GUI Agents `Cross-platform` <br> <sup><sub>*Bofei Zhang, Zirui Shang, Zhi Gao, Wang Zhang, Rui Xie, Xiaojian Ma, Tao Yuan, Xinxiao Wu, et al.*</sub></sup> | [Paper](https://arxiv.org/abs/2504.12679)\|[Code](https://github.com/TongUI-agent/TongUI-agent) |
| ICLR<br><sup>2025</sup> | <sup>`Learn-by-Interact`</sup> | Learn-by-interact: A Data-Centric Framework for Self-Adaptive Agents in Realistic Environments `Cross-platform` <br> <sup><sub>*Hongjin Su, Ruoxi Sun, Jinsung Yoon, Pengcheng Yin, Tao Yu, Sercan Ö. Arık*</sub></sup> | [Paper](https://arxiv.org/abs/2501.10893)\|Code |
| ICLR<br><sup>2025</sup> | <sup>`AgentTrek`</sup> | AgentTrek: Agent Trajectory Synthesis via Guiding Replay with Web Tutorials `Web` <br> <sup><sub>*Yiheng Xu, Dunjie Lu, Zhennan Shen, Junli Wang, Zekun Wang, Yuchen Mao, Caiming Xiong, Tao Yu*</sub></sup> | [Paper](https://arxiv.org/abs/2412.09605)\|[Code](https://github.com/xlang-ai/AgentTrek) |
| ACL<br><sup>2025</sup> | <sup>`OS-Genesis`</sup> | OS-Genesis: Automating GUI Agent Trajectory Construction via Reverse Task Synthesis `Web/Mobile` <br> <sup><sub>*Qiushi Sun, Kanzhi Cheng, Zichen Ding, Chuanyang Jin, Yian Wang, Fangzhi Xu, Zhenyu Wu, Chengyou Jia, et al.*</sub></sup> | [Paper](https://arxiv.org/abs/2412.19723)\|[Code](https://github.com/OS-Copilot/OS-Genesis) |
| ACL<br><sup>2025</sup> | <sup>`GUICourse`</sup> | GUICourse: From General Vision Language Models to Versatile GUI Agents `Cross-platform` <sub>![GUIAct](https://img.shields.io/badge/GUIAct-grey)</sub> <br> <sup><sub>*Wentong Chen, Junbo Cui, Jinyi Hu, Yujia Qin, Junjie Fang, Yue Zhao, Chongyi Wang, Jun Liu, et al.*</sub></sup> | [Paper](https://arxiv.org/abs/2406.11317)\|[Code](https://github.com/yiye3/GUICourse) |
| ACL Findings<br><sup>2025</sup> | <sup>`Explorer`</sup> | Explorer: Scaling Exploration-driven Web Trajectory Synthesis for Multimodal Web Agents `Web` <br> <sup><sub>*Vardaan Pahuja, Yadong Lu, Corby Rosset, Boyu Gou, Arindam Mitra, Spencer Whitehead, Yu Su, Ahmed Awadallah*</sub></sup> | [Paper](https://arxiv.org/abs/2502.11357)\|[Code](https://github.com/OSU-NLP-Group/Explorer) |
| arXiv<br><sup>2025</sup> | <sup>`InSTA`</sup> | InSTA: Towards Internet-Scale Training For Agents `Web` <br> <sup><sub>*Brandon Trabucco, Gunnar Sigurdsson, Robinson Piramuthu, Ruslan Salakhutdinov*</sub></sup> | [Paper](https://arxiv.org/abs/2502.06776)\|Code |
| NeurIPS<br><sup>2024</sup> | <sup>`Synatra`</sup> | Synatra: Turning Indirect Knowledge into Direct Demonstrations for Digital Agents at Scale `Web` <br> <sup><sub>*Tianyue Ou, Frank F. Xu, Aman Madaan, Jiarui Liu, Robert Lo, Abishek Sridhar, Sudipta Sengupta, Dan Roth, et al.*</sub></sup> | [Paper](https://arxiv.org/abs/2409.15637)\|Code |
| arXiv<br><sup>2024</sup> | <sup>`NNetNav`</sup> | NNetNav: Unsupervised Learning of Browser Agents Through Environment Interaction in the Wild `Web` <br> <sup><sub>*Shikhar Murty, Hao Zhu, Dzmitry Bahdanau, Christopher D. Manning*</sub></sup> | [Paper](https://arxiv.org/abs/2410.02907)\|[Code](https://github.com/MurtyShikhar/NNetnav) |

</details>


--------------------------------------------------------------------------------------

<details>
<summary><h2 id="safety">🛡️ Safety & Security</h2></summary>

> Attacks (prompt injection, pop-ups, environmental injection), red-teaming and safety benchmarks.

| **Pub.** | **Model** | **Title**          | **Links**        |
| :------: | :------: | :----------------------------------------------------------- |  :----------------------------------------------------------- |
| arXiv<br><sup>2026</sup> | <sup>`Action Rebinding`</sup> | Mind the Gap: Action Rebinding Attacks against Android GUI Agents `Mobile` <br> <sup><sub>*Yi Qian, Kunwei Qian, Xingbang He, Ligeng Chen, Jikang Zhang, Tiantai Zhang, Haiyang Wei, Linzhang Wang, et al.*</sub></sup> | [Paper](https://arxiv.org/abs/2601.12349)\|Code |
| NeurIPS<br><sup>2025</sup> | <sup>`OS-Harm`</sup> | OS-Harm: A Benchmark for Measuring Safety of Computer Use Agents `Desktop` <sub>![OS-Harm](https://img.shields.io/badge/OS--Harm-grey)</sub> <br> <sup><sub>*Thomas Kuntz, Agatha Duzan, Hao Zhao, Francesco Croce, Zico Kolter, Nicolas Flammarion, Maksym Andriushchenko*</sub></sup> | [Paper](https://arxiv.org/abs/2506.14866)\|[Code](https://github.com/tml-epfl/os-harm) |
| NeurIPS<br><sup>2025</sup> | <sup>`RiOSWorld`</sup> | RiOSWorld: Benchmarking the Risk of Multimodal Computer-Use Agents `Desktop` <sub>![RiOSWorld](https://img.shields.io/badge/RiOSWorld-grey)</sub> <br> <sup><sub>*Jingyi Yang, Shuai Shao, Dongrui Liu, Jing Shao*</sub></sup> | [Paper](https://arxiv.org/abs/2506.00618)\|Code |
| NeurIPS<br><sup>2025</sup> | <sup>`WASP`</sup> | WASP: Benchmarking Web Agent Security Against Prompt Injection Attacks `Web` <br> <sup><sub>*Ivan Evtimov, Arman Zharmagambetov, Aaron Grattafiori, Chuan Guo, Kamalika Chaudhuri*</sub></sup> | [Paper](https://arxiv.org/abs/2504.18575)\|[Code](https://github.com/facebookresearch/wasp) |
| ICML<br><sup>2025</sup> | <sup>`AdvAgent`</sup> | AdvAgent: Controllable Blackbox Red-teaming on Web Agents `Web` <br> <sup><sub>*Chejian Xu, Mintong Kang, Jiawei Zhang, Zeyi Liao, Lingbo Mo, Mengqi Yuan, Huan Sun, Bo Li*</sub></sup> | [Paper](https://arxiv.org/abs/2410.17401)\|Code |
| ICLR<br><sup>2025</sup> | <sup>`EIA`</sup> | EIA: Environmental Injection Attack on Generalist Web Agents for Privacy Leakage `Web` <br> <sup><sub>*Zeyi Liao, Lingbo Mo, Chejian Xu, Mintong Kang, Jiawei Zhang, Chaowei Xiao, Yuan Tian, Bo Li, et al.*</sub></sup> | [Paper](https://arxiv.org/abs/2409.11295)\|Code |
| ACL<br><sup>2025</sup> | <sup>`Pop-up Attack`</sup> | Attacking Vision-Language Computer Agents via Pop-ups `Desktop/Web` <br> <sup><sub>*Yanzhe Zhang, Tao Yu, Diyi Yang*</sub></sup> | [Paper](https://arxiv.org/abs/2411.02391)\|[Code](https://github.com/SALT-NLP/PopupAttack) |
| arXiv<br><sup>2024</sup> | <sup>`MobileSafetyBench`</sup> | MobileSafetyBench: Evaluating Safety of Autonomous Agents in Mobile Device Control `Mobile` <sub>![MobileSafetyBench](https://img.shields.io/badge/MobileSafetyBench-grey)</sub> <br> <sup><sub>*Juyong Lee, Dongyoon Hahm, June Suk Choi, W. Bradley Knox, Kimin Lee*</sub></sup> | [Paper](https://arxiv.org/abs/2410.17520)\|Code |
| arXiv<br><sup>2024</sup> | <sup>`ST-WebAgentBench`</sup> | ST-WebAgentBench: A Benchmark for Evaluating Safety and Trustworthiness in Web Agents `Web` <sub>![ST-WebAgentBench](https://img.shields.io/badge/ST--WebAgentBench-grey)</sub> <br> <sup><sub>*Ido Levy, Ben Wiesel, Sami Marreed, Alon Oved, Avi Yaeli, Nir Mashkif, Segev Shlomov*</sub></sup> | [Paper](https://arxiv.org/abs/2410.06703)\|Code |

</details>


--------------------------------------------------------------------------------------

<h2 id="backdoor">🦠 Backdoor Attacks & Defenses</h2>

> Backdoors in GUI agents, LLM agents and VLMs, organised by **where the backdoor is planted** and **what activates it**. Titles were checked against the arXiv API and venues against proceedings / OpenReview / ACM DL (checked 2026-11-25).
>
> <sup>†</sup> Venue as stated in the arXiv author comment or Semantic Scholar metadata, not yet matched to the proceedings. **Under Review** = OpenReview submission; entries without an arXiv version could not be re-verified.

<details open>
<summary><h3 id="bd-gui">📱 GUI / Mobile / Computer-Use Agent Backdoors</h3></summary>

| **Pub.** | **Title** | **Key Idea** | **Links** |
| :------: | :----------------------------------------------------------- | :----------------------------------------- | :------: |
| Under Review<br><sup>ICLR 2027</sup> | EvolvAttack: Backdooring self Evolving VLM Agents <br> <sup><sub>*Chuan Zou, Yang Xiang, Zexin Li, Xiaonan Luo, Simin Chen*</sub></sup> | Dual-condition backdoor for self-evolving VLM agents: fires only when a visual trigger appears and memory has evolved far enough | [Paper](https://arxiv.org/abs/2610.15244) |
| Under Review<br><sup>ICLR 2027</sup> | Agentic Backdoors via Pretraining Poisoning <br> <sup><sub>*Xinyan Hu, Pingbang Hu, Chloe Loughridge, Xuanli He, Nicholas Carlini, Matthew Jagielski, et al.*</sub></sup> | Pretraining-corpus poisoning that survives clean post-training into CLI agents | [Paper](https://arxiv.org/abs/2610.37741)\|[Code](https://github.com/safety-research/agentic-backdoor) |
| Under Review<br><sup>ICLR 2027</sup> | GistBackdoor: Intent-Triggered Backdoors in GUI Grounding <br> <sup><sub>*Anonymous (under review; not re-verified)*</sub></sup> | Intent-level trigger: whenever the instruction expresses a given intent, clicks are redirected to an attacker-chosen element, regardless of wording and with no extra input cue | [OpenReview](https://openreview.net/forum?id=7XpGtbIqLk) |
| CVPR<br><sup>2026</sup> | IAG: Input-aware Backdoor Attack on VLM-based Visual Grounding <br> <sup><sub>*Junxian Li, Beining Xu, Simin Chen, Jiatong Li, Jingdi Lei, Haodong Zhao, et al.*</sub></sup> | Input-aware, imperceptible triggers generated from the attacker's target description hijack visual grounding (evaluated incl. ShowUI) | [Paper](https://arxiv.org/abs/2508.09456)\|[Code](https://github.com/lijunxian111/IAG) |
| CAIS<br><sup>2026</sup> | Malice in Agentland: Down the Rabbit Hole of Backdoors in the AI Supply Chain <br> <sup><sub>*Léo Boisvert, Abhay Puri, Chandra Kiran Reddy Evuru, Nazanin Sepahvand, Nicolas Chapados, Quentin Cappart, et al.*</sub></sup> | Three supply-chain threats: fine-tuning data poisoning, pre-backdoored base models, and environment poisoning of teacher trajectories | [Paper](https://arxiv.org/abs/2510.05159) |
| CVPR<br><sup>2026</sup> | AdapAction: Adaptive Target Action Backdoor Attack against GUI Agents <br> <sup><sub>*Baicheng Chen, Mingda Zhang, Min Zhang, Haizhou Li, Baoyuan Wu*</sub></sup> | Embeds an adaptive, context-aware malicious policy: the agent picks environment-coherent malicious actions from the current GUI state and instruction, evading LLM-based defenses | [Paper](https://openaccess.thecvf.com/content/CVPR2026/html/Chen_AdapAction_Adaptive_Target_Action_Backdoor_Attack_against_GUI_Agents_CVPR_2026_paper.html) |
| ECCV<sup>†</sup><br><sup>2026</sup> | SlowBA: An efficiency backdoor attack towards VLM-based GUI agents <br> <sup><sub>*Junxian Li, Tu Lan, Haozhen Tan, Yan Meng, Haojin Zhu*</sub></sup> | Efficiency backdoor: realistic pop-up triggers make the agent emit excessively long responses; injected via two-stage reward-level RL | [Paper](https://arxiv.org/abs/2603.08316)\|[Code](https://github.com/tu-tuing/SlowBA) |
| arXiv<br><sup>2026</sup> | AgentRAE: Remote Action Execution through Notification-based Visual Backdoors against Screenshots-based Mobile GUI Agents <br> <sup><sub>*Yutao Luo, Haotian Zhu, Shuchao Pang, Zhigang Lu, Tian Dong, Yongbin Zhou, et al.*</sub></sup> | Benign app icons in notifications act as visual triggers for remote action execution, with multi-target action redirection | [Paper](https://arxiv.org/abs/2603.23007) |
| arXiv<br><sup>2026</sup> | MemVenom: Triggered Poisoning of Multimodal Memories in Web Agents <br> <sup><sub>*Yv Zhang, Hao Sun, Hao Fang, Kuofeng Gao, Fan Mo, Bin Chen, et al.*</sub></sup> | Injects content into a web agent's multimodal external memory; retrieval keeps steering behaviour without touching model weights | [Paper](https://arxiv.org/abs/2606.10742) |
| arXiv<br><sup>2026</sup> | SynChain: Inducing Computer-Use Agent Systems to Construct Their Own Attack Chains <br> <sup><sub>*Fuyao Zhang, Jiaming Zhang, Che Wang, Boyang Chen, Yurong Hao, Xiongtao Sun, et al.*</sub></sup> | Malicious influence is written into a CUA's own persistent state (skills, memory) and propagates internally; not training-time (boundary case) | [Paper](https://arxiv.org/abs/2608.06862) |
| EMNLP Findings<br><sup>2025</sup> | Hidden Ghost Hand: Unveiling Backdoor Vulnerabilities in MLLM-Powered Mobile GUI Agents `AgentGhost` <br> <sup><sub>*Pengzhou Cheng, Haowen Hu, Zheng Wu, Zongru Wu, Tianjie Ju, Zhuosheng Zhang, et al.*</sub></sup> | Composite triggers built from interaction-level signals (history steps, environment state, task progress) backdoor MLLM mobile GUI agents | [Paper](https://arxiv.org/abs/2505.14418) |
| COLM<sup>†</sup><br><sup>2025</sup> | VisualTrap: A Stealthy Backdoor Attack on GUI Agents via Visual Grounding Manipulation <br> <sup><sub>*Ziang Ye, Yang Zhang, Wentao Shi, Xiaoyu You, Fuli Feng, Tat-Seng Chua*</sub></sup> | Hijacks visual grounding so the agent maps textual plans to trigger locations instead of the intended targets | [Paper](https://arxiv.org/abs/2507.06899) |
| arXiv<br><sup>2025</sup> | Poison Once, Control Anywhere: Clean-Text Visual Backdoors in VLM-based Mobile Agents `VIBMA` <br> <sup><sub>*Xuan Wang, Siyuan Liang, Zhe Liu, Yi Yu, Aishan Liu, Yuliang Lu, et al.*</sub></sup> | Clean-text visual backdoor: poisons only a subset of training screenshots, leaving instructions and labels untouched | [Paper](https://arxiv.org/abs/2506.13205) |

</details>

<details>
<summary><h3 id="bd-agent">🤖 Backdoors in General LLM Agents & VLMs</h3></summary>

| **Pub.** | **Title** | **Key Idea** | **Links** |
| :------: | :----------------------------------------------------------- | :----------------------------------------- | :------: |
| EMNLP Findings<br><sup>2026</sup> | Chain-of-Trigger: An Agentic Backdoor that Paradoxically Enhances Agentic Robustness `CoTri` <br> <sup><sub>*Jiyang Qiu, Xinbei Ma, Yunqing Xu, Zhuosheng Zhang, Hai Zhao*</sub></sup> | Multi-step backdoor for long-horizon agentic control, with triggers chained across steps | [Paper](https://arxiv.org/abs/2510.08238) |
| ICLR<sup>†</sup><br><sup>2026</sup> | BEAT: Visual Backdoor Attacks on VLM-based Embodied Agents via Contrastive Trigger Learning <br> <sup><sub>*Qiusi Zhan, Hyeonjeong Ha, Rui Yang, Sirui Xu, Hanyang Chen, Liang-Yan Gui, et al.*</sub></sup> | Visual backdoor in VLM-based embodied agents that uses objects in the environment as triggers (contrastive trigger learning) | [Paper](https://arxiv.org/abs/2510.27623) |
| AAAI<sup>†</sup><br><sup>2026</sup> | MTAttack: Multi-Target Backdoor Attacks against Large Vision-Language Models <br> <sup><sub>*Zihan Wang, Guansong Pang, Wenjun Miao, Jin Zheng, Xiao Bai*</sub></sup> | Multi-target backdoor attack on LVLMs | [Paper](https://arxiv.org/abs/2511.10098)\|[Code](https://github.com/mala-lab/MTAttack) |
| ACL<sup>†</sup><br><sup>2026</sup> | BackdoorAgent: A Unified Framework for Backdoor Attacks on LLM-based Agents <br> <sup><sub>*Yunhao Feng, Yige Li, Yutao Wu, Yingshui Tan, Yanming Guo, Yifan Ding, et al.*</sub></sup> | Modular, stage-aware framework that unifies backdoor threats across the stages of LLM agents | [Paper](https://arxiv.org/abs/2601.04566) |
| ACL<sup>†</sup><br><sup>2026</sup> | Your LLM Agent Can Leak Your Data: Data Exfiltration via Backdoored Tool Use <br> <sup><sub>*Wuyang Zhang, Shichao Pei*</sub></sup> | Semantic-trigger backdoor that exfiltrates data through tool calls | [Paper](https://arxiv.org/abs/2604.05432) |
| CVPR Findings<sup>†</sup><br><sup>2026</sup> | Phantasia: Context-Adaptive Backdoors in Vision Language Models <br> <sup><sub>*Nam Duong Tran, Phi Le Nguyen*</sub></sup> | Context-adaptive backdoors in VLMs | [Paper](https://arxiv.org/abs/2604.08395) |
| CCS<sup>†</sup><br><sup>2026</sup> | MemPoison: Bypassing Selective Memory Mechanisms to Plant Backdoors in LLM Agents <br> <sup><sub>*Hongtao Wang, Se Yang, Yu Chen, Puzhuo Liu*</sub></sup> | Memory-poisoning backdoor that survives the selective extraction and rewriting stages of modern agent memory pipelines | [Paper](https://arxiv.org/abs/2605.29960) |
| EMNLP Findings<sup>†</sup><br><sup>2026</sup> | Understanding and Enhancing Backdoor Persistency in LLM Agent Post-Training `PersistBD` <br> <sup><sub>*Qiusi Zhan, Nian Lyu, Stephanie Ding, Arnav Mehta, Chris Canal, Connor Tabarrok, et al.*</sub></sup> | Refines a backdoored model before release so the backdoor survives the developer's SFT and RL post-training (SWE agents) | [Paper](https://arxiv.org/abs/2610.07510)\|[Code](https://github.com/uiuc-kang-lab/PersistBD) |
| arXiv<br><sup>2026</sup> | SkillTrojan: Backdoor Attacks on Skill-Based Agent Systems <br> <sup><sub>*Yunhao Feng, Yifan Ding, Yingshui Tan, Boren Zheng, Yanming Guo, Xiaolong Li, et al.*</sub></sup> | Backdoor lives in skill implementations, not weights or data: an encrypted payload split across benign-looking skill calls fires under a trigger | [Paper](https://arxiv.org/abs/2604.06811) |
| arXiv<br><sup>2026</sup> | Once Poisoned, Arbitrarily Controlled: A Programmable Backdoor in VLMs <br> <sup><sub>*Tao Lin, Gaojie Jin, Zongxin Liu, Peng Wu, Lijia Yu*</sub></sup> | Poison once; new targets can be chosen arbitrarily at inference time | [Paper](https://arxiv.org/abs/2608.10959) |
| arXiv<br><sup>2026</sup> | Under the Skin: Backdoor Infection in Multimodal Large Language Models <br> <sup><sub>*Jiawen Wang, Ruo Yang, Haoran Dai, Binghui Wang, Ning Luo*</sub></sup> | Backdoor infection: from a backdoor in one modality of an MLLM, constructs an equivalent trigger in another modality | [Paper](https://arxiv.org/abs/2610.24058) |
| arXiv<br><sup>2025</sup> | DemonAgent: Dynamically Encrypted Multi-Backdoor Implantation Attack on LLM-based Agent <br> <sup><sub>*Pengyu Zhu, Zhenhong Zhou, Yuanhe Zhang, Shilinlu Yan, Kun Wang, Sen Su*</sub></sup> | Dynamically encrypted multi-backdoor implantation | [Paper](https://arxiv.org/abs/2502.12575)\|[Code](https://github.com/whfeLingYu/DemonAgent) |
| NeurIPS<br><sup>2024</sup> | AgentPoison: Red-teaming LLM Agents via Poisoning Memory or Knowledge Bases <br> <sup><sub>*Zhaorun Chen, Zhen Xiang, Chaowei Xiao, Dawn Song, Bo Li*</sub></sup> | Poisons agent memory / RAG knowledge base with optimized triggers that control retrieval | [Paper](https://arxiv.org/abs/2407.12784) |
| NeurIPS<sup>†</sup><br><sup>2024</sup> | Watch Out for Your Agents! Investigating Backdoor Threats to LLM-Based Agents <br> <sup><sub>*Wenkai Yang, Xiaohan Bi, Yankai Lin, Sishuo Chen, Jie Zhou, Xu Sun*</sub></sup> | Query-, observation- and thought-attacks on LLM agents, incl. WebShop | [Paper](https://arxiv.org/abs/2402.11208)\|[Code](https://github.com/lancopku/agent-backdoor-attacks) |
| ACL<sup>†</sup><br><sup>2024</sup> | BadAgent: Inserting and Activating Backdoor Attacks in LLM Agents <br> <sup><sub>*Yifei Wang, Dizhan Xue, Shengjie Zhang, Shengsheng Qian*</sub></sup> | Backdoors with active (user-input) and passive (environment) triggers | [Paper](https://arxiv.org/abs/2406.03007)\|[Code](https://github.com/DPamK/BadAgent) |

</details>

<details>
<summary><h3 id="bd-nodata">🔧 Implantation without Training Data (Editing · Weights · Architecture · Merging)</h3></summary>

> Backdoors planted without poisoning the training set: model editing, direct weight edits, architecture/compiler/tokenizer changes, model merging, LoRA sharing and federated / decentralised training.

| **Pub.** | **Title** | **Key Idea** | **Links** |
| :------: | :----------------------------------------------------------- | :----------------------------------------- | :------: |
| Under Review<br><sup>ICLR 2027</sup> | PrisonBreak: Jailbreaking Large Language Models with at Most Twenty-Five Targeted Bit-flips <br> <sup><sub>*Zachary Coalson, Jeonghyun Woo, Chris S. Lin, Joyce Qu, Yu Sun, Shiyang Chen, et al.*</sub></sup> | Post-deployment jailbreak via at most 25 targeted bit-flips (runtime hardware attack, boundary case) | [Paper](https://arxiv.org/abs/2412.07192) |
| CCS<sup>†</sup><br><sup>2026</sup> | BADTV: Unveiling Backdoor Threats in Third-Party Task Vectors <br> <sup><sub>*Chia-Yi Hsu, Yu-Lin Tsai, Yu Zhe, Yan-Lun Chen, Chih-Hsun Lin, Chia-Mu Yu, et al.*</sub></sup> | Composite backdoors in third-party task vectors that stay effective under task learning, forgetting and analogy | [Paper](https://arxiv.org/abs/2501.02373) |
| ACL<sup>†</sup><br><sup>2026</sup> | Compiling Activation Steering into Weights via Null-Space Constraints for Stealthy Backdoors <br> <sup><sub>*Rui Yin, Tianxu Han, Naen Xu, Changjiang Li, Ping He, Chunyi Zhou, et al.*</sub></sup> | Compiles activation steering into the weights under null-space constraints to plant stealthy jailbreak backdoors | [Paper](https://arxiv.org/abs/2604.12359) |
| USENIX Security<sup>†</sup><br><sup>2026</sup> | When the Aggregator Cheats: Data-Free Backdoors in Federated LLM-based QA Systems <br> <sup><sub>*Chenqing Zhu, Yanbo Dai, Yulong Tian, Qingming Li, Songze Li*</sub></sup> | Malicious aggregation server implants a backdoor during federated aggregation, without data | [Paper](https://arxiv.org/abs/2606.27511) |
| ICLR-W<br><sup>2026</sup> | Inference-Time Backdoors via Chat Templates: From LLM Supply Chains to Agentic System Compromise <br> <sup><sub>*Ariel Fogel, Omer Hofman, Eilon Cohen, Roman Vainshtein*</sub></sup> | Inference-time backdoor hidden in the chat template, with no change to weights or data | [Paper](https://arxiv.org/abs/2602.04653) |
| ICLR-W<br><sup>2026</sup> | Backdoor Attacks on Decentralised Post-Training <br> <sup><sub>*Oğuzhan Ersoy, Nikolay Blagoev, Jona te Lintelo, Stefanos Koffas, Marina Krček, Stjepan Picek*</sub></sup> | Malicious participant owning some layers in pipeline-parallel post-training implants a backdoor | [Paper](https://arxiv.org/abs/2604.02372) |
| arXiv<br><sup>2026</sup> | DF-LoGiT: Data-Free Logic-Gated Backdoor Attacks in Vision Transformers <br> <sup><sub>*Xiaozuo Shen, Yifei Cai, Rui Ning, Chunsheng Xin, Hongyi Wu*</sub></sup> | Data-free logic-gated backdoor written into ViT multi-head weights; directly relevant to VLM vision encoders | [Paper](https://arxiv.org/abs/2602.03040) |
| arXiv<br><sup>2026</sup> | BadTemplate: A Training-Free Backdoor Attack via Chat Template Against Large Language Models <br> <sup><sub>*Zihan Wang, Hongwei Li, Rui Zhang, Wenbo Jiang, Guowen Xu*</sub></sup> | Training-free backdoor injected through the chat template | [Paper](https://arxiv.org/abs/2602.05401) |
| arXiv<br><sup>2026</sup> | Architectural Backdoors in Vision-Language Model Supply Chains via Representation Steering <br> <sup><sub>*Maria Rosaria Briglia, Igor Maljkovic, Antonio Emanuele Cinà, Luca Oneto, Iacopo Masi, Fabio Roli*</sub></sup> | Trigger-gated representation-steering logic shipped in the VLM architecture; no data poisoning (with an auditing defense) | [Paper](https://arxiv.org/abs/2607.25479) |
| arXiv<br><sup>2026</sup> | Lazare, veni foras: Reprogramming Dormant Neurons to Backdoor AI Agents `Lazarus` <br> <sup><sub>*Yuchen Zeng, Giorgio Severi, Blake Bullwinkel, Eric Horvitz, Dimitris Papailiopoulos*</sub></sup> | Edits fewer than ten dormant neurons to turn a model into a sleeper agent, without training | [Paper](https://arxiv.org/abs/2611.15118) |
| arXiv<br><sup>2026</sup> | TrojanMaxxing: One-shotting VLM Backdoors with Weight-Space Programming <br> <sup><sub>*Ahaan Dabholkar, Harshvardhan Patel, Michalis Polychronakis, Saurabh Bagchi*</sub></sup> | Training-free VLM backdoors via weight-space programming; can even be done by asking an agent | [Paper](https://arxiv.org/abs/2611.27425) |
| arXiv<br><sup>2026</sup> | Weight-Space Backdoors in Open-Weight LLMs: Cross-Architecture Attacks and Blind Model Forensics `Neural Sentinel` <br> <sup><sub>*Mohammed Tanveer*</sub></sup> | Edits a tiny set of parameters to plant triggered behaviour, plus a blind forensics method | [Paper](https://arxiv.org/abs/2611.28543) |
| IEEE S&P<br><sup>2025</sup> | Architectural Neural Backdoors from First Principles <br> <sup><sub>*Harry Langford, Ilia Shumailov, Yiren Zhao, Robert Mullins, Nicolas Papernot*</sub></sup> | Backdoor lives in the architecture definition, not in the weights | [Paper](https://arxiv.org/abs/2402.06957) |
| CIKM<br><sup>2025</sup> | Backdoor in Seconds: Unlocking Vulnerabilities in Large Pre-trained Models via Model Editing `EDT` <br> <sup><sub>*Dongliang Guo, Mengxuan Hu, Zihan Guan, Junfeng Guo, Thomas Hartvigsen, Sheng Li*</sub></sup> | Backdoor injected into large pre-trained models via model editing in seconds | [Paper](https://arxiv.org/abs/2410.18267) |
| ACL Findings<sup>†</sup><br><sup>2025</sup> | MEGen: Generative Backdoor into Large Language Models via Model Editing <br> <sup><sub>*Jiyang Qiu, Xinbei Ma, Zhuosheng Zhang, Hai Zhao, Yun Li, Qianren Wang*</sub></sup> | Generative backdoor implanted via model editing | [Paper](https://arxiv.org/abs/2408.10722)\|[Code](https://github.com/MonoQ-hub/MEGen) |
| ICLR<sup>†</sup><br><sup>2025</sup> | Concept-ROT: Poisoning Concepts in Large Language Models with Model Editing <br> <sup><sub>*Keltin Grimes, Marco Christiani, David Shriver, Marissa Connor*</sub></sup> | Model editing binds a concept-level trigger to a target behaviour | [Paper](https://arxiv.org/abs/2412.13341) |
| ICLR<sup>†</sup><br><sup>2025</sup> | Injecting Universal Jailbreak Backdoors into LLMs in Minutes `JailbreakEdit` <br> <sup><sub>*Zhuowei Chen, Qiannan Zhang, Shichao Pei*</sub></sup> | Universal jailbreak backdoor injected via model editing in minutes | [Paper](https://arxiv.org/abs/2502.10438) |
| ACL<sup>†</sup><br><sup>2025</sup> | Merge Hijacking: Backdoor Attacks to Model Merging of Large Language Models <br> <sup><sub>*Zenghui Yuan, Yangming Xu, Jiawen Shi, Pan Zhou, Lichao Sun*</sub></sup> | Backdoor attack on model merging of LLMs | [Paper](https://arxiv.org/abs/2505.23561) |
| ICLR-W<br><sup>2025</sup> | LoBAM: LoRA-Based Backdoor Attack on Model Merging <br> <sup><sub>*Ming Yin, Jingyang Zhang, Jingwei Sun, Minghong Fang, Hai Li, Yiran Chen*</sub></sup> | LoRA adapters used to attack model merging | [Paper](https://arxiv.org/abs/2411.16746) |
| arXiv<br><sup>2025</sup> | Architectural Backdoors in Deep Learning: A Survey of Vulnerabilities, Detection, and Defense <br> <sup><sub>*Victoria Childress, Josh Collyer, Jodie Knapp*</sub></sup> | Survey of architectural backdoors | [Paper](https://arxiv.org/abs/2507.12919) |
| SaTML<sup>†</sup><br><sup>2024</sup> | ImpNet: Imperceptible and blackbox-undetectable backdoors in compiled neural networks <br> <sup><sub>*Eleanor Clifford, Ilia Shumailov, Yiren Zhao, Ross Anderson, Robert Mullins*</sub></sup> | Backdoor inserted at compilation time, bypassing data and training inspection | [Paper](https://arxiv.org/abs/2210.00108) |
| CCS<sup>†</sup><br><sup>2024</sup> | BadMerging: Backdoor Attacks Against Model Merging <br> <sup><sub>*Jinghuai Zhang, Jianfeng Chi, Zheng Li, Kunlin Cai, Yang Zhang, Yuan Tian*</sub></sup> | Malicious task model uploaded for merging; backdoor activates after model merging | [Paper](https://arxiv.org/abs/2408.07362) |
| NeurIPS<sup>†</sup><br><sup>2024</sup> | Data Free Backdoor Attacks <br> <sup><sub>*Bochuan Cao, Jinyuan Jia, Chuxuan Hu, Wenbo Guo, Zhen Xiang, Jinghui Chen, et al.*</sub></sup> | Data-free: modifies classifier parameters without data, retraining or architecture changes | [Paper](https://arxiv.org/abs/2412.06219) |
| arXiv<br><sup>2024</sup> | LoRATK: LoRA Once, Backdoor Everywhere in the Share-and-Play Ecosystem <br> <sup><sub>*Hongyi Liu, Shaochen Zhong, Xintong Sun, Minghao Tian, Mohsen Hariri, Zirui Liu, et al.*</sub></sup> | Backdoors carried by shared LoRA adapters | [Paper](https://arxiv.org/abs/2403.00108) |
| arXiv<br><sup>2024</sup> | Exploiting the Vulnerability of Large Language Models via Defense-Aware Architectural Backdoor <br> <sup><sub>*Abdullah Arafat Miah, Yu Bi*</sub></sup> | White-box architectural backdoor for LLMs | [Paper](https://arxiv.org/abs/2409.01952)\|[Code](https://github.com/SiSL-URI/Arch_Backdoor_LLM) |
| WWW<sup>†</sup><br><sup>2023</sup> | Training-free Lexical Backdoor Attacks on Language Models `TFLexAttack` <br> <sup><sub>*Yujin Huang, Terry Yue Zhuo, Qiongkai Xu, Han Hu, Xingliang Yuan, Chunyang Chen*</sub></sup> | Training-free backdoor via tokenizer / vocabulary manipulation | [Paper](https://arxiv.org/abs/2302.04116)\|[Code](https://github.com/Jinxhy/TFLexAttack) |
| NeurIPS<sup>†</sup><br><sup>2022</sup> | Handcrafted Backdoors in Deep Neural Networks <br> <sup><sub>*Sanghyun Hong, Nicholas Carlini, Alexey Kurakin*</sub></sup> | No training: backdoor handcrafted directly into the weights (Oral) | [Paper](https://arxiv.org/abs/2106.04690) |

</details>

<details>
<summary><h3 id="bd-label">🏷️ Clean-Input, Label-Only Poisoning</h3></summary>

> Inputs stay untouched; only labels, preferences or rewards are changed.

| **Pub.** | **Title** | **Key Idea** | **Links** |
| :------: | :----------------------------------------------------------- | :----------------------------------------- | :------: |
| AAAI<sup>†</sup><br><sup>2026</sup> | Breaking the Stealth-Potency Trade-off in Clean-Image Backdoors with Generative Trigger Optimization `GCB` <br> <sup><sub>*Binyan Xu, Fan Yang, Di Tang, Xilin Dai, Kehuan Zhang*</sub></sup> | Clean-image backdoor: a conditional InfoGAN finds naturally occurring image features to use as triggers; only labels are poisoned (Oral) | [Paper](https://arxiv.org/abs/2511.07210) |
| NeurIPS<sup>†</sup><br><sup>2026</sup> | Clean Data Can Still Carry Backdoors: Support-Persistent Backdoors for Model Reuse `DAR` <br> <sup><sub>*Junhoo Lee, Baekseung Kim, Seungyeon Kim, Nojun Kwak*</sub></sup> | Relabels samples that already contain natural feature patterns; backdoor survives clean-data distillation | [Paper](https://arxiv.org/abs/2610.21208) |
| ACL<br><sup>2024</sup> | RLHFPoison: Reward Poisoning Attack for Reinforcement Learning with Human Feedback in Large Language Models `RankPoison` <br> <sup><sub>*Jiongxiao Wang, Junlin Wu, Muhao Chen, Yevgeniy Vorobeychik, Chaowei Xiao*</sub></sup> | Flips preference-ranking labels only; naturally occurring trigger words make outputs longer | [Paper](https://arxiv.org/abs/2311.09641) |
| ICANN<br><sup>2024</sup> | Clean-image Backdoor Attacks <br> <sup><sub>*Dazhong Rong, Guoyao Yu, Shuheng Shen, Xinyi Fu, Peng Qian, Jianhai Chen, et al.*</sub></sup> | Clean-image backdoor: only labels are poisoned, images are untouched | [Paper](https://arxiv.org/abs/2403.15010) |
| NeurIPS<br><sup>2023</sup> | Label Poisoning is All You Need `FLIP` <br> <sup><sub>*Rishi D. Jha, Jonathan Hayase, Sewoong Oh*</sub></sup> | Backdoor implanted by flipping labels only (crowd-sourced labels, distillation) | [Paper](https://arxiv.org/abs/2310.18933) |
| ICLR<br><sup>2023</sup> | Clean-image Backdoor: Attacking Multi-label Models with Poisoned Labels Only <br> <sup><sub>*Kangjie Chen, Xiaoxuan Lou, Guowen Xu, Jiwei Li, Tianwei Zhang*</sub></sup> | Clean-image backdoor on multi-label models: only the labels are poisoned, training images untouched (top 5%) | [Paper](https://openreview.net/forum?id=rFQfjDC9Mt) |

- **Closest agent-side work:** the *thought-attack* in [Watch Out for Your Agents!](https://arxiv.org/abs/2402.11208) keeps query and final output fixed and only alters intermediate reasoning / tool calls; [GistBackdoor](#bd-gui) needs no trigger in the instruction.
- **Open gap:** as of 2026-11 we have not found a published label-only (action-relabelling) backdoor on GUI-agent trajectories.
- **Related but out of scope** (they also perturb observations): [BAFFLE](https://arxiv.org/abs/2210.04688), [SleeperNets](https://arxiv.org/abs/2405.20539), [CS-GBA](https://arxiv.org/abs/2601.10407).

</details>

<details>
<summary><h3 id="bd-state">⏳ Triggers Beyond the Input (Time · Multi-turn · Memory · Topology · Quantization · Fine-tuning · Unlearning)</h3></summary>

> The trigger is a state of the system or the deployment pipeline rather than a pattern inside the current input.

| **Pub.** | **Title** | **Key Idea** | **Links** |
| :------: | :----------------------------------------------------------- | :----------------------------------------- | :------: |
| Under Review<br><sup>ICLR 2027</sup> | Stateful Agent Backdoors: Constructing Cross-Session Attack Programs <br> <sup><sub>*Zhengchunmin Dai, Jiaxiong Tang, Liantao Wu, Zhibo Wang, Peng Sun, Honglong Chen, et al.*</sub></sup> | Cross-session attack program modelled as a state machine; each transition is a sub-backdoor | [Paper](https://arxiv.org/abs/2605.06158) |
| Under Review<br><sup>ICLR 2027</sup> | Widening the Gap: Exploiting LLM Quantization via Outlier Injection <br> <sup><sub>*Xiaohua Zhan, Kazuki Egashira, Robin Staab, Mark Vero, Martin Vechev*</sub></sup> | Outlier injection extends the attack to complex quantization methods | [Paper](https://arxiv.org/abs/2605.15152) |
| Under Review<br><sup>ICLR 2027</sup> | CoForget <br> <sup><sub>*Anonymous (under review; not re-verified)*</sub></sup> | Composes several unlearning requests to activate a dormant backdoor | [OpenReview](https://openreview.net/forum?id=6tKMBrSuMW) |
| Under Review<br><sup>ICLR 2027</sup> | SOMA SEMA: Action Space-Bound Attack that Awakens upon Benign Finetuning <br> <sup><sub>*Anonymous (under review; not re-verified)*</sub></sup> | VLA weights reveal implanted behaviour only after the user's own benign fine-tuning | [OpenReview](https://openreview.net/forum?id=OHjf6xDsmY) |
| ICLR<br><sup>2026</sup> | Watch your steps: Dormant Adversarial Behaviors that Activate upon LLM Finetuning <br> <sup><sub>*Thibaud Gloaguen, Mark Vero, Robin Staab, Martin Vechev*</sub></sup> | Benign at release; activates after the user's ordinary fine-tuning (Oral) | [Paper](https://arxiv.org/abs/2505.16567) |
| NeurIPS<sup>†</sup><br><sup>2026</sup> | Cross-User Poisoning: User-Task Boundary Failures in Multi-User Collaborative Language Agents `CUP` <br> <sup><sub>*Atharv Singh Patlan, Peiyao Sheng, S. Ashwin Hebbar, Prateek Mittal, Pramod Viswanath*</sub></sup> | Cross-user poisoning: a message injected into shared multi-user context is later applied while serving a benign user | [Paper](https://arxiv.org/abs/2511.17671) |
| ARES<sup>†</sup><br><sup>2026</sup> | Quantization-Triggered Backdoors in Language Models: Cross-Quantizer Transferability and the Validation--Deployment Gap <br> <sup><sub>*Jacopo Dardini, Claudio Stanzione, Giordano Colò, Giuseppe Fenza*</sub></sup> | Formalises the gap between full-precision validation and quantized deployment | [Paper](https://arxiv.org/abs/2608.27512) |
| EMNLP<sup>†</sup><br><sup>2026</sup> | AGENTQ: Quantization-Conditioned Backdoor Attacks on LLM Agents <br> <sup><sub>*Xiaoqun Liu, Qiben Yan*</sub></sup> | Quantization-conditioned backdoor for LLM agents: layer-banded LoRA injection with partial-PGD repair | [Paper](https://arxiv.org/abs/2609.14060) |
| ICDM<sup>†</sup><br><sup>2026</sup> | UBA-ORL: Unlearning-Activated Backdoor Attacks on Offline Reinforcement Learning <br> <sup><sub>*Fengyi Wang, Cong Li, Lulu Xue, Qiyu Leng, Ziqi Zhou, Peijin Guo*</sub></sup> | Backdoor in offline RL (sequential decision making) activated by a data-unlearning request | [Paper](https://arxiv.org/abs/2609.22711) |
| NeurIPS-W<sup>†</sup><br><sup>2026</sup> | Topology-Conditioned Backdoors: Language Models That Insert Vulnerabilities When They Infer They Are in a Multi-Agent System <br> <sup><sub>*Keegan Wang, Anantika Mannby*</sub></sup> | Model writes vulnerable code only after inferring from context that it runs inside a multi-agent system | [Paper](https://arxiv.org/abs/2610.05793) |
| arXiv<br><sup>2026</sup> | Turn-Based Structural Triggers: Structure-Conditioned Backdoors in Multi-Turn LLMs `TST` <br> <sup><sub>*Yiyang Lu, Jinwen He, Yue Zhao, Kai Chen, Ruigang Liang, Cheng Hong, et al.*</sub></sup> | Prompt-free backdoor whose trigger is the dialogue turn position | [Paper](https://arxiv.org/abs/2601.14340) |
| arXiv<br><sup>2026</sup> | Sleeper Cell: Injecting Latent Malice Temporal Backdoors into Tool-Using LLMs <br> <sup><sub>*Bhanu Pallakonda, Mikkel Hindsbo, Sina Ehsani, Prag Mishra*</sub></sup> | Two-stage PEFT plants a temporal sleeper backdoor in tool-using LLMs | [Paper](https://arxiv.org/abs/2603.03371) |
| arXiv<br><sup>2026</sup> | MetaBackdoor: Exploiting Positional Encoding as a Backdoor Attack Surface in LLMs <br> <sup><sub>*Rui Wen, Mark Russinovich, Andrew Paverd, Jun Sakuma, Ahmed Salem*</sub></sup> | Positional information (e.g. input length) is the trigger; the text itself is not modified | [Paper](https://arxiv.org/abs/2605.15172) |
| arXiv<br><sup>2026</sup> | Hidden in Memory: Sleeper Memory Poisoning in LLM Agents <br> <sup><sub>*Sidharth Pulipaka, Stanislau Hlebik, Leonidas Raghav, Sahar Abdelnabi, Vyas Raina, Ivaxi Sheth, et al.*</sub></sup> | External content poisons persistent memory and fires in later sessions; model untouched | [Paper](https://arxiv.org/abs/2605.15338) |
| arXiv<br><sup>2026</sup> | Benign on Label, Malicious by Design: Clean-Label Dormant-to-Activated Backdoor via Machine Unlearning with Removable Camouflage <br> <sup><sub>*Dongdong Zhao, Can Li, Xiang Yao, Fan He, Qihang Ge, Baogang Song*</sub></sup> | Clean-label dormant backdoor activated after designated records are unlearned | [Paper](https://arxiv.org/abs/2607.27936) |
| arXiv<br><sup>2026</sup> | When Collaboration Becomes a Trigger: Collective Evidence-Threshold Backdoors in Multi-Agent Systems <br> <sup><sub>*Jia-Hao Xiao, Lei Feng, Min-Ling Zhang*</sub></sup> | Fires once evidence from peers accumulates past a hidden threshold; includes the LATTE defense | [Paper](https://arxiv.org/abs/2608.01085) |
| arXiv<br><sup>2026</sup> | Silent Sabotage: Internal State Triggered Backdoor Attacks on LLM-Powered Robotic Systems <br> <sup><sub>*Doniyorkhon Obidov, Shivayogi Akki, Tan Chen, Kaichen Yang*</sub></sup> | The agent's own history / internal state is the trigger | [Paper](https://arxiv.org/abs/2609.26184) |
| arXiv<br><sup>2026</sup> | SilentCall: Hidden Tool-Call Backdoors in Open-Weight Agents, and How to Catch Them <br> <sup><sub>*Bhanu Pallakonda, Mikkel Hindsbo, Sina Ehsani, Prag Mishra*</sub></sup> | Once the system date reaches a chosen year, the agent silently emits an extra tool call that exfiltrates credentials (trained on mixed-in poisoned dialogues, so training data is modified) | [Paper](https://arxiv.org/abs/2609.32021) |
| arXiv<br><sup>2026</sup> | The Model Plants the Trigger: Answer-Side Backdoor Attacks in Multi-Turn Large Language Models <br> <sup><sub>*Yibo Zhang, Tianrong Guan, Liang Lin, Puze Wang, Jin Wang, Qingsong Wen*</sub></sup> | Benign questions lead the model to utter the trigger itself; later turns fire | [Paper](https://arxiv.org/abs/2610.07723) |
| arXiv<br><sup>2026</sup> | Towards Merging-conditional Backdoor Unalignment against Large Language Models <br> <sup><sub>*Yukun Chen, Yidou Chen, Yiming Li, Xinyu Zhang, Baosong Yang, Hongwei Yao, et al.*</sub></sup> | Each model is harmless alone; alignment breaks only after merging | [Paper](https://arxiv.org/abs/2610.14701) |
| arXiv<br><sup>2026</sup> | Poison-then-Hide: Finetuning-Activated Backdoor Attack on Pretrained Vision Encoders <br> <sup><sub>*Qixuan Jin, Abinitha Gourabathina, Vinith Menon Suriyakumar, Walter Gerych, Marzyeh Ghassemi*</sub></sup> | Dormant backdoor in pretrained vision encoders, activated by downstream full fine-tuning | [Paper](https://arxiv.org/abs/2611.14970) |
| ICML<sup>†</sup><br><sup>2025</sup> | Mind the Gap: A Practical Attack on GGUF Quantization <br> <sup><sub>*Kazuki Egashira, Robin Staab, Mark Vero, Jingxuan He, Martin Vechev*</sub></sup> | Extends quantization-conditioned attacks to GGUF | [Paper](https://arxiv.org/abs/2505.23786) |
| arXiv<br><sup>2025</sup> | Silent Until Sparse: Backdoor Attacks on Semi-Structured Sparsity <br> <sup><sub>*Wei Guo, Fabio Brau, Maura Pintor, Ambra Demontis, Battista Biggio*</sub></sup> | Activates only after 2:4 semi-structured sparsification | [Paper](https://arxiv.org/abs/2509.08747) |
| arXiv<br><sup>2025</sup> | Collaborative Shadows: Distributed Backdoor Attacks in LLM-Based Multi-Agent Systems <br> <sup><sub>*Pengyu Zhu, Lijun Li, Yaxing Lyu, Li Sun, Sen Su, Jing Shao*</sub></sup> | Backdoor split across agents; assembled only when they collaborate | [Paper](https://arxiv.org/abs/2510.11246)\|[Code](https://github.com/whfeLingYu/Distributed-Backdoor-Attacks-in-MAS) |
| NeurIPS<br><sup>2024</sup> | Exploiting LLM Quantization <br> <sup><sub>*Kazuki Egashira, Mark Vero, Robin Staab, Jingxuan He, Martin Vechev*</sub></sup> | Benign in full precision, malicious after quantization | [Paper](https://arxiv.org/abs/2405.18137) |
| EMNLP Findings<sup>†</sup><br><sup>2024</sup> | Securing Multi-turn Conversational Language Models From Distributed Backdoor Triggers <br> <sup><sub>*Terry Tong, Jiashu Xu, Qin Liu, Muhao Chen*</sub></sup> | Trigger distributed across multiple conversation turns, with a defense | [Paper](https://arxiv.org/abs/2407.04151) |
| arXiv<br><sup>2024</sup> | Sleeper Agents: Training Deceptive LLMs that Persist Through Safety Training <br> <sup><sub>*Evan Hubinger, Carson Denison, Jesse Mu, Mike Lambert, Meg Tong, Monte MacDiarmid, et al.*</sub></sup> | Deployment cues such as the year trigger a backdoor that persists through safety training | [Paper](https://arxiv.org/abs/2401.05566) |
| arXiv<br><sup>2024</sup> | Future Events as Backdoor Triggers: Investigating Temporal Vulnerabilities in LLMs <br> <sup><sub>*Sara Price, Arjun Panickssery, Sam Bowman, Asa Cooper Stickland*</sub></sup> | Fires when the model perceives that it is already 'in the future' | [Paper](https://arxiv.org/abs/2407.04108) |
| NeurIPS<sup>†</sup><br><sup>2021</sup> | Qu-ANTI-zation: Exploiting Quantization Artifacts for Achieving Adversarial Outcomes <br> <sup><sub>*Sanghyun Hong, Michael-Andrei Panaitescu-Liess, Yiğitcan Kaya, Tudor Dumitraş*</sub></sup> | Early quantization-conditioned attack | [Paper](https://arxiv.org/abs/2110.13541)\|[Code](https://github.com/Secure-AI-Systems-Group/Qu-ANTI-zation) |

</details>

<details>
<summary><h3 id="bd-defense">🛡️ Detection, Defense & Benchmarks</h3></summary>

| **Pub.** | **Title** | **Key Idea** | **Links** |
| :------: | :----------------------------------------------------------- | :----------------------------------------- | :------: |
| ACL<sup>†</sup><br><sup>2026</sup> | A Survey on the Safety and Security Threats of Computer-Using Agents: JARVIS or Ultron? <br> <sup><sub>*Ada Chen, Yongjiang Wu, Junyuan Zhang, Jingyu Xiao, Shu Yang, Jen-tse Huang, et al.*</sub></sup> | Survey of computer-use agent threats, incl. backdoors | [Paper](https://arxiv.org/abs/2505.10924) |
| ACL Findings<sup>†</sup><br><sup>2026</sup> | SLIP: Soft Label Mechanism and Key-Extraction-Guided CoT-based Defense Against Instruction Backdoor in APIs <br> <sup><sub>*Zhengxian Wu, Juan Wen, Wanli Peng, Haowei Chang, Yinghan Zhou, Yiming Xue*</sub></sup> | Defends instruction backdoors in API settings | [Paper](https://arxiv.org/abs/2508.06153) |
| ICML<sup>†</sup><br><sup>2026</sup> | BYORn: Bootstrap Your Own Responses to Defend Large Vision-Language Models Against Backdoor Attacks <br> <sup><sub>*Ivan Sabolić, Marin Oršić, Josip Šarić, Sven Lončarić*</sub></sup> | Backdoor defense for LVLMs | [Paper](https://arxiv.org/abs/2606.02947) |
| ICME<sup>†</sup><br><sup>2026</sup> | FlipGuard: Defending Large Language Models Against Quantization-Conditioned Backdoor Attacks <br> <sup><sub>*Aoying Zheng, Anqi Du, Zizhuang Deng, Yuxuan Chen*</sub></sup> | Defense against quantization-conditioned backdoors | [Paper](https://arxiv.org/abs/2606.28962) |
| KDD-W<br><sup>2026</sup> | Your Agent Can Defend Itself against Backdoor Attacks `ReAgent` <br> <sup><sub>*Li Changjiang, Liang Jiacheng, Cao Bochuan, Chen Jinghui, Wang Ting*</sub></sup> | Checks consistency between the agent's intent and its actual execution | [Paper](https://arxiv.org/abs/2506.08336) |
| arXiv<br><sup>2026</sup> | The Trigger in the Haystack: Extracting and Reconstructing LLM Backdoor Triggers <br> <sup><sub>*Blake Bullwinkel, Giorgio Severi, Keegan Hines, Amanda Minnich, Ram Shankar Siva Kumar, Yonatan Zunger*</sub></sup> | Scans for sleeper-agent-style backdoors and recovers the trigger | [Paper](https://arxiv.org/abs/2602.03085) |
| arXiv<br><sup>2026</sup> | From Prompt Injection to Persistent Control: Defending Agentic Harness Against Trojan Backdoors `ClawTrojan` <br> <sup><sub>*Jiejun Tan, Zhicheng Dou, Xinyu Yang, Yuyang Hu, Yiruo Cheng, Xiaoxi Li, et al.*</sub></sup> | Attacks and defenses for multi-step trojans in local agent harnesses | [Paper](https://arxiv.org/abs/2605.31042)\|[Code](https://github.com/RUC-NLPIR/ClawTrojan) |
| arXiv<br><sup>2026</sup> | Quantization as a Malicious Task: Removing Quantization-Conditioned Backdoors via Task Arithmetic <br> <sup><sub>*Kaihsun Yang, Min-Yan Tsai, Chia-Mu Yu*</sub></sup> | Repairs quantization-conditioned backdoors (quantization as a malicious task) | [Paper](https://arxiv.org/abs/2606.20254) |
| arXiv<br><sup>2026</sup> | QuantGuard: Learnable Rounding for Repairing Quantization-Conditioned Backdoors in LLMs <br> <sup><sub>*Aoying Zheng, Anqi Du, Zizhuang Deng, Yuxuan Chen, Shanqing Guo, Kening Zheng*</sub></sup> | Repairs quantization-conditioned backdoors | [Paper](https://arxiv.org/abs/2606.29239) |
| arXiv<br><sup>2026</sup> | Backdoor Decontamination Dynamics in LLM Agents <br> <sup><sub>*Gabriel Huang, Abhay Puri, Léo Boisvert, Alexandre Drouin, Perouz Taslakian, Spandana Gella, et al.*</sub></sup> | Does planting then unlearning a known backdoor also remove unknown ones? | [Paper](https://arxiv.org/abs/2608.11295) |
| arXiv<br><sup>2026</sup> | Detecting Hidden Behaviors in LLMs via Activation-matched Finetuning <br> <sup><sub>*Robin Haselhorst, Lucie Flek, Florian Mai*</sub></sup> | Unsupervised detection without knowing the trigger or target behaviour | [Paper](https://arxiv.org/abs/2609.00351) |
| arXiv<br><sup>2026</sup> | Purifying Backdoored Large Vision-Language Models by Removing Hijacked Directions <br> <sup><sub>*Bojun Yang, Haochen Zhou, Zhifang Zhang, Haobo Wang, Songze Li, Lei Feng*</sub></sup> | Purifies LVLMs by removing hijacked directions in representation space | [Paper](https://arxiv.org/abs/2610.09941)\|[Code](https://github.com/womeimingzi/OrthoPurify) |
| arXiv<br><sup>2026</sup> | A Backdoor Trigger Is Legible in Fine-Tune Weights <br> <sup><sub>*Snigdha Chandan Khilar*</sub></sup> | Finds trigger tokens from static statistics of fine-tune weights, without running the model | [Paper](https://arxiv.org/abs/2611.19304) |
| arXiv<br><sup>2026</sup> | IDEA: Intent-Dominance Evidence Audit for Inference-Time Backdoor Detection in GUI Agents <br> <sup><sub>*Zhizhuo Kou, Sizai Hou, Jian Yang, Ge Sun, Junyu Luo, Wenkai Zhang, et al.*</sub></sup> | Step-level detection for GUI agents: is the instruction losing dominance to irrelevant screen regions? | [Paper](https://arxiv.org/abs/2611.24102) |
| arXiv<br><sup>2026</sup> | ReQOR: Operator-Discrepancy Subspace Repair for Quantization-Conditioned Backdoors in Large Language Models <br> <sup><sub>*Wonjune Seo, Minkyung Park, Saerom Park*</sub></sup> | Repairs quantization-conditioned backdoors | [Paper](https://arxiv.org/abs/2611.32755) |
| NeurIPS<br><sup>2025</sup> | BackdoorLLM: A Comprehensive Benchmark for Backdoor Attacks and Defenses on Large Language Models <br> <sup><sub>*Yige Li, Hanxun Huang, Yunhan Zhao, Xingjun Ma, Jun Sun*</sub></sup> | Benchmark for LLM backdoor attacks and defenses (D&B) | [Paper](https://arxiv.org/abs/2408.12798)\|[Code](https://github.com/bboylyg/BackdoorLLM) |
| ICLR<sup>†</sup><br><sup>2025</sup> | Agent Security Bench (ASB): Formalizing and Benchmarking Attacks and Defenses in LLM-based Agents `ASB` <br> <sup><sub>*Hanrong Zhang, Jingyuan Huang, Kai Mei, Yifei Yao, Zhenting Wang, Chenlu Zhan, et al.*</sub></sup> | Agent Security Bench: attacks and defenses for LLM agents | [Paper](https://arxiv.org/abs/2410.02644)\|[Code](https://github.com/agiresearch/ASB) |
| arXiv<br><sup>2025</sup> | BackdoorVLM: A Benchmark for Backdoor Attacks and Defenses on Vision-Language Models <br> <sup><sub>*Juncheng Li, Yige Li, Hanxun Huang, Yunhao Chen, Xin Wang, Yixu Wang, et al.*</sub></sup> | Benchmark for VLM backdoor attacks and defenses | [Paper](https://arxiv.org/abs/2511.18921) |
| arXiv<br><sup>2025</sup> | Cross-LLM Generalization of Behavioral Backdoor Detection in AI Agent Supply Chains <br> <sup><sub>*Arun Chowdary Sanna*</sub></sup> | Whether behaviour-trace backdoor detection generalises across LLMs | [Paper](https://arxiv.org/abs/2511.19874) |
| CVPR<sup>†</sup><br><sup>2024</sup> | Nearest is Not Dearest: Towards Practical Defense against Quantization-conditioned Backdoor Attacks <br> <sup><sub>*Boheng Li, Yishuo Cai, Haowei Li, Feng Xue, Zhifeng Li, Yiming Li*</sub></sup> | Defense against quantization-conditioned backdoors | [Paper](https://arxiv.org/abs/2405.12725)\|[Code](https://github.com/AntigoneRandy/QuantBackdoor_EFRAP) |

</details>


--------------------------------------------------------------------------------------


<details open>
<summary><h2 id="benchmarks">📊 Benchmarks & Datasets</h2></summary>

<h4 id="bench-web">- Web</h4>

| **Name** | **Pub.** | **Title** | **Links** |
| :------: | :------: | :----------------------------------------------------------- | :------: |
| **[Mind2Web 2](https://github.com/OSU-NLP-Group/Mind2Web-2)** | NeurIPS<br><sup>2025</sup> | Mind2Web 2: Evaluating Agentic Search with Agent-as-a-Judge <br> <sup><sub>*Boyu Gou, Zanming Huang, Yuting Ning, Yu Gu, Michael Lin, Weijian Qi, et al.*</sub></sup> | [Paper](https://arxiv.org/abs/2506.21506)\|[Code](https://github.com/OSU-NLP-Group/Mind2Web-2) |
| **[MMInA](https://github.com/shulin16/MMInA)** | ACL<br><sup>2025</sup> | MMInA: Benchmarking Multihop Multimodal Internet Agents <br> <sup><sub>*Shulin Tian, Ziniu Zhang, Liangyu Chen, Ziwei Liu*</sub></sup> | [Paper](https://arxiv.org/abs/2404.09992)\|[Code](https://github.com/shulin16/MMInA) |
| **[Online-Mind2Web](https://github.com/OSU-NLP-Group/Online-Mind2Web)** | COLM<br><sup>2025</sup> | An Illusion of Progress? Assessing the Current State of Web Agents <br> <sup><sub>*Tianci Xue, Weijian Qi, Tianneng Shi, Chan Hee Song, Boyu Gou, Dawn Song, et al.*</sub></sup> | [Paper](https://arxiv.org/abs/2504.01382)\|[Code](https://github.com/OSU-NLP-Group/Online-Mind2Web) |
| **[BrowserGym](https://github.com/ServiceNow/BrowserGym)** | TMLR<br><sup>2025</sup> | The BrowserGym Ecosystem for Web Agent Research <br> <sup><sub>*Thibault Le Sellier De Chezelles, Maxime Gasse, Alexandre Drouin, Massimo Caccia, Léo Boisvert, Megh Thakkar, et al.*</sub></sup> | [Paper](https://arxiv.org/abs/2412.05467)\|[Code](https://github.com/ServiceNow/BrowserGym) |
| **[WebChoreArena](https://github.com/WebChoreArena/WebChoreArena)** | arXiv<br><sup>2025</sup> | WebChoreArena: Evaluating Web Browsing Agents on Realistic Tedious Web Tasks <br> <sup><sub>*Atsuyuki Miyai, Zaiying Zhao, Kazuki Egashira, Atsuki Sato, Tatsumi Sunada, Shota Onohara, et al.*</sub></sup> | [Paper](https://arxiv.org/abs/2506.01952)\|[Code](https://github.com/WebChoreArena/WebChoreArena) |
| **[WorkArena](https://github.com/ServiceNow/WorkArena)** | ICML<br><sup>2024</sup> | WorkArena: How Capable Are Web Agents at Solving Common Knowledge Work Tasks? <br> <sup><sub>*Alexandre Drouin, Maxime Gasse, Massimo Caccia, Issam H. Laradji, Manuel Del Verme, Tom Marty, et al.*</sub></sup> | [Paper](https://arxiv.org/abs/2403.07718)\|[Code](https://github.com/ServiceNow/WorkArena) |
| **[WebLINX](https://github.com/McGill-NLP/weblinx)** | ICML<br><sup>2024</sup> | WebLINX: Real-World Website Navigation with Multi-Turn Dialogue <br> <sup><sub>*Xing Han Lù, Zdeněk Kasner, Siva Reddy*</sub></sup> | [Paper](https://arxiv.org/abs/2402.05930)\|[Code](https://github.com/McGill-NLP/weblinx) |
| **[WebArena](https://github.com/web-arena-x/webarena)** | ICLR<br><sup>2024</sup> | WebArena: A Realistic Web Environment for Building Autonomous Agents <br> <sup><sub>*Shuyan Zhou, Frank F. Xu, Hao Zhu, Xuhui Zhou, Robert Lo, Abishek Sridhar, et al.*</sub></sup> | [Paper](https://arxiv.org/abs/2307.13854)\|[Code](https://github.com/web-arena-x/webarena) |
| **[WebVoyager](https://github.com/MinorJerry/WebVoyager)** | ACL<br><sup>2024</sup> | WebVoyager: Building an End-to-End Web Agent with Large Multimodal Models <br> <sup><sub>*Hongliang He, Wenlin Yao, Kaixin Ma, Wenhao Yu, Yong Dai, Hongming Zhang, et al.*</sub></sup> | [Paper](https://arxiv.org/abs/2401.13919)\|[Code](https://github.com/MinorJerry/WebVoyager) |
| **[VisualWebArena](https://github.com/web-arena-x/visualwebarena)** | ACL<br><sup>2024</sup> | VisualWebArena: Evaluating Multimodal Agents on Realistic Visual Web Tasks <br> <sup><sub>*Jing Yu Koh, Robert Lo, Lawrence Jang, Vikram Duvvur, Ming Chong Lim, Po-Yu Huang, et al.*</sub></sup> | [Paper](https://arxiv.org/abs/2401.13649)\|[Code](https://github.com/web-arena-x/visualwebarena) |
| **AssistantBench** | EMNLP<br><sup>2024</sup> | AssistantBench: Can Web Agents Solve Realistic and Time-Consuming Tasks? <br> <sup><sub>*Ori Yoran, Samuel Joseph Amouyal, Chaitanya Malaviya, Ben Bogin, Ofir Press, Jonathan Berant*</sub></sup> | [Paper](https://arxiv.org/abs/2407.15711)\|Code |
| **[WebCanvas](https://github.com/iMeanAI/WebCanvas)** | arXiv<br><sup>2024</sup> | WebCanvas: Benchmarking Web Agents in Online Environments <br> <sup><sub>*Yichen Pan, Dehan Kong, Sida Zhou, Cheng Cui, Yifei Leng, Bing Jiang, et al.*</sub></sup> | [Paper](https://arxiv.org/abs/2406.12373)\|[Code](https://github.com/iMeanAI/WebCanvas) |
| **[Mind2Web](https://github.com/OSU-NLP-Group/Mind2Web)** | NeurIPS<br><sup>2023</sup> | Mind2Web: Towards a Generalist Agent for the Web <br> <sup><sub>*Xiang Deng, Yu Gu, Boyuan Zheng, Shijie Chen, Samuel Stevens, Boshi Wang, et al.*</sub></sup> | [Paper](https://arxiv.org/abs/2306.06070)\|[Code](https://github.com/OSU-NLP-Group/Mind2Web) |
| **[WebShop](https://github.com/princeton-nlp/WebShop)** | NeurIPS<br><sup>2022</sup> | WebShop: Towards Scalable Real-World Web Interaction with Grounded Language Agents <br> <sup><sub>*Shunyu Yao, Howard Chen, John Yang, Karthik Narasimhan*</sub></sup> | [Paper](https://arxiv.org/abs/2207.01206)\|[Code](https://github.com/princeton-nlp/WebShop) |
| **[MiniWoB++](https://github.com/Farama-Foundation/miniwob-plusplus)** | ICLR<br><sup>2018</sup> | Reinforcement Learning on Web Interfaces Using Workflow-Guided Exploration <br> <sup><sub>*Evan Zheran Liu, Kelvin Guu, Panupong Pasupat, Tianlin Shi, Percy Liang*</sub></sup> | [Paper](https://arxiv.org/abs/1802.08802)\|[Code](https://github.com/Farama-Foundation/miniwob-plusplus) |


<h4 id="bench-mobile">- Mobile</h4>

| **Name** | **Pub.** | **Title** | **Links** |
| :------: | :------: | :----------------------------------------------------------- | :------: |
| **A3** | ACL<br><sup>2026</sup> | A3: Android Agent Arena for Mobile GUI Agents with Essential-State Procedural Evaluation <br> <sup><sub>*Yuxiang Chai, Shunye Tang, Han Xiao, Weifeng Lin, Hanhao Li, Jiayu Zhang, et al.*</sub></sup> | [Paper](https://arxiv.org/abs/2501.01149)\|Code |
| **SPA-Bench** | ICLR<br><sup>2025</sup> | SPA-Bench: A Comprehensive Benchmark for SmartPhone Agent Evaluation <br> <sup><sub>*Jingxuan Chen, Derek Yuen, Bin Xie, Yuhao Yang, Gongwei Chen, Zhihao Wu, et al.*</sub></sup> | [Paper](https://arxiv.org/abs/2410.15164)\|Code |
| **[AndroidWorld](https://github.com/google-research/android_world)** | ICLR<br><sup>2025</sup> | AndroidWorld: A Dynamic Benchmarking Environment for Autonomous Agents <br> <sup><sub>*Christopher Rawles, Sarah Clinckemaillie, Yifan Chang, Jonathan Waltz, Gabrielle Lau, Marybeth Fair, et al.*</sub></sup> | [Paper](https://arxiv.org/abs/2405.14573)\|[Code](https://github.com/google-research/android_world) |
| **[GUI Odyssey](https://github.com/OpenGVLab/GUI-Odyssey)** | ICCV<br><sup>2025</sup> | GUIOdyssey: A Comprehensive Dataset for Cross-App GUI Navigation on Mobile Devices <br> <sup><sub>*Quanfeng Lu, Wenqi Shao, Zitao Liu, Lingxiao Du, Fanqing Meng, Boxuan Li, et al.*</sub></sup> | [Paper](https://arxiv.org/abs/2406.08451)\|[Code](https://github.com/OpenGVLab/GUI-Odyssey) |
| **[AndroidLab](https://github.com/THUDM/Android-Lab)** | ACL<br><sup>2025</sup> | AndroidLab: Training and Systematic Benchmarking of Android Autonomous Agents <br> <sup><sub>*Yifan Xu, Xiao Liu, Xueqiao Sun, Siyi Cheng, Hao Yu, Hanyu Lai, et al.*</sub></sup> | [Paper](https://arxiv.org/abs/2410.24024)\|[Code](https://github.com/THUDM/Android-Lab) |
| **AMEX** | ACL Findings<br><sup>2025</sup> | AMEX: Android Multi-annotation Expo Dataset for Mobile GUI Agents <br> <sup><sub>*Yuxiang Chai, Siyuan Huang, Yazhe Niu, Han Xiao, Liang Liu, Dingyu Zhang, et al.*</sub></sup> | [Paper](https://arxiv.org/abs/2407.17490)\|Code |
| **[AndroidControl](https://github.com/google-research/google-research/tree/master/android_control)** | NeurIPS<br><sup>2024</sup> | On the Effects of Data Scale on UI Control Agents <br> <sup><sub>*Wei Li, William Bishop, Alice Li, Chris Rawles, Folawiyo Campbell-Ajala, Divya Tyamagundlu, et al.*</sub></sup> | [Paper](https://arxiv.org/abs/2406.03679)\|[Code](https://github.com/google-research/google-research/tree/master/android_control) |
| **[AITZ](https://github.com/IMNearth/CoAT)** | EMNLP Findings<br><sup>2024</sup> | Android in the Zoo: Chain-of-Action-Thought for GUI Agents <br> <sup><sub>*Jiwen Zhang, Jihao Wu, Yihua Teng, Minghui Liao, Nuo Xu, Xiao Xiao, et al.*</sub></sup> | [Paper](https://arxiv.org/abs/2403.02713)\|[Code](https://github.com/IMNearth/CoAT) |
| **[AndroidArena](https://github.com/AndroidArenaAgent/AndroidArena)** | KDD<br><sup>2024</sup> | Understanding the Weakness of Large Language Model Agents within a Complex Android Environment <br> <sup><sub>*Mingzhe Xing, Rongkai Zhang, Hui Xue, Qi Chen, Fan Yang, Zhen Xiao*</sub></sup> | [Paper](https://arxiv.org/abs/2402.06596)\|[Code](https://github.com/AndroidArenaAgent/AndroidArena) |
| **[LlamaTouch](https://github.com/LlamaTouch/LlamaTouch)** | UIST<br><sup>2024</sup> | LlamaTouch: A Faithful and Scalable Testbed for Mobile UI Task Automation <br> <sup><sub>*Li Zhang, Shihe Wang, Xianqing Jia, Zhihan Zheng, Yunhe Yan, Longxi Gao, et al.*</sub></sup> | [Paper](https://arxiv.org/abs/2404.16054)\|[Code](https://github.com/LlamaTouch/LlamaTouch) |
| **MobileAgentBench** | arXiv<br><sup>2024</sup> | MobileAgentBench: An Efficient and User-Friendly Benchmark for Mobile LLM Agents <br> <sup><sub>*Luyuan Wang, Yongyu Deng, Yiwei Zha, Guodong Mao, Qinmin Wang, Tianchen Min, et al.*</sub></sup> | [Paper](https://arxiv.org/abs/2406.08184)\|Code |
| **B-MoCA** | arXiv<br><sup>2024</sup> | Benchmarking Mobile Device Control Agents across Diverse Configurations <br> <sup><sub>*Juyong Lee, Taywon Min, Minyong An, Dongyoon Hahm, Haeone Lee, Changyeon Kim, et al.*</sub></sup> | [Paper](https://arxiv.org/abs/2404.16660)\|Code |
| **[AITW](https://github.com/google-research/google-research/tree/master/android_in_the_wild)** | NeurIPS<br><sup>2023</sup> | Android in the Wild: A Large-Scale Dataset for Android Device Control <br> <sup><sub>*Christopher Rawles, Alice Li, Daniel Rodriguez, Oriana Riva, Timothy Lillicrap*</sub></sup> | [Paper](https://arxiv.org/abs/2307.10088)\|[Code](https://github.com/google-research/google-research/tree/master/android_in_the_wild) |
| **[Mobile-Env](https://github.com/X-LANCE/Mobile-Env)** | arXiv<br><sup>2023</sup> | Mobile-Env: Building Qualified Evaluation Benchmarks for LLM-GUI Interaction <br> <sup><sub>*Danyang Zhang, Zhennan Shen, Rui Xie, Situo Zhang, Tianbao Xie, Zihan Zhao, et al.*</sub></sup> | [Paper](https://arxiv.org/abs/2305.08144)\|[Code](https://github.com/X-LANCE/Mobile-Env) |
| **[PixelHelp](https://github.com/google-research/google-research/tree/master/seq2act)** | ACL<br><sup>2020</sup> | Mapping Natural Language Instructions to Mobile UI Action Sequences <br> <sup><sub>*Yang Li, Jiacong He, Xin Zhou, Yuan Zhang, Jason Baldridge*</sub></sup> | [Paper](https://arxiv.org/abs/2005.03776)\|[Code](https://github.com/google-research/google-research/tree/master/seq2act) |


<h4 id="bench-desktop">- Desktop / OS</h4>

| **Name** | **Pub.** | **Title** | **Links** |
| :------: | :------: | :----------------------------------------------------------- | :------: |
| **[ScienceBoard](https://github.com/OS-Copilot/ScienceBoard)** | ICLR<br><sup>2026</sup> | ScienceBoard: Evaluating Multimodal Autonomous Agents in Realistic Scientific Workflows <br> <sup><sub>*Qiushi Sun, Zhoumianze Liu, Chang Ma, Zichen Ding, Fangzhi Xu, Zhangyue Yin, et al.*</sub></sup> | [Paper](https://arxiv.org/abs/2505.19897)\|[Code](https://github.com/OS-Copilot/ScienceBoard) |
| **[macOSWorld](https://github.com/showlab/macosworld)** | NeurIPS<br><sup>2025</sup> | macOSWorld: A Multilingual Interactive Benchmark for GUI Agents <br> <sup><sub>*Pei Yang, Hai Ci, Mike Zheng Shou*</sub></sup> | [Paper](https://arxiv.org/abs/2506.04135)\|[Code](https://github.com/showlab/macosworld) |
| **[TheAgentCompany](https://github.com/TheAgentCompany/TheAgentCompany)** | NeurIPS<br><sup>2025</sup> | TheAgentCompany: Benchmarking LLM Agents on Consequential Real World Tasks <br> <sup><sub>*Frank F. Xu, Yufan Song, Boxuan Li, Yuxuan Tang, Kritanjali Jain, Mengxue Bao, et al.*</sub></sup> | [Paper](https://arxiv.org/abs/2412.14161)\|[Code](https://github.com/TheAgentCompany/TheAgentCompany) |
| **[WindowsAgentArena](https://github.com/microsoft/WindowsAgentArena)** | ICML<br><sup>2025</sup> | Windows Agent Arena: Evaluating Multi-Modal OS Agents at Scale <br> <sup><sub>*Rogerio Bonatti, Dan Zhao, Francesco Bonacci, Dillon Dupont, Sara Abdali, Yinheng Li, et al.*</sub></sup> | [Paper](https://arxiv.org/abs/2409.08264)\|[Code](https://github.com/microsoft/WindowsAgentArena) |
| **OSUniverse** | arXiv<br><sup>2025</sup> | OSUniverse: Benchmark for Multimodal GUI-navigation AI Agents <br> <sup><sub>*Mariya Davydova, Daniel Jeffries, Patrick Barker, Arturo Márquez Flores, Sinéad Ryan*</sub></sup> | [Paper](https://arxiv.org/abs/2505.03570)\|Code |
| **WorldGUI** | arXiv<br><sup>2025</sup> | WorldGUI: An Interactive Benchmark for Desktop GUI Automation from Any Starting Point <br> <sup><sub>*Henry Hengyuan Zhao, Kaiming Yang, Wendi Yu, Difei Gao, Mike Zheng Shou*</sub></sup> | [Paper](https://arxiv.org/abs/2502.08047)\|Code |
| **[Spider2-V](https://github.com/xlang-ai/Spider2-V)** | NeurIPS<br><sup>2024</sup> | Spider2-V: How Far Are Multimodal Agents From Automating Data Science and Engineering Workflows? <br> <sup><sub>*Ruisheng Cao, Fangyu Lei, Haoyuan Wu, Jixuan Chen, Yeqiao Fu, Hongcheng Gao, et al.*</sub></sup> | [Paper](https://arxiv.org/abs/2407.10956)\|[Code](https://github.com/xlang-ai/Spider2-V) |
| **[VideoGUI](https://github.com/showlab/videogui)** | NeurIPS<br><sup>2024</sup> | VideoGUI: A Benchmark for GUI Automation from Instructional Videos <br> <sup><sub>*Kevin Qinghong Lin, Linjie Li, Difei Gao, Qinchen WU, Mingyi Yan, Zhengyuan Yang, et al.*</sub></sup> | [Paper](https://arxiv.org/abs/2406.10227)\|[Code](https://github.com/showlab/videogui) |
| **[OSWorld](https://github.com/xlang-ai/OSWorld)** | NeurIPS<br><sup>2024</sup> | OSWorld: Benchmarking Multimodal Agents for Open-Ended Tasks in Real Computer Environments <br> <sup><sub>*Tianbao Xie, Danyang Zhang, Jixuan Chen, Xiaochuan Li, Siheng Zhao, Ruisheng Cao, et al.*</sub></sup> | [Paper](https://arxiv.org/abs/2404.07972)\|[Code](https://github.com/xlang-ai/OSWorld) |
| **[AssistGUI](https://github.com/showlab/assistgui)** | CVPR<br><sup>2024</sup> | ASSISTGUI: Task-Oriented Desktop Graphical User Interface Automation <br> <sup><sub>*Difei Gao, Lei Ji, Zechen Bai, Mingyu Ouyang, Peiran Li, Dongxing Mao, et al.*</sub></sup> | [Paper](https://arxiv.org/abs/2312.13108)\|[Code](https://github.com/showlab/assistgui) |
| **OmniACT** | ECCV<br><sup>2024</sup> | OmniACT: A Dataset and Benchmark for Enabling Multimodal Generalist Autonomous Agents for Desktop and Web <br> <sup><sub>*Raghav Kapoor, Yash Parag Butala, Melisa Russak, Jing Yu Koh, Kiran Kamble, Waseem Alshikh, et al.*</sub></sup> | [Paper](https://arxiv.org/abs/2402.17553)\|Code |
| **[OfficeBench](https://github.com/zlwang-cs/OfficeBench)** | arXiv<br><sup>2024</sup> | OfficeBench: Benchmarking Language Agents across Multiple Applications for Office Automation <br> <sup><sub>*Zilong Wang, Yuedong Cui, Li Zhong, Zimin Zhang, Da Yin, Bill Yuchen Lin, et al.*</sub></sup> | [Paper](https://arxiv.org/abs/2407.19056)\|[Code](https://github.com/zlwang-cs/OfficeBench) |


<h4 id="bench-cross">- Cross-platform</h4>

| **Name** | **Pub.** | **Title** | **Links** |
| :------: | :------: | :----------------------------------------------------------- | :------: |
| **[VisualAgentBench](https://github.com/THUDM/VisualAgentBench)** | ICLR<br><sup>2025</sup> | VisualAgentBench: Towards Large Multimodal Models as Visual Foundation Agents <br> <sup><sub>*Xiao Liu, Tianjie Zhang, Yu Gu, Iat Long Iong, Yifan Xu, Xixuan Song, et al.*</sub></sup> | [Paper](https://arxiv.org/abs/2408.06327)\|[Code](https://github.com/THUDM/VisualAgentBench) |
| **[GUI-World](https://github.com/Dongping-Chen/GUI-World)** | ICLR<br><sup>2025</sup> | GUI-World: A Video Benchmark and Dataset for Multimodal GUI-oriented Understanding <br> <sup><sub>*Dongping Chen, Yue Huang, Siyuan Wu, Jingyu Tang, Liuyi Chen, Yilin Bai, et al.*</sub></sup> | [Paper](https://arxiv.org/abs/2406.10819)\|[Code](https://github.com/Dongping-Chen/GUI-World) |
| **[AgentStudio](https://github.com/SkyworkAI/agent-studio)** | ICLR<br><sup>2025</sup> | AgentStudio: A Toolkit for Building General Virtual Agents <br> <sup><sub>*Longtao Zheng, Zhiyuan Huang, Zhenghai Xue, Xinrun Wang, Bo An, Shuicheng Yan*</sub></sup> | [Paper](https://arxiv.org/abs/2403.17918)\|[Code](https://github.com/SkyworkAI/agent-studio) |
| **[CRAB](https://github.com/camel-ai/crab)** | ACL Findings<br><sup>2025</sup> | CRAB: Cross-environment Agent Benchmark for Multimodal Language Model Agents <br> <sup><sub>*Tianqi Xu, Linyao Chen, Dai-Jie Wu, Yanjun Chen, Zecheng Zhang, Xiang Yao, et al.*</sub></sup> | [Paper](https://arxiv.org/abs/2407.01511)\|[Code](https://github.com/camel-ai/crab) |


<h4 id="bench-grounding">- GUI Grounding & Understanding</h4>

> ScreenSpot, ScreenSpot-v2 and OSWorld-G are introduced together with SeeClick, OS-Atlas and Jedi respectively (see [GUI Grounding](#gui-grounding)).

| **Name** | **Pub.** | **Title** | **Links** |
| :------: | :------: | :----------------------------------------------------------- | :------: |
| **UI-Vision** | ICML<br><sup>2025</sup> | UI-Vision: A Desktop-centric GUI Benchmark for Visual Perception and Interaction <br> <sup><sub>*Shravan Nayak, Xiangru Jian, Kevin Qinghong Lin, Juan A. Rodriguez, Montek Kalsi, Rabiul Awal, et al.*</sub></sup> | [Paper](https://arxiv.org/abs/2503.15661)\|Code |
| **[ScreenSpot-Pro](https://github.com/likaixin2000/ScreenSpot-Pro-GUI-Grounding)** | ACM MM<br><sup>2025</sup> | ScreenSpot-Pro: GUI Grounding for Professional High-Resolution Computer Use <br> <sup><sub>*Kaixin Li, Ziyang Meng, Hongzhan Lin, Ziyang Luo, Yuchen Tian, Jing Ma, et al.*</sub></sup> | [Paper](https://arxiv.org/abs/2504.07981)\|[Code](https://github.com/likaixin2000/ScreenSpot-Pro-GUI-Grounding) |
| **[MMBench-GUI](https://github.com/open-compass/MMBench-GUI)** | arXiv<br><sup>2025</sup> | MMBench-GUI: Hierarchical Multi-Platform Evaluation Framework for GUI Agents <br> <sup><sub>*Xuehui Wang, Zhenyu Wu, JingJing Xie, Zichen Ding, Bowen Yang, Zehao Li, et al.*</sub></sup> | [Paper](https://arxiv.org/abs/2507.19478)\|[Code](https://github.com/open-compass/MMBench-GUI) |
| **WebUI** | CHI<br><sup>2023</sup> | WebUI: A Dataset for Enhancing Visual UI Understanding with Web Semantics <br> <sup><sub>*Jason Wu, Siyan Wang, Siman Shen, Yi-Hao Peng, Jeffrey Nichols, Jeffrey P. Bigham*</sub></sup> | [Paper](https://arxiv.org/abs/2301.13280)\|Code |
| **MoTIF** | ECCV<br><sup>2022</sup> | A Dataset for Interactive Vision-Language Navigation with Unknown Command Feasibility <br> <sup><sub>*Andrea Burns, Deniz Arsan, Sanjna Agrawal, Ranjitha Kumar, Kate Saenko, Bryan A. Plummer*</sub></sup> | [Paper](https://arxiv.org/abs/2202.02312)\|Code |
| **ScreenQA** | arXiv<br><sup>2022</sup> | ScreenQA: Large-Scale Question-Answer Pairs over Mobile App Screenshots <br> <sup><sub>*Yu-Chung Hsiao, Fedir Zubach, Gilles Baechler, Srinivas Sunkara, Victor Carbune, Jason Lin, et al.*</sub></sup> | [Paper](https://arxiv.org/abs/2209.08199)\|Code |
| **Screen2Words** | UIST<br><sup>2021</sup> | Screen2Words: Automatic Mobile UI Summarization with Multimodal Learning <br> <sup><sub>*Bryan Wang, Gang Li, Xin Zhou, Zhourong Chen, Tovi Grossman, Yang Li*</sub></sup> | [Paper](https://arxiv.org/abs/2108.03353)\|Code |
| **Widget Captioning** | EMNLP<br><sup>2020</sup> | Widget Captioning: Generating Natural Language Description for Mobile User Interface Elements <br> <sup><sub>*Yang Li, Gang Li, Luheng He, Jingjie Zheng, Hong Li, Zhiwei Guan*</sub></sup> | [Paper](https://arxiv.org/abs/2010.04295)\|Code |


</details>


--------------------------------------------------------------------------------------


<h2 id="projects">🛠️ Open-source Projects</h2>

| **Project** | **Description** |
| :------ | :------ |
| [browser-use](https://github.com/browser-use/browser-use) ![GitHub stars](https://img.shields.io/github/stars/browser-use/browser-use?style=social) | Make websites accessible for AI agents; LLM-driven browser automation |
| [UI-TARS-desktop](https://github.com/bytedance/UI-TARS-desktop) ![GitHub stars](https://img.shields.io/github/stars/bytedance/UI-TARS-desktop?style=social) | Desktop app & Agent TARS stack built on UI-TARS models |
| [Agent S](https://github.com/simular-ai/Agent-S) ![GitHub stars](https://img.shields.io/github/stars/simular-ai/Agent-S?style=social) | Open agentic framework for computer use (Agent S / S2 / S3) |
| [UFO](https://github.com/microsoft/UFO) ![GitHub stars](https://img.shields.io/github/stars/microsoft/UFO?style=social) | Microsoft's UI-focused agent / Desktop AgentOS for Windows |
| [Mobile-Agent](https://github.com/X-PLUG/MobileAgent) ![GitHub stars](https://img.shields.io/github/stars/X-PLUG/MobileAgent?style=social) | Mobile-Agent family (v1/v2/v3, -E, PC-Agent, GUI-Owl) |
| [OmniParser](https://github.com/microsoft/OmniParser) ![GitHub stars](https://img.shields.io/github/stars/microsoft/OmniParser?style=social) | Screen parsing tool for pure-vision GUI agents (OmniTool included) |
| [Cua](https://github.com/trycua/cua) ![GitHub stars](https://img.shields.io/github/stars/trycua/cua?style=social) | Open-source infrastructure (sandboxes, SDKs) for computer-use agents |
| [Open Interpreter](https://github.com/OpenInterpreter/open-interpreter) ![GitHub stars](https://img.shields.io/github/stars/OpenInterpreter/open-interpreter?style=social) | Natural-language interface for computers |
| [Self-Operating Computer](https://github.com/OthersideAI/self-operating-computer) ![GitHub stars](https://img.shields.io/github/stars/OthersideAI/self-operating-computer?style=social) | Framework that lets multimodal models operate a computer |
| [Midscene.js](https://github.com/web-infra-dev/midscene) ![GitHub stars](https://img.shields.io/github/stars/web-infra-dev/midscene?style=social) | Vision-driven UI automation for Web, Android and more |
| [Skyvern](https://github.com/Skyvern-AI/skyvern) ![GitHub stars](https://img.shields.io/github/stars/Skyvern-AI/skyvern?style=social) | Browser workflow automation with LLMs and computer vision |
| [Stagehand](https://github.com/browserbase/stagehand) ![GitHub stars](https://img.shields.io/github/stars/browserbase/stagehand?style=social) | AI browser automation framework |
| [Playwright MCP](https://github.com/microsoft/playwright-mcp) ![GitHub stars](https://img.shields.io/github/stars/microsoft/playwright-mcp?style=social) | MCP server that exposes browser automation to LLMs |
| [Computer Use OOTB](https://github.com/showlab/computer_use_ootb) ![GitHub stars](https://img.shields.io/github/stars/showlab/computer_use_ootb?style=social) | Out-of-the-box GUI agent for Windows & macOS |
| [OSWorld](https://github.com/xlang-ai/OSWorld) ![GitHub stars](https://img.shields.io/github/stars/xlang-ai/OSWorld?style=social) | Real-computer benchmark & environment for multimodal agents |
| [AndroidWorld](https://github.com/google-research/android_world) ![GitHub stars](https://img.shields.io/github/stars/google-research/android_world?style=social) | Dynamic Android benchmarking environment |
| [BrowserGym](https://github.com/ServiceNow/BrowserGym) ![GitHub stars](https://img.shields.io/github/stars/ServiceNow/BrowserGym?style=social) | Gym environment unifying web agent benchmarks |


<h2 id="products">🏢 Commercial Systems</h2>

| **Organization** | **System** |
| :------ | :------ |
| Anthropic | [Claude Computer Use](https://www.anthropic.com/news/3-5-models-and-computer-use) |
| OpenAI | [Computer-Using Agent (Operator)](https://openai.com/index/computer-using-agent/) |
| Google DeepMind | [Gemini 2.5 Computer Use](https://blog.google/technology/google-deepmind/gemini-computer-use-model/) |
| Google DeepMind | [Project Mariner](https://deepmind.google/models/project-mariner/) |


--------------------------------------------------------------------------------------


<h2 id="reference">📎 Related Awesome Lists</h2>

- [GUI Agents Paper List (OSU NLP)](https://github.com/OSU-NLP-Group/GUI-Agents-Paper-List)
- [Awesome GUI Agent (Show Lab)](https://github.com/showlab/Awesome-GUI-Agent)
- [Awesome Computer Use (ACU)](https://github.com/francedot/acu)
- [LLM-Brained GUI Agents Survey](https://github.com/vyokky/LLM-Brained-GUI-Agents-Survey)
- [OS Agents Survey](https://github.com/OS-Agent-Survey/OS-Agent-Survey)
- [Awesome GUI Agent Security](https://github.com/Yuxuan2003/Awesome-GUI-Agent-Security)
- [Awesome Backdoor in Agent](https://github.com/Robin-WZQ/Awesome-Backdoor-in-Agent)
- [Awesome Backdoor on LMMs](https://github.com/Robin-WZQ/Awesome-Backdoor-on-LMMs)


<h2>🤝 Contributing</h2>

Contributions are welcome! Please read [CONTRIBUTING.md](CONTRIBUTING.md) for the entry format, then open a pull request or an issue.


<h2>⭐ Star History</h2>

[![Star History Chart](https://api.star-history.com/svg?repos=farewellIamLoser/awesome-gui-agent&type=date&legend=top-left)](https://www.star-history.com/#farewellIamLoser/awesome-gui-agent&type=date&legend=top-left)
