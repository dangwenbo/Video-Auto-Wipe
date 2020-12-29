# Video-Auto-Wipe
&emsp;&emsp;I occasionally make some fun and interesting algorithm models based on generative technology. The work I brought this time is an application model in the task of "video inpainting". Its function is to automatically perceive the parts of the video that we don’t want to see (such as advertisements, watermark, subtitles, icons, etc.) and then erase it. At present, the "trial version" model has been opened for everyone to play, hoping to help friends in need. Please note that I made this model to help you improve your work efficiency, please use it in a compliant and appropriate way. I am not responsible for the results of your use.<br />
&emsp;&emsp;I will continue to explore and produce new technical content in generative models. There are still many playable points based on the generative technology, and this project only shows one of the practical examples. The model's copyright of this project belongs to: [www.seeprettyface.com](www.seeprettyface.com), directly
commercial use without authorization is not allowed . For details of the algorithm, please refer to my [research notes](http://www.seeprettyface.com/research_notes_page3.html)。<br/><br/><br/><br/>

# Effect preview
## 1. Icon erase
&emsp;&emsp;The function of the icon erasing model is that the model automatically perceives the position of the icon in the video and then erases it. The method of perceiving the icon is that small blocks of pixels that are stationary in the time domain are regarded as icons.<br/><br/>

### 1.1 Test 1
![Image text](https://github.com/a312863063/Video-Auto-Wipe/blob/main/pics/de-logo/delogo_7_en.JPG)<br/>
<p align="center"><a href='http://www.seeprettyface.com/mp4/video-inpainting/others/delogo1.mp4' target='_blank'>Watch video</a></p>
<br/><br/>

### 1.2 Test 2
![Image text](https://github.com/a312863063/Video-Auto-Wipe/blob/main/pics/de-logo/delogo_8_en.JPG)<br/>
<p align="center"><a href='http://www.seeprettyface.com/mp4/video-inpainting/others/delogo2.mp4' target='_blank'>Watch video</a></p>
<br/><br/>

### 1.3 Test 3
![Image text](https://github.com/a312863063/Video-Auto-Wipe/blob/main/pics/de-logo/delogo_9_en.JPG)<br/>
<p align="center"><a href='http://www.seeprettyface.com/mp4/video-inpainting/others/delogo3.mp4' target='_blank'>Watch video</a></p>
<br/><br/>

### 1.4 Test 4
![Image text](https://github.com/a312863063/Video-Auto-Wipe/blob/main/pics/de-logo/delogo_10_en.JPG)<br/>
<p align="center"><a href='http://www.seeprettyface.com/mp4/video-inpainting/others/delogo4.mp4' target='_blank'>Watch video</a></p>
<br/><br/>

### 1.5 Test 5
![Image text](https://github.com/a312863063/Video-Auto-Wipe/blob/main/pics/de-logo/delogo_11_en.JPG)<br/>
<p align="center"><a href='http://www.seeprettyface.com/mp4/video-inpainting/others/delogo5.mp4' target='_blank'>Watch video</a></p>
<br/><br/>

### 1.6 Test 6
![Image text](https://github.com/a312863063/Video-Auto-Wipe/blob/main/pics/de-logo/delogo_12_en.JPG)<br/>
<p align="center"><a href='http://www.seeprettyface.com/mp4/video-inpainting/others/delogo6.mp4' target='_blank'>Watch video</a></p>
<br/><br/><br/><br/>

## 2. Dynamic icon erase
&emsp;&emsp;The function of the dynamic icon erasing model is that the model automatically senses the position of the dynamic icon in the video and then erases it. The method of perceiving the dynamic icon is that the fixed pixel block that flashes or moves dynamically in the time domain is regarded as a dynamic icon. There is a certain degree of difficulty in production, so it has not been opened to the public.<br/><br/>
### 2.1 Test 1
![Image text](https://github.com/a312863063/Video-Auto-Wipe/blob/main/pics/de-dynamic-logo/de-dynamic-logo_1.JPG)<br/><br/>
![Image text](https://github.com/a312863063/Video-Auto-Wipe/blob/main/pics/de-dynamic-logo/de-dynamic-logo_2.JPG)<br/>
<p align="center"><a href='http://www.seeprettyface.com/mp4/video-inpainting/de_dynamic_logo.mp4' target='_blank'>Watch video</a></p>
<br/><br/><br/><br/> 

## 3. Subtitle erase
&emsp;&emsp;The function of the subtitle erasing model is that the model automatically perceives the position of the subtitle in the video and then erases it. The method of sensing the subtitle is that the text area with a uniform style is regarded as the subtitle.<br/><br/>
### 3.1 Test1 - English
![Image text](https://github.com/a312863063/Video-Auto-Wipe/blob/main/pics/de-text/detext_6_en.JPG)<br/>
<p align="center"><a href='http://www.seeprettyface.com/mp4/video-inpainting/others/detext1.mp4' target='_blank'>Watch video</a></p>
<br/><br/>

### 3.2 Test2 - English
![Image text](https://github.com/a312863063/Video-Auto-Wipe/blob/main/pics/de-text/detext_7_en.JPG)<br/>
<p align="center"><a href='http://www.seeprettyface.com/mp4/video-inpainting/others/detext2.mp4' target='_blank'>Watch video</a></p>
<br/><br/>

### 3.3 Test3 - Spanish
![Image text](https://github.com/a312863063/Video-Auto-Wipe/blob/main/pics/de-text/detext_8_sp.JPG)<br/>
<p align="center"><a href='http://www.seeprettyface.com/mp4/video-inpainting/others/detext3.mp4' target='_blank'>Watch video/a></p>
<br/><br/>

### 3.4 Test4 - Korean, .etc
![Image text](https://github.com/a312863063/Video-Auto-Wipe/blob/main/pics/de-text/detext_9_ko.JPG)<br/>
<p align="center"><a href='http://www.seeprettyface.com/mp4/video-inpainting/others/detext4.mp4' target='_blank'>Watch video</a></p>
<br/><br/>

### 3.5 Test5 - Russion with double subtitle occlusion
![Image text](https://github.com/a312863063/Video-Auto-Wipe/blob/main/pics/de-text/detext_10_ru.JPG)<br/>
<p align="center"><a href='http://www.seeprettyface.com/mp4/video-inpainting/others/detext5.mp4' target='_blank'>Watch video</a></p>
<br/><br/><br/><br/>


# Usage
### 1.Environment configuration
&emsp;&emsp;torch>1.0<br/>
&emsp;&emsp;If other dependencies are missing, use "pip install xxx", not much needed.<br/><br/>

### 2.Operation method
&emsp;&emsp;1. Download the pre-trained model and place it in the ``pretrained-weight`` folder;<br/>
&emsp;&emsp;&emsp;&emsp;Pre-trained model download link:https://drive.google.com/file/d/16PWnlOEDfdQ1RzwHhW5n_WPAHrG_MMea/view?usp=sharing; <br/> <br/>
&emsp;&emsp;2. Put the video file and mask file in the ``input`` folder, edit demo.py (or use command line) to select the corresponding file location;<br/>
&emsp;&emsp;&emsp;&emsp;Input samples download address:https://drive.google.com/file/d/1KECp6E77XAOZH590Ak9HvSo_KK0eRvLg/view?usp=sharing;<br/> <br/>
&emsp;&emsp;3. Icon erasing task runs:``python demo.py delogo``<br/>
&emsp;&emsp;&emsp;Subtitle erasing task runs:``python demo.py detext``<br/><br/><br/><br/>

# Training method
### Training data
&emsp;&emsp;1.YoutubeVOS2018 daraset;<br/><br/>
&emsp;&emsp;2.Based on the collected more than 300 high-definition movies, 2,709 movie fragment datasets were produced;<br/>
&emsp;&emsp;&emsp;&emsp;download link:https://pan.baidu.com/s/1CIgJmFmx5iR2JfgAyjVaeg  code: xb7o <br/><br/>
&emsp;&emsp;3.Based on the collected more than 40 variety shows, 864 variety-show fragment datasets were produced;<br/>
&emsp;&emsp;&emsp;&emsp;download link:https://pan.baidu.com/s/1lJk6IIWlwxknAie0LlGYOg  code: 9rd4 <br/><br/>
&emsp;&emsp;4.Based on the collected 180,000 icon materials, more than 36,000 icon datasets were created.<br/><br/>

### Training process
&emsp;&emsp;Step 1. Time domain perception training for specific tasks;<br/>
&emsp;&emsp;Step 2. Fine-tuning of the fusioned inapainting model.<br/>
<br/>
### Training configuration
&emsp;&emsp;The icon erasure model is trained on one 3090-GPU for 6 days;<br/>
&emsp;&emsp;The subtitle erasure model is trained on one 2080Ti-GPU for 4 days;<br/>

<br/><br/><br/><br/>
# Derivative play
&emsp;&emsp;This project is currently just doing it for fun, and the open model is a rough training result (training directly on the mixed data set). There are many extension tasks for video erasing, such as sensitive content (pornography, violence, etc.) erasing, advertisement erasing, designated person/object erasing, background person erasing, etc., as long as you can find scenes with pixel predictions where "video erasure" can show its ability greatly~<br/>
<p align="center">
	<img src="https://github.com/a312863063/Video-Auto-Wipe/blob/main/pics/undo.png" alt="Sample" width="640" >
</p>
<br/><br/><br/><br/>

# Learn more

&emsp;&emsp;Although most of the current CV landing projects are focused on perception and recognition tasks, and there is relatively little research and development on reconstruction and generation tasks, however this should not affect our judgment on the value of generation technology, after all, generation technology is relatively new Research directions with fewer participants but meantime it has a wide range of applications. I will continue to devote to the research and development of landing algorithms that explore the direction of generation. Welcome to visit my website to learn about the latest research progress in this area， the website is:[www.seeprettyface.com](http://www.seeprettyface.com)。<br/>
&emsp;&emsp;If you have the intention of cooperation, I welcome you to contact me to see if we can create more value together.<br />
<p align="center">
	<img src="https://github.com/a312863063/Video-Auto-Wipe/blob/main/pics/cover.png" alt="Sample" width="512" >
</p>





