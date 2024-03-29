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
4. Temporal Layer：https://arxiv.org/pdf/2307.04725.pdf


## 文本到动作到视频流
text to motion to video by Kijai@discord
added some features to MotionDiff so it outputs a perfect normal map and mask, depth it already did, dwpose works great with the normal output
also got it running 10 times faster
first frame of that to init image, that through tiled ipadapter to standard AnimateLCM pipe
oh and added sparsergb for first frame
https://discord.com/channels/1076117621407223829/1145677539738665020/1222684351666458716

