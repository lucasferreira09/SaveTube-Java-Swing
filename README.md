<div align="center"> 
<h1> <span style="color:red"> SaveTube </span> </h1>
</div>

#

<div align="center">

![YouTube](https://img.shields.io/badge/YouTube-%23FF0000.svg?style=for-the-badge&logo=YouTube&logoColor=white)

## Download videos and audios from YouTube for free and without ads!
</div>


## ⚠️ This project is only for academic purposes!
## Application: https://github.com/lucasferreira09/Video-Downloader-Swing.git

##
## 🤔 How to use?

#### 🔗 All you have to do is past the link in the rectangular box next to download image and click in SEARCH.
#### 🚫 Please don't use direct playlist links—they are not supported. However, if it's a video from a playlist, then it's supported.

#### 👀 Take a look
![PASTE-LINK](https://github.com/lucasferreira09/SaveTube-Java-Swing/blob/02036f427120fe979e2be07695e98970a9f3545a/screenshots/paste_link_video.png)

##

## 📂 You can choose the download location too.
![DOWNLOAD-PATH](https://github.com/lucasferreira09/SaveTube-Java-Swing/blob/02036f427120fe979e2be07695e98970a9f3545a/screenshots/download_path.png)

##


## ⌛Once you have pasted the link and waited a little time. The app will show you the available video options.

![VIDEOS-OPTIONS](https://github.com/lucasferreira09/SaveTube-Java-Swing/blob/b0eb2b8cfca339efce0dd4cb3784325ee7f7d629/screenshots/video_options.png)

##


## 🎵 You can download only the audio, if you want to.
![AUDIO](https://github.com/lucasferreira09/SaveTube-Java-Swing/blob/02036f427120fe979e2be07695e98970a9f3545a/screenshots/audio.png)

#
# ✍️ **CREATION**
#
## 📂 Project Structure

![Project-Structure](https://github.com/lucasferreira09/SaveTube-Java-Swing/blob/b0eb2b8cfca339efce0dd4cb3784325ee7f7d629/screenshots/project_structure.png)

##
## 🤖 Technologies used

> ### <span style="color:red"> **Jawa Swing | Yt-dlp | Ffmpeg | ProcessBuilder | BufferedReader | Threads | Callback | MVC Pattern** </span>
# 
#
# 🤔 How did I make this application?👨‍💻

### First of all, I need to get what the Ytdlp returns.
### Then process it, and show only what is necessary to the user, in a cool interface.

## Like this👇
![YTDLP-RETURN](https://github.com/lucasferreira09/SaveTube-Java-Swing/blob/b0eb2b8cfca339efce0dd4cb3784325ee7f7d629/screenshots/ytdlp_return_information.png)

## The  <span style="color:red"> **getInformationEachVideo()** </span> method of the DownloaderSystem class takes this function. It retrieves the **title, quality, size, code and thumbnail.**

![DOWNLOADER-SYSTEM-CLASS](https://github.com/lucasferreira09/SaveTube-Java-Swing/blob/b0eb2b8cfca339efce0dd4cb3784325ee7f7d629/screenshots/downloader_system_class.png)

### 🔴 The _**DownloaderSystem**_ class from the model package is the application's heart. It _**handles everything related to processing video and audio data**_. Without it, there would be no application.

### 🔴 All of the information that Ytdlp returns is stored in an ArrayList.
### The line contains the _**code, quality, size and other irrelevant information**_. So, I have to extract this for each video option.
### Each video option's quality is added to a HashMap as a key and the value for that key is an ArrayList containing the code and size of the corresponding video option.

> ### ⚠️**For example, suppose this is a line that Ytdlp returns:**
> ### **323 mp4 1920x1080 00 | 500mb 434k m3u8 | dsds.234434 3245k video_only**
> ### 👉**I need to extract '323', '1920x1080' and '500mb'**

### 
### Then, put it into the HashMap, like this:

> * ### Create an ArrayList and add the code and size ('323' and '500mb').
> * ### Create a HashMap and add the quality as the key ('1080'), and the ArrayList you just created as the value.
#
#
## 🖥️ Then, the controller's methods will display each video option of this HashMap to the user in a cool interface.

