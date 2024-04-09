## 图像分隔sota
  UniRef++: Segment Every Reference Object in Spatial and Temporal Spaces，https://arxiv.org/pdf/2312.15715.pdf
## text-embedding模型sota
  ### sota榜
  https://huggingface.co/spaces/mteb/leaderboard，
  ### bge-base模型
  https://github.com/FlagOpen/FlagEmbedding/blob/master/README_zh.md

## kg与RAG结合的讨论
  https://discuss.nebula-graph.com.cn/t/topic/14134

## 一些AGI资讯的网站
  https://waytoagi.feishu.cn/wiki/QPe5w5g7UisbEkkow8XcDmOpn8e

## 生成图片
1. controlnet：添加控制信号给去噪过程，https://arxiv.org/abs/2302.05543，ControlNet的参数是需要训练fine tune的。fine tune完的ControlNet可以将额外的condition信息映射到参数固定的stable diffusion中。由于stable diffusion模型参数一致保持不变，它将维持强大的生成能力，而且不会因为fine tune的数据集太小而出现过拟合的问题。
2. ReferenceNet，用于有参考图的生成，https://arxiv.org/pdf/2311.17117.pdf
3. pose guider设计，将pose控制信息转为controlnet，https://arxiv.org/pdf/2311.17117.pdf
4. Temporal Layer：animatediff,https://arxiv.org/pdf/2307.04725.pdf

## comfyui库
1. 一个抠图、扣视频的的库：https://github.com/ZHO-ZHO-ZHO/ComfyUI-BiRefNet-ZHO
2. 一个动画着色的库：https://github.com/ykdai/BasicPBC
3. 基于扩展模型的光照渲染：https://github.com/DiffusionLight/DiffusionLight/，https://github.com/kijai/ComfyUI-DiffusionLight ， 模型: https://cdn.discordapp.com/attachments/1145677539738665020/1224765647909683280/diffusion_light_sdxl_lora_comfy.safetensors?ex=661eaee5&is=660c39e5&hm=06d70f334da69f6f7566bb1f3175586cfd1fdb3648f85a2be569907a4334ed9b&
4. champ的confy节点：https://github.com/kijai/ComfyUI-champWrapper
5. 一个开源数字人的库museV：https://github.com/TMElyralab/MuseV/blob/main/README-zh.md
6. 支撑生成透明背景：https://github.com/huchenlei/ComfyUI-layerdiffuse
7. 一个开源的声音clone库（从demo对比看，英文表达比gpt-sovits好，中文还没试）：https://github.com/kijai/ComfyUI-VoiceCraft



## 文本到动作到视频流
text to motion to video by Kijai@discord
added some features to MotionDiff so it outputs a perfect normal map and mask, depth it already did, dwpose works great with the normal output
also got it running 10 times faster
first frame of that to init image, that through tiled ipadapter to standard AnimateLCM pipe
oh and added sparsergb for first frame
https://discord.com/channels/1076117621407223829/1145677539738665020/1222684351666458716

