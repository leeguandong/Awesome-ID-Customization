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
    
    - [1.1 基于DiT架构](#11-Flux模型)
    - [1.2 基于unet架构](#12-Unet模型)
    
    
  
- [Star History](#star-history)

###  1. <a name='模型'></a>人物自定义模型

#### 1.1 Flux模型

* **EditID: Training-Free Editable ID Customization for Text-to-Image Generation**
  
  * 地址：https://github.com/leeguandong/IBench ![](https://img.shields.io/github/stars/typemovie/IBench.svg)  
  * 架构图：
  
   ![image](pic/editid.png)

* **EditIDv2: Editable ID Customization with Data-Lubricated ID Feature Integration for Text-to-Image Generation**
  
  * 地址：https://github.com/typemovie/EditIDv2 ![](https://img.shields.io/github/starstypemovie/EditIDv2.svg)
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

* **ACE++: Instruction-Based Image Creation and Editing via Context-Aware Content Fillingn**
  
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
  
  * 地址：[https://github.com/bytedance/FaceCLIP]![](https://img.shields.io/github/stars/bytedance/FaceCLIP.svg)
  * 架构图：
  
  ![image](pic/faceclip.jpeg)
  

#### 1.2 Unet模型

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

###  2. <a name='评测'></a>测评



###  3. <a name='数据集'></a>数据集



## Star History

<a href="https://star-history.com/#leeguandong/Awesome-ID-Customization&Date">

  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://api.star-history.com/svg?repos=leeguandong/Awesome-ID-Customization&type=Date&theme=dark" />
    <source media="(prefers-color-scheme: light)" srcset="https://api.star-history.com/svg?repos=leeguandong/Awesome-ID-Customization&type=Date" />
    <img alt="Star History Chart" src="https://api.star-history.com/svg?repos=leeguandong/Awesome-ID-Customization&type=Date" />
  </picture>
</a>
