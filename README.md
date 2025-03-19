# AnimateDiff Lightning: Does Faster Computation Result in Lower Fidelity?

## Overview

This project examines the trade-off between computational efficiency and video quality in diffusion-based video generation. Our focus is on **AnimateDiff-Lightning**, a variant designed to accelerate video generation while maintaining—or even improving—output fidelity compared to the original **AnimateDiff** model.

| AnimateDiff-Lightning   | AnimateDiff   |
|------------|------------|
| ![Urban_Exploration_lightning_pipe_Prompt3](https://github.com/user-attachments/assets/29f0a832-ed68-4ad3-8d3e-0dc76ec01808)| ![Urban_Exploration_original_pipe_Prompt3](https://github.com/user-attachments/assets/b61a14f6-4100-4540-845d-d8213a23a4a2)| 


## Objectives

- **Research Question:**  
  Can AnimateDiff-Lightning achieve comparable or better video quality than the original AnimateDiff while significantly reducing computational costs?

- **Goal:**  
  Through systematic benchmarking and A/B testing across diverse themes and evaluation metrics, determine whether the lightning-fast model maintains high fidelity or introduces trade-offs in video quality.

## Methods

- **Dataset & Prompts:**  
  - Generate videos in GIF format from 100 diverse text prompts covering themes such as sports, nature, wildlife, and urban exploration.
  - Prompts were carefully crafted with varying levels of detail and complexity to challenge both models equally.

- **Standardization:**  
  - Ensure fair comparison by standardizing parameters such as guidance scale, inference steps, and base model style.

- **Evaluation Framework:**  
  - **A/B Testing:**  
    Evaluators were presented with pairs of GIFs (one from AnimateDiff-Lightning and one from AnimateDiff) in randomized order.
  - **Scoring Criteria:**  
    - **Video-Text Relevance:** Measures how accurately the GIF represents the provided text prompt.
    - **Appearance Distortion:** Assesses the extent of visual artifacts or deformities.
    - **Appearance Aesthetics:** Evaluates overall visual appeal, including design consistency and color harmony.
    - **Motion Naturalness:** Examines the fluidity and believability of movement.
    - **Motion Amplitude:** Reflects the appropriate range and dynamism of movement.
    - **Overall Quality:** A holistic measure combining all the above metrics.

## Results

- **Overall Preferences:**  
  AnimateDiff-Lightning was strongly preferred across all metrics, indicating higher overall performance.

- **Metric-Specific Insights:**  
  - **Motion Naturalness, Motion Amplitude, and Video-Text Relevance:**  
    These metrics showed closer results between the two models.
  - **Theme-Specific Findings:**  
    - For abstract concepts and mystical themes, the differences were less pronounced.
    - In most cases, however, Model A demonstrated a significant advantage.

## Conclusion

The benchmarking results indicate that **AnimateDiff-Lightning** is not only faster but also generates higher fidelity GIFs compared to the original AnimateDiff model. These findings suggest that enhanced computational efficiency does not come at the cost of video quality—in fact, the lightning variant often outperforms its predecessor in key quality metrics.

## Acknowledgements

We acknowledge the contributions of the following works:
- Lin, S., & Xiao, Y. (2024). *Animatediff-lightning: Cross-model diffusion distillation.* [arXiv:2403.12706](https://arxiv.org/abs/2403.12706)
- Guo, Y., Yang, C., Rao, A., Liang, Z., Wang, Y., Qiao, Y., Agrawala, M., Lin, D., & Dai, B. (2023). *AnimateDiff: Animate Your Personalized Text-to-Image Diffusion Models without Specific Tuning.* [arXiv:2307.04725](https://arxiv.org/abs/2307.04725)
- Zhou, Y., Wang, Q., Cai, Y., & Yang, H. (2024). *Allegro: Open the black box of Commercial-Level Video Generation Model.* [arXiv:2410.15458](https://arxiv.org/abs/2410.15458)

## Authors:
  - Yow Siao Kang
  - Chan Jie Ru
  - Yee Jia Zhen
  - Ong Wei Xiang
  - Huang Jiayi


## Viewing the Poster

For detailed insights and visual representations of our evaluation, please refer to the project poster: [Project_Poster.pdf](Project_Poster.pdf)
