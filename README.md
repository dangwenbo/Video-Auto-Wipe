# Video-Auto-Wipe
&emsp;&emsp;本人不定期的基于生成技术制作一些好玩有趣的算法模型，这次带来的作品是“视频擦除”方向的应用模型，它实现的功能是自动感知到视频中我们不想看见的部分（譬如广告、水印、字幕、图标等等）然后进行擦除。目前已开放出“体验版”模型供大家玩耍，希望能帮助到有需要的朋友。请注意，<b>本人制作此模型希望能帮助大家提升工作效率，请您在合规、合适的场景下使用，本人对于您的使用造成的结果概不负责</b>。<br />
&emsp;&emsp;我后续会持续不断的探索和制作新的生成方向的技术内容。基于生成模型可玩的点还有很多，此项目仅展示了其中一个做落地应用的例子。本项目的模型版权所属为：[www.seeprettyface.com](www.seeprettyface.com) ，未获得授权严禁直接用作商业用途。关于算法的细节介绍可以参阅我的[研究笔记](http://www.seeprettyface.com/research_notes_page3.html)。<br/><br/><br/><br/>

# 效果预览
## 1. 图标擦除
&emsp;&emsp;图标擦除模型的功能是模型自动感知到视频中图标的位置然后进行擦除，感知图标的方法为在时域上静止不动的小块像素块被视作图标。<br/><br/>

### 1.1 测试1-电视剧的台标、剧名和角标擦除
![Image text](https://github.com/a312863063/Video-Auto-Wipe/blob/main/pics/de-logo/delogo_1.JPG)<br/>
<p align="center"><a href='http://www.seeprettyface.com/mp4/video-inpainting/delogo_01.mp4' target='_blank'>查看视频</a></p>
<br/><br/>

### 1.2 测试2-足球赛的台标、状态栏擦除
![Image text](https://github.com/a312863063/Video-Auto-Wipe/blob/main/pics/de-logo/delogo_2.JPG)<br/>
<p align="center"><a href='http://www.seeprettyface.com/mp4/video-inpainting/delogo_02.mp4' target='_blank'>查看视频</a></p>
<br/><br/>

### 1.3 测试3-综艺节目的台标、状态栏擦除
![Image text](https://github.com/a312863063/Video-Auto-Wipe/blob/main/pics/de-logo/delogo_3.JPG)<br/>
<p align="center"><a href='http://www.seeprettyface.com/mp4/video-inpainting/delogo_03.mp4' target='_blank'>查看视频</a></p>
<br/><br/>

### 1.4 测试4-短视频MV的遮挡图标擦除
![Image text](https://github.com/a312863063/Video-Auto-Wipe/blob/main/pics/de-logo/delogo_4.JPG)<br/>
<p align="center"><a href='http://www.seeprettyface.com/mp4/video-inpainting/delogo_04.mp4' target='_blank'>查看视频</a></p>
<br/><br/>

### 1.5 测试5-短视频MV的遮挡水印擦除
![Image text](https://github.com/a312863063/Video-Auto-Wipe/blob/main/pics/de-logo/delogo_5.JPG)<br/>
<p align="center"><a href='http://www.seeprettyface.com/mp4/video-inpainting/delogo_05.mp4' target='_blank'>查看视频</a></p>
<br/><br/>

### 1.6 测试6-新闻媒体的台标擦除
![Image text](https://github.com/a312863063/Video-Auto-Wipe/blob/main/pics/de-logo/delogo_6.JPG)<br/>
<p align="center"><a href='http://www.seeprettyface.com/mp4/video-inpainting/delogo_06.mp4' target='_blank'>查看视频</a></p>
<br/><br/><br/><br/>

## 2. 动态图标擦除
&emsp;&emsp;动态图标擦除模型的功能是模型自动感知到视频中动态图标的位置然后进行擦除，感知动态图标的方法为在时域上闪烁出现或动态移动的固定像素块被视作动态图标，这个在制作上有一定难度所以还没有对外开放。<br/><br/>
### 2.1 测试1-闪烁出现的特效文字擦除
![Image text](https://github.com/a312863063/Video-Auto-Wipe/blob/main/pics/de-dynamic-logo/de-dynamic-logo_1.JPG)<br/><br/>
![Image text](https://github.com/a312863063/Video-Auto-Wipe/blob/main/pics/de-dynamic-logo/de-dynamic-logo_2.JPG)<br/>
<p align="center"><a href='http://www.seeprettyface.com/mp4/video-inpainting/de_dynamic_logo.mp4' target='_blank'>查看视频</a></p>
<br/><br/><br/><br/> 

## 3. 字幕擦除
&emsp;&emsp;字幕擦除模型的功能是模型自动感知到视频中字幕的位置然后进行擦除，感知字幕的方法为具有统一样式的文字区域被视作字幕。
### 3.1 测试1-电影字幕擦除
![Image text](https://github.com/a312863063/Video-Auto-Wipe/blob/main/pics/de-text/detext_1.JPG)<br/>
<p align="center"><a href='http://www.seeprettyface.com/mp4/video-inpainting/detext_01.mp4' target='_blank'>查看视频</a></p>
<br/><br/>

### 3.2 测试2-电视剧字幕擦除
![Image text](https://github.com/a312863063/Video-Auto-Wipe/blob/main/pics/de-text/detext_2.JPG)<br/>
<p align="center"><a href='http://www.seeprettyface.com/mp4/video-inpainting/detext_02.mp4' target='_blank'>查看视频</a></p>
<br/><br/>

### 3.3 测试3-综艺节目字幕擦除
![Image text](https://github.com/a312863063/Video-Auto-Wipe/blob/main/pics/de-text/detext_3.JPG)<br/>
<p align="center"><a href='http://www.seeprettyface.com/mp4/video-inpainting/detext_03.mp4' target='_blank'>查看视频</a></p>
<br/><br/>

### 3.4 测试4-综艺节目特殊字幕擦除
![Image text](https://github.com/a312863063/Video-Auto-Wipe/blob/main/pics/de-text/detext_4.JPG)<br/>
<p align="center"><a href='http://www.seeprettyface.com/mp4/video-inpainting/detext_04.mp4' target='_blank'>查看视频</a></p>
<br/><br/>

### 3.5 测试5-网络视频字幕擦除
![Image text](https://github.com/a312863063/Video-Auto-Wipe/blob/main/pics/de-text/detext_5.JPG)<br/>
<p align="center"><a href='http://www.seeprettyface.com/mp4/video-inpainting/detext_05.mp4' target='_blank'>查看视频</a></p>
<br/><br/>

### 3.6 测试6-小语种字幕擦除
![Image text](https://github.com/a312863063/Video-Auto-Wipe/blob/main/pics/de-text/detext_9_ko.JPG)<br/>
<p align="center"><a href='http://www.seeprettyface.com/mp4/video-inpainting/detext_06.mp4' target='_blank'>查看视频</a></p>
<br/><br/><br/><br/>


# 使用方法
### 1.环境配置
&emsp;&emsp;torch>1.0<br/>
&emsp;&emsp;其他的缺什么依赖就pip install xxx，需要的东西不多<br/><br/>

### 2.运行方法
&emsp;&emsp;1. 下载预训练模型放在pretrained-weight文件夹里；<br/>
&emsp;&emsp;&emsp;&emsp;预训练模型下载地址：https://pan.baidu.com/s/12Kv9DkyhLE5sWEiwm59_IA  提取码：pela <br/> <br/>
&emsp;&emsp;2. 将视频文件和mask文件放在input文件夹里，编辑demo.py(或通过命令行参数)选中对应文件位置；<br/>
&emsp;&emsp;&emsp;&emsp;输入样例下载地址：https://pan.baidu.com/s/1R366Zu8TGMyv5C9kXkC9Gw  提取码：x73i <br/> <br/>
&emsp;&emsp;3. 图标擦除任务运行：``python demo.py delogo``<br/>
&emsp;&emsp;&emsp;字幕擦除任务运行：``python demo.py detext``<br/><br/><br/><br/>

# 训练方法
### 训练数据
&emsp;&emsp;1.YoutubeVOS2018数据集；<br/><br/>
&emsp;&emsp;2.基于搜集的300余部高清电影制作了2,709部电影片段数据集；<br/>
&emsp;&emsp;&emsp;&emsp;下载地址：https://pan.baidu.com/s/1CIgJmFmx5iR2JfgAyjVaeg  提取码：xb7o <br/><br/>
&emsp;&emsp;3.基于搜集的40余部综艺节目制作了864部综艺片段数据集；<br/>
&emsp;&emsp;&emsp;&emsp;下载地址：https://pan.baidu.com/s/1lJk6IIWlwxknAie0LlGYOg  提取码：9rd4 <br/><br/>
&emsp;&emsp;4.基于搜集的180,000余张图标素材制作了36,000余张图标数据集。<br/><br/>

### 训练过程
&emsp;&emsp;第1步. 针对特定任务的时域感知训练；<br/>
&emsp;&emsp;第2步. 融合擦除模型的微调训练。<br/>
<br/>
### 训练配置
&emsp;&emsp;图标擦除模型在单卡3090上训练6天；<br/>
&emsp;&emsp;字幕擦除模型在单卡2080Ti上训练4天；<br/>

<br/><br/><br/><br/>
# 衍伸玩法
&emsp;&emsp;这个项目目前还只是自己做着好玩的，开放出的模型是比较糙的训练结果（在揉合的数据集上直接训练）。视频擦除的衍伸任务也有很多，譬如敏感内容（涉黄涉暴等）擦除、广告擦除、指定人/物擦除、背景人擦除等等，只要能寻找到有像素预测的场景+有像素预测的需求都是“视频擦除”可以玩出花样的情景~<br/>
<p align="center">
	<img src="https://github.com/a312863063/Video-Auto-Wipe/blob/main/pics/undo.png" alt="Sample" width="640" >
</p>
<br/><br/><br/><br/>

# 了解更多
&emsp;&emsp;本人的研究方向是生成模型的应用技术研究。生成技术解决的问题是像素的预测，也就是在一个有缺失/完全缺失的图像棋盘上进行像素的填补/预测，使填补/预测完的图像符合真实图像的规律。基于这种模式可展开的玩法有很多，除了我之前做的数字人生成、视频内容生成等，我们还可以拓展出更多并行的思路出来。<br/>
&emsp;&emsp;尽管目前大部分的CV落地项目都集中在感知和识别任务上，而对于重构和生成任务的研发相对较少，但这不应影响我们对于生成技术价值的判断，毕竟生成技术是相对较新的、参与人较少的研究方向。我后续将持续致力于探索生成方向的落地型算法研发，欢迎访问我的网站了解这方面最新的研究进展：[www.seeprettyface.com](http://www.seeprettyface.com)。<br/>
<p align="center">
	<img src="https://github.com/a312863063/Video-Auto-Wipe/blob/main/pics/cover.png" alt="Sample" width="512" >
</p>





