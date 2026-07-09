<h1 align="center">
Awesome-ID-Customization 
</h1>
<p align="center">
<font face="黑体" color=orange size=5"> An Awesome Collection for ID Customization  </font>
</p>
<p align="center">
<font face="黑体" color=orange size=5"> 收集和梳理人物自定义相关 </font>
</p>
<p align="center">
  <a href="https://github.com/leeguandong/Awesome-ID-Customization/stargazers"> <img src="https://img.shields.io/github/stars/leeguandong/Awesome-ID-Customization.svg?style=popout-square" alt="GitHub stars"></a>
  <a href="https://github.com/leeguandong/Awesome-ID-Customization/issues"> <img src="https://img.shields.io/github/issues/leeguandong/Awesome-ID-Customization.svg?style=popout-square" alt="GitHub issues"></a>
  <a href="https://github.com/leeguandong/Awesome-ID-Customization/forks"> <img src="https://img.shields.io/github/forks/leeguandong/Awesome-ID-Customization.svg?style=popout-square" alt="GitHub forks"></a>
</p>



本项目旨在收集和梳理人物自定义相关的开源模型、应用、数据集及教程等资料，人物自定义主要指的是人物一致性生成，一致性与可编辑性之间的均衡优化，当前基于flux版本的人物一致性方法很少！

如果本项目能给您带来一点点帮助，麻烦点个⭐️吧～

同时也欢迎大家贡献本项目未收录的开源模型、应用、数据集等。提供新的仓库信息请发起PR，并按照本项目的格式提供仓库链接、star数，简介等相关信息，感谢~


