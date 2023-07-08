# Stable Diffution学习


## 学习资料，来源于吴东子
```
《耗时80小时！超详细的胎教级Stable Diffusion使用教程，看这一篇就够！》
https://ry5hwpuf7b.feishu.cn/docx/HYrZdLBMRorB0qxKqFFcQ075nWf

《瞬息全宇宙终极教程，手把手教你做出百万点赞视频》
【穿越之旅】https://ry5hwpuf7b.feishu.cn/docx/WbFVdvGkAoo38ZxDumwclWEynRg
【平行宇宙】https://ry5hwpuf7b.feishu.cn/docx/Lfjedtd4QoCkBhxkgTfcBsG1np0

《保姆级Lora炼丹教程，一站式整合包，让你实现真人模特定制》
https://ry5hwpuf7b.feishu.cn/docx/LUmKdLd0AofzbcxFRkQcg56Rnnf

《耗时7天，终于把15种ControlNet模型搞明白了！》
https://ry5hwpuf7b.feishu.cn/docx/NeqIdWC9PovqQ6xruAJcErqHnxc
```

## Stable Diffusion使用教程
* 使用青椒云
    * https://my.qingjiaocloud.com/billing/buying?property=0&productType=11395&region=3&pricingMode=5
    * 选择定制产品 赛博丹炉V1.42(朱尼酱独家)
    * 2.5元一小时
* 写关键词
    * 正面词
        * 画质 + 主体 + 主体细节 + 人物服饰 + 其他（背景，天气，构图风格）
        * 单词用英文,隔开
        * 权重
            * 加权重 (curly hair) 1.1倍， ((curly hair)) 1.1 * 1.1 = 1.21，(curly hair: 1.3) 1.3倍
            * 减权重 [curly hair] ，(curly hair: 0.9) 
    * 负面词
        * 比如不希望出现的，低质量，多余的手
        *  (worst quality:2), (low quality:2), (normal quality:2), lowres, ((monochrome)), ((grayscale)), bad anatomy,DeepNegative, skin spots, acnes, skin blemishes,(fat:1.2),facing away, looking away,tilted head, lowres,bad anatomy,bad hands, missing fingers,extra digit, fewer digits,bad feet,poorly drawn hands,poorly drawn face,mutation,deformed,extra fingers,extra limbs,extra arms,extra legs,malformed limbs,fused fingers,too many fingers,long neck,cross-eyed,mutated hands,polar lowres,bad body,bad proportions,gross proportions,missing arms,missing legs,extra digit, extra arms, extra leg, extra foot,teethcroppe,signature, watermark, username,blurry,cropped,jpeg artifacts,text,error,
* 知识点
    * VAE，就是色彩更丰富一点，有点像加滤镜
    * 迭代步数，相当于画笔数，越多就越清晰，出图也会越慢 25 ~ 30之间就好
    * 采样方法，Euler a、DPM++ 2S a Karras、DPM++ 2M Karras
    * 面部修复，用在真人照片上
    * 高分辨率修复， 修复大的图片
    * 图片分辨率，正方形512 * 512，长方形512 * 768
    * 用脚本来对比不同关键词以及采样方式
        