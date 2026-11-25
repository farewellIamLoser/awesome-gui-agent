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
    <img src="https://img.shields.io/badge/papers-163-blue?style=flat" alt="Papers">
  </p>
</div>

> A curated, regularly updated list of papers, code and benchmarks on **GUI agents**: (multimodal) LLM-based agents that perceive screens and operate **web, mobile and desktop** interfaces like humans do. It covers
> - Native GUI agent models and GUI grounding
> - Agent frameworks (prompting, multi-agent, memory) for Web / Mobile / Desktop
> - Reinforcement learning, data synthesis and world models for GUI agents
> - Benchmarks, datasets, and safety & security of computer-use agents
>
> 📌 An inline tag after a title, e.g. `Mobile`, marks the main platform. A grey badge, e.g. <sub>![ScreenSpot](https://img.shields.io/badge/ScreenSpot-grey)</sub>, names the dataset/benchmark that paper introduces. A plain **Code** without a link means the code has not been released (or we have not found it).
>
> 🔄 Updated regularly. Missing a paper? Open an issue or PR (see [CONTRIBUTING.md](CONTRIBUTING.md)).


<details>
<summary><strong>:loudspeaker: Latest Updates</strong></summary>

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


<h2>🤝 Contributing</h2>

Contributions are welcome! Please read [CONTRIBUTING.md](CONTRIBUTING.md) for the entry format, then open a pull request or an issue.


<h2>⭐ Star History</h2>

[![Star History Chart](https://api.star-history.com/svg?repos=farewellIamLoser/awesome-gui-agent&type=date&legend=top-left)](https://www.star-history.com/#farewellIamLoser/awesome-gui-agent&type=date&legend=top-left)