## 目录
- [目录](#目录)
  
  - [1. 人物自定义模型](#1-人物自定义模型)
    
    - [1.1 方法全景表](#11-方法全景表)
    - [1.2 基于DiT架构](#12-flux模型)
    - [1.3 基于unet架构](#13-unet模型)
  - [2. 测评](#2-测评)
  - [3. 数据集](#3-数据集)
  
- [Star History](#star-history)

###  1. <a name='模型'></a>人物自定义模型

#### 1.1 方法全景表

| 方法 | 年份 | 基座/架构 | 任务范式 | ID/主体能力 | 链接 |
|------|------|-----------|----------|-------------|------|
| **EditID** | 2025 | Flux / DiT | Training-free editable ID customization | 单人 ID，可编辑性 | [GitHub](https://github.com/leeguandong/IBench) |
| **EditIDv2** | 2025 | Flux / DiT | Data-lubricated ID feature integration | 单人 ID，长文本编辑 | [GitHub](https://github.com/typemovie/EditIDv2) |
| **PuLID** | 2024 | SD / Flux | Contrastive ID alignment | 单人 ID，轻量快速 | [GitHub](https://github.com/ToTheBeginning/PuLID) |
| **FLUX-customID** | 2024 | Flux | ID adapter / customization | 单人 ID，真实感定制 | [GitHub](https://github.com/damo-cv/FLUX-customID) |
| **ConsisID** | 2024 | Video DiT | Frequency decomposition for T2V | 单人 ID 视频 | [GitHub](https://github.com/PKU-YuanGroup/ConsisID) |
| **InfiniteYou** | 2025 | Flux / DiT | Flexible photo recrafting | 单人 ID，照片重绘 | [GitHub](https://github.com/bytedance/InfiniteYou) |
| **UNO** | 2025 | DiT | In-context subject generation | 单/多主体，少样本上下文 | [GitHub](https://github.com/bytedance/UNO) |
| **ACE++** | 2025 | DiT | Instruction image creation/editing | 上下文填充，主体/风格编辑 | [GitHub](https://github.com/ali-vilab/ACE_plus) |
| **Personalize Anything** | 2025 | DiT | Free personalization | 通用主体定制 | [GitHub](https://github.com/fenghora/personalize-anything) |
| **Diptych** | 2025 | Flux / Inpainting | Zero-shot subject-driven generation | 任意主体，inpainting 条件 | [GitHub](https://github.com/wuyou22s/Diptych) |
| **DynamicID** | 2025 | DiT | Zero-shot multi-ID personalization | 多 ID，脸部可编辑 | [arXiv](https://arxiv.org/abs/2503.06505) |
| **InstantCharacter** | 2025 | DiT | Scalable character personalization | 角色一致性 | [GitHub](https://github.com/Tencent/InstantCharacter) |
| **RealCustom++** | 2025 | DiT | Real-word representation | 实时主体定制 | [GitHub](https://github.com/bytedance/RealCustom) |
| **DreamO** | 2025 | DiT | Unified image customization | 通用图像定制 | [GitHub](https://github.com/bytedance/DreamO) |
| **FlexIP** | 2025 | DiT | Preservation / personality control | 保真度与个性化可控 | [arXiv](https://arxiv.org/abs/2504.07405) |
| **XVerse** | 2025 | DiT | DiT modulation | 多主体 ID + 语义属性控制 | [GitHub](https://github.com/bytedance/XVerse) |
| **UMO** | 2025 | DiT / RL | Matching reward optimization | 多 ID 一致性与防混淆 | [GitHub](https://github.com/bytedance/UMO) |
| **FaceCLIP** | 2025 | DiT | Joint ID-textual representation | ID-文本联合表征 | [GitHub](https://github.com/bytedance/FaceCLIP) |
| **USO** | 2025 | DiT | Style / subject disentanglement | 风格 + 主体统一生成 | [GitHub](https://github.com/bytedance/USO) |
| **IC-Custom** | 2025 | DiT | In-context image customization | 上下文主体定制 | [GitHub](https://github.com/TencentARC/IC-Custom) |
| **WithAnyone** | 2025 | DiT | Controllable ID-consistent generation | 人物 ID 可控生成 | [GitHub](https://github.com/Doby-Xu/WithAnyone) |
| **MagicMirror** | 2025 | Video DiT | ID-preserved video generation | 单人 ID 视频 | [GitHub](https://github.com/JIA-Lab-research/MagicMirror) |
| **ExpPortrait** | 2026 | DiT | Expressive portrait generation | 表情化肖像定制 | [arXiv](https://arxiv.org/abs/2602.19900) |
| **AnyPhoto** | 2026 | DiT | Location-canvas ID modulation | 多人 ID，位置绑定 | [arXiv](https://arxiv.org/abs/2603.14770) |
| **PositionIC** | 2025 | DiT | Position + identity consistency | 位置控制 + ID 一致 | [GitHub](https://github.com/MeiGen-AI/PositionIC) |
| **MultiCrafter** | 2025 | DiT | Disentangled attention + preference alignment | 多主体高保真生成 | [arXiv](https://arxiv.org/abs/2509.21953) |
| **LatentUnfold** | 2025 | Flux / DiT | Training-free subject activation | 无训练主体驱动生成 | [GitHub](https://github.com/bytedance/LatentUnfold) |
| **Scone** | 2026 | Unified model | Composition + distinction modeling | 多主体组合与目标主体区分 | [GitHub](https://github.com/Ryann-Ran/Scone) |
| **MagicView** | 2025 | DiT | Priors-guided in-context learning | 单图到多视角 ID 一致 | [arXiv](https://arxiv.org/abs/2511.00293) |
| **Proteus-ID** | 2025 | Video DiT | ID-consistent video customization | 单人 ID，运动一致视频 | [GitHub](https://github.com/grenoble-zhang/Proteus-ID) |
| **DivRL** | 2026 | Post-training / RL | Identity-diversity reward optimization | 主体一致性 + 多样性 | [GitHub](https://github.com/QianWangX/DivRL) |
| **PortraitBooth** | 2023 | UNet | Fast portrait personalization | 单人肖像定制 | [Project](https://portraitbooth.github.io/) |
| **DreamIdentity** | 2023 | UNet | Face-identity preserved generation | 单人 ID，编辑性增强 | [arXiv](https://arxiv.org/abs/2307.00300) |
| **ConsistentID** | 2024 | UNet | Multimodal fine-grained ID preserving | 单人肖像生成 | [GitHub](https://github.com/JackAILab/ConsistentID) |
| **PhotoMaker** | 2024 | UNet / SDXL | Stacked ID embedding | 单人/多人照片定制 | [GitHub](https://github.com/TencentARC/PhotoMaker) |
| **IDAdapter** | 2024 | UNet | Mixed feature adapter | Tuning-free 个性化 | [arXiv](https://arxiv.org/abs/2403.13535) |
| **InstantID** | 2024 | UNet / SDXL | Plug-and-play IdentityNet | 单图零样本 ID 保持 | [GitHub](https://github.com/instantX-research/InstantID) |
| **Character-Adapter** | 2024 | UNet | Region-controlled character adapter | 角色区域控制 | [GitHub](https://github.com/Character-Adapter/Character-Adapter) |
| **Face Adapter** | 2024 | UNet | Fine-grained ID / attribute adapter | ID + 属性控制 | [GitHub](https://github.com/FaceAdapter/Face-Adapter) |
| **FastComposer** | 2023 | UNet | Localized attention | 多主体免训练生成 | [GitHub](https://github.com/open-mmlab/mmagic/tree/main/configs/fastcomposer) |
| **IC-Portrait** | 2025 | UNet | In-context portrait matching | 视角一致肖像生成 | [arXiv](https://arxiv.org/abs/2501.17159) |
| **MasterWeaver** | 2024 | UNet | Editability / identity balancing | 人物个性化编辑 | [GitHub](https://github.com/csyxwei/MasterWeaver) |
| **PhotoVerse** | 2023 | UNet | Tuning-free image customization | 图像主体定制 | [GitHub](https://github.com/idonahum/photoVerse) |
| **UniPortrait** | 2024 | UNet | Unified single / multi-human personalization | 单人/多人 ID | [GitHub](https://github.com/junjiehe96/UniPortrait) |
| **RealisID** | 2024 | UNet | Local-global complementation | 小脸/位置/姿态可控 | [arXiv](https://arxiv.org/abs/2412.16832) |
| **FlashFace** | 2024 | UNet | High-fidelity human personalization | 高保真人脸定制 | [GitHub](https://github.com/ali-vilab/FlashFace) |
| **CrossFaceID** | 2024 | UNet | Cross-training data | FaceID customization | [GitHub](https://github.com/ShuheSH/CrossFaceID) |
| **DreamID** | 2024 | UNet | Triplet ID group learning | 快速高保真人脸交换 | [GitHub](https://github.com/superhero-7/DreamID) |
| **ID-Booth** | 2023 | UNet | Identity-consistent face generation | 单人脸生成 | [GitHub](https://github.com/dariant/ID-Booth) |
| **FaceSnap** | 2026 | UNet | ID-fidelity network | Tuning-free portrait customization | [arXiv](https://arxiv.org/abs/2602.00627) |
| **Diff-PC** | 2026 | UNet | 3D-aware controllable diffusion | 零样本肖像定制 | [arXiv](https://arxiv.org/abs/2602.00639) |
| **UniID** | 2025 | UNet | Training for identity, inference for control | 免调参人脸个性化 | [GitHub](https://github.com/lyuPang/UniID) |

> 备注：年份按论文或项目公开时间粗略标注，详细信息以下方条目与原论文/仓库为准。

#### 1.2 Flux模型

* **EditID: Training-Free Editable ID Customization for Text-to-Image Generation**
  
  * 地址：https://github.com/leeguandong/IBench ![](https://img.shields.io/github/stars/leeguandong/IBench.svg)
  * 架构图：
  
   ![image](pic/editid.png)

* **EditIDv2: Editable ID Customization with Data-Lubricated ID Feature Integration for Text-to-Image Generation**
  
  * 地址：https://github.com/typemovie/EditIDv2 ![](https://img.shields.io/github/stars/typemovie/EditIDv2.svg)
  * 架构图：
  
  ![image](pic/editidv2.png)

* **PuLID: Pure and Lightning ID Customization via Contrastive Alignment**
  
  * 地址：https://github.com/ToTheBeginning/PuLID ![](https://img.shields.io/github/stars/ToTheBeginning/PuLID.svg)  
  * 架构图：
  
   ![image](pic/pulid.png)
  
* **FLUX-customID: Realistically Customize Your Personal ID to Perfection**
  
  * 地址：https://github.com/damo-cv/FLUX-customID ![](https://img.shields.io/github/stars/damo-cv/FLUX-customID.svg)    
  * [comfyui](https://github.com/leeguandong/ComfyUI_FluxCustomId)：
  
   ![image](pic/flux-customid.png)
  
* **Identity-Preserving Text-to-Video Generation by Frequency Decomposition**
  
  * 地址：https://github.com/PKU-YuanGroup/ConsisID ![](https://img.shields.io/github/stars/PKU-YuanGroup/ConsisID.svg)
  * 架构图：
  
  ![image](pic/consistid.png)

* **InfiniteYou: Flexible Photo Recrafting While Preserving Your Identity**
  
  * 地址：https://github.com/bytedance/InfiniteYou ![](https://img.shields.io/github/stars/bytedance/InfiniteYou.svg)
  * 架构图：
  
  ![image](pic/infunet.png)

* **Less-to-More Generalization: Unlocking More Controllability by In-Context Generation**
  
  * 地址：https://github.com/bytedance/UNO ![](https://img.shields.io/github/stars/bytedance/UNO.svg)
  * 架构图：
  
  ![image](pic/uno.png)

* **ACE++: Instruction-Based Image Creation and Editing via Context-Aware Content Filling**
  
  * 地址：https://github.com/ali-vilab/ACE_plus ![](https://img.shields.io/github/stars/ali-vilab/ACE_plus.svg)
  * 架构图：
  
  ![image](pic/ace++.png)

* **Personalize Anything for Free with Diffusion Transformer**
  
  * 地址：https://github.com/fenghora/personalize-anything ![](https://img.shields.io/github/stars/fenghora/personalize-anything.svg)
  * 架构图：
  
  ![image](pic/personalize_anything.png)

* **Large-Scale Text-to-Image Model with Inpainting is a Zero-Shot Subject-Driven Image Generator**
  
  * 地址：https://github.com/wuyou22s/Diptych ![](https://img.shields.io/github/stars/wuyou22s/Diptych.svg)
  * 架构图：
  
  ![image](pic/diptych.png)

* **DynamicID: Zero-Shot Multi-ID Image Personalization with Flexible Facial Editability**
  
  * 地址：https://arxiv.org/abs/2503.06505
  * 架构图：
  
  ![image](pic/dynamicid.png)

* **InstantCharacter: Personalize Any Characters with a Scalable Diffusion Transformer Framework**
  
  * 地址：https://github.com/Tencent/InstantCharacter ![](https://img.shields.io/github/stars/Tencent/InstantCharacter.svg)
  * 架构图：
  
  ![image](pic/instantcharacter.png)

* **RealCustom++: Representing Images as Real Text Word for Real-Time Customization**
  
  * 地址：https://github.com/bytedance/RealCustom ![](https://img.shields.io/github/stars/bytedance/RealCustom.svg)
  * 架构图：
  
  ![image](pic/realcustom++.jpg)

* **DreamO: A Unified Framework for Image Customization**
  
  * 地址：https://github.com/bytedance/DreamO ![](https://img.shields.io/github/stars/bytedance/DreamO.svg)
  * 架构图：
  
  ![image](pic/dreamo.png)

* **FlexIP: Dynamic Control of Preservation and Personality for Customized Image Generation**
  
  * 地址：https://arxiv.org/abs/2504.07405
  * 架构图：
  
  ![image](pic/flexip.jpg)

* **XVerse: Consistent Multi-Subject Control of Identity and Semantic Attributes via DiT Modulation**
  
  * 地址：https://github.com/bytedance/XVerse ![](https://img.shields.io/github/stars/bytedance/XVerse.svg)
  * 架构图：
  
  ![image](pic/xverse.png)

* **UMO: Scaling Multi-Identity Consistency for Image Customization via Matching Reward**
  
  * 地址：https://github.com/bytedance/UMO ![](https://img.shields.io/github/stars/bytedance/UMO.svg)
  * 架构图：
  
  ![image](pic/umo.png)

* **Learning Joint ID-Textual Representation for ID-Preserving Image Synthesis**
  
  * 地址：https://github.com/bytedance/FaceCLIP ![](https://img.shields.io/github/stars/bytedance/FaceCLIP.svg)
  * 架构图：
  
  ![image](pic/faceclip.jpeg)

* **USO: Unified Style and Subject-Driven Generation via Disentangled and Reward Learning**

  * 地址：https://github.com/bytedance/USO ![](https://img.shields.io/github/stars/bytedance/USO.svg)
  * 架构图：

  ![image](pic/uso.png)

* **IC-Custom: Diverse Image Customization via In-Context Learning**

  * 地址：https://github.com/TencentARC/IC-Custom ![](https://img.shields.io/github/stars/TencentARC/IC-Custom.svg)
  * 架构图：

  ![image](pic/ic-custom.png)

* **WithAnyone: Towards Controllable and ID Consistent Image Generation**

  * 地址：https://github.com/Doby-Xu/WithAnyone ![](https://img.shields.io/github/stars/Doby-Xu/WithAnyone.svg)
  * 架构图：

  ![image](pic/withanyone.png)

* **MagicMirror: ID-Preserved Video Generation in Video Diffusion Transformers**

  * 地址：https://github.com/JIA-Lab-research/MagicMirror ![](https://img.shields.io/github/stars/JIA-Lab-research/MagicMirror.svg)
  * 架构图：

  ![image](pic/magicmirror.png)

* **ExpPortrait: Expressive Portrait Generation via Personalized Representation**

  * 地址：https://arxiv.org/abs/2602.19900
  * 架构图：

  ![image](pic/expportrait.jpg)

* **AnyPhoto: Multi-Person Identity Preserving Image Generation with ID Adaptive Modulation on Location Canvas**

  * 地址：https://arxiv.org/abs/2603.14770
  * 架构图：

  ![image](pic/anyphoto.png)

* **PositionIC: Unified Position and Identity Consistency for Image Customization**

  * 地址：https://github.com/MeiGen-AI/PositionIC ![](https://img.shields.io/github/stars/MeiGen-AI/PositionIC.svg)
  * 架构图：

  ![image](pic/positionic.png)

* **MultiCrafter: High-Fidelity Multi-Subject Generation via Disentangled Attention and Identity-Aware Preference Alignment**

  * 地址：https://arxiv.org/abs/2509.21953
  * 架构图：

  ![image](pic/multicrafter.png)

* **Flux Already Knows: Activating Subject-Driven Image Generation without Training**

  * 地址：https://github.com/bytedance/LatentUnfold ![](https://img.shields.io/github/stars/bytedance/LatentUnfold.svg)
  * 架构图：

  ![image](pic/latentunfold.png)

* **Scone: Bridging Composition and Distinction in Subject-Driven Image Generation via Unified Understanding-Generation Modeling**

  * 地址：https://github.com/Ryann-Ran/Scone ![](https://img.shields.io/github/stars/Ryann-Ran/Scone.svg)
  * 架构图：

  ![image](pic/scone.png)

* **MagicView: Multi-View Consistent Identity Customization via Priors-Guided In-Context Learning**

  * 地址：https://arxiv.org/abs/2511.00293
  * 架构图：

  ![image](pic/magicview.png)

* **Proteus-ID: ID-Consistent and Motion-Coherent Video Customization**

  * 地址：https://github.com/grenoble-zhang/Proteus-ID ![](https://img.shields.io/github/stars/grenoble-zhang/Proteus-ID.svg)
  * 架构图：

  ![image](pic/proteus-id.jpg)

* **DivRL: Disentangled Self-Similarity Rewards for Diverse Subject-Driven Generation**

  * 地址：https://github.com/QianWangX/DivRL ![](https://img.shields.io/github/stars/QianWangX/DivRL.svg)
  * 架构图：

  ![image](pic/divrl.png)


#### 1.3 Unet模型

* **PortraitBooth: A Versatile Portrait Model for Fast Identity-preserved Personalization**
  
  * 地址：https://portraitbooth.github.io/
  * 架构图：
  
  ![image](pic/portraitBooth.png)
  
* **DreamIdentity: Improved Editability for Efficient Face-identity Preserved Image Generation**
  
  * 地址：https://arxiv.org/abs/2307.00300
  * 架构图：
  
  ![image](pic/dreamidentity.png)
  
* **ConsistentID : Portrait Generation with Multimodal Fine-Grained Identity Preserving**
  
  * 地址：https://github.com/JackAILab/ConsistentID ![](https://img.shields.io/github/stars/JackAILab/ConsistentID.svg)  
  * 架构图：
  
  ![image](pic/consistantid.png)
  
* **PhotoMaker: Customizing Realistic Human Photos via Stacked ID Embedding**

  * 地址：https://github.com/TencentARC/PhotoMaker ![](https://img.shields.io/github/stars/TencentARC/PhotoMaker.svg)
  * 架构图：

  ![image](pic/photomaker.png)

* **IDAdapter: Learning Mixed Features for Tuning-Free Personalization of Text-to-Image Models**

  * 地址：https://arxiv.org/abs/2403.13535
  * 架构图：

  ![image](pic/idadapter.png)

* **InstantID: Zero-shot Identity-Preserving Generation in Seconds**

  * 地址：https://github.com/instantX-research/InstantID ![](https://img.shields.io/github/stars/instantX-research/InstantID.svg)
  * 架构图：

  ![image](pic/instantid.png)
  
* **Character-Adapter: Prompt-Guided Region Control for High-Fidelity Character Customization**

  * 地址：https://github.com/Character-Adapter/Character-Adapter ![](https://img.shields.io/github/stars/Character-Adapter/Character-Adapter.svg)
  * 架构图：

  ![image](pic/character-adapter.png)

* **Face Adapter for Pre-Trained Diffusion Models with Fine-Grained ID and Attribute Control**

  * 地址：https://github.com/FaceAdapter/Face-Adapter ![](https://img.shields.io/github/stars/FaceAdapter/Face-Adapter.svg)
  * 架构图：

  ![image](pic/faceadapter.png)

* **FastComposer: Tuning-Free Multi-Subject Image Generation with Localized Attention**

  * 地址：https://github.com/open-mmlab/mmagic/tree/main/configs/fastcomposer ![](https://img.shields.io/github/stars/open-mmlab/mmagic.svg)
  * 架构图：

  ![image](pic/fastcomposer.png)

* **IC-Portrait: In-Context Matching for View-Consistent Personalized Portrait Generation**

  * 地址：https://arxiv.org/abs/2501.17159
  * 架构图：

  ![image](pic/ic-portrait.png)

* **MasterWeaver: Taming Editability and Identity for Personalized Text-to-Image Generation**

  * 地址：https://github.com/csyxwei/MasterWeaver ![](https://img.shields.io/github/stars/csyxwei/MasterWeaver.svg)
  * 架构图：

  ![image](pic/masterweaver.jpg)

* **PhotoVerse: Tuning-Free Image Customization with Text-to-Image Diffusion Models**

  * 地址：https://github.com/idonahum/photoVerse ![](https://img.shields.io/github/stars/idonahum/photoVerse.svg)
  * 架构图：

  ![image](pic/photoverse.png)

* **UniPortrait: A Unified Framework for Identity-Preserving Single- and Multi-Human Image Personalization**

  * 地址：https://github.com/junjiehe96/UniPortrait ![](https://img.shields.io/github/stars/junjiehe96/UniPortrait.svg)
  * 架构图：

  ![image](pic/uniportrait.png)

* **RealisID: Scale-Robust and Fine-Controllable Identity Customization via Local and Global Complementation**

  * 地址：https://arxiv.org/abs/2412.16832
  * 架构图：

  ![image](pic/realisid.png)

* **FlashFace: Human Image Personalization with High-fidelity Identity Preservation**

  * 地址：https://github.com/ali-vilab/FlashFace ![](https://img.shields.io/github/stars/ali-vilab/FlashFace.svg)
  * 架构图：

  ![image](pic/flashface.png)

* **Turn That Frown Upside Down:FaceID Customization via Cross-Training Data**

  * 地址：https://github.com/ShuheSH/CrossFaceID ![](https://img.shields.io/github/stars/ShuheSH/CrossFaceID.svg)
  * 架构图：

  ![image](pic/crossid.png)

* **DreamID: High-Fidelity and Fast diffusion-based Face Swapping via Triplet ID Group Learning**

  * 地址：https://github.com/superhero-7/DreamID ![](https://img.shields.io/github/stars/superhero-7/DreamID.svg)
  * 架构图：

  ![image](pic/dreamid.png)

* **ID-Booth: Identity-consistent Face Generation with Diffusion Models**

  * 地址：https://github.com/dariant/ID-Booth ![](https://img.shields.io/github/stars/dariant/ID-Booth.svg)
  * 架构图：
  
  ![image](pic/id_booth.png)

* **FaceSnap: Enhanced ID-fidelity Network for Tuning-free Portrait Customization**

  * 地址：https://arxiv.org/abs/2602.00627
  * 架构图：

  ![image](pic/facesnap.jpg)

* **Diff-PC: Identity-preserving and 3D-aware Controllable Diffusion for Zero-shot Portrait Customization**

  * 地址：https://arxiv.org/abs/2602.00639
  * 架构图：

  ![image](pic/diff-pc.jpg)

* **Training for Identity, Inference for Controllability: A Unified Approach to Tuning-Free Face Personalization**

  * 地址：https://github.com/lyuPang/UniID ![](https://img.shields.io/github/stars/lyuPang/UniID.svg)
  * 架构图：

  ![image](pic/uniid.jpg)

###  2. <a name='评测'></a>测评



* **SconeEval: Benchmark for Subject-Driven Composition and Distinction**

  * 地址：https://huggingface.co/datasets/Ryann829/SconeEval
  * 简介：面向 subject-driven image generation 的组合与区分能力测评集，覆盖复杂参考图、多主体组合和目标主体辨别。

* **DSH-Bench: A Difficulty- and Scenario-Aware Benchmark with Hierarchical Subject Taxonomy for Subject-Driven Text-to-Image Generation**

  * 地址：https://arxiv.org/abs/2603.08090
  * 简介：面向 subject-driven T2I 的分难度、分场景层级测评体系，包含 Subject Identity Consistency Score 等评估指标。

###  3. <a name='数据集'></a>数据集

* **OpenSubject: Leveraging Video-Derived Identity and Diversity Priors for Subject-driven Image Generation and Manipulation**

  * 地址：https://arxiv.org/abs/2512.08294
  * 简介：从视频中构造的 subject-driven generation / manipulation 数据集与 benchmark，包含跨帧身份先验和复杂场景样本。

* **Proteus-Bench: Benchmark for Video Identity Customization**

  * 地址：https://grenoble-zhang.github.io/Proteus-ID/
  * 简介：Proteus-ID 提出的身份一致视频定制训练与测评数据，覆盖身份保持、文本对齐和运动质量评估。

## Star History

<a href="https://star-history.com/#leeguandong/Awesome-ID-Customization&Date">

  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://api.star-history.com/svg?repos=leeguandong/Awesome-ID-Customization&type=Date&theme=dark" />
    <source media="(prefers-color-scheme: light)" srcset="https://api.star-history.com/svg?repos=leeguandong/Awesome-ID-Customization&type=Date" />
    <img alt="Star History Chart" src="https://api.star-history.com/svg?repos=leeguandong/Awesome-ID-Customization&type=Date" />
  </picture>
</a>
