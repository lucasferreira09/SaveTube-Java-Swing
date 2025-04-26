<div align="center"> 
<<<<<<< Updated upstream
<h1> SaveTube </h1>
=======
<<<<<<< HEAD
<h1> <span style="color:red"> SaveTube </span> </h1>
</div>
=======
<h1> SaveTube </h1>
>>>>>>> 4f6db116365a02b427f75fab0dee75b430713b58
>>>>>>> Stashed changes
  
![YouTube](https://img.shields.io/badge/YouTube-%23FF0000.svg?style=for-the-badge&logo=YouTube&logoColor=white)
</div>


### Download videos and audios from YouTube for free and without ads!
### ⚠️ Due to copyright reasons, i won't release the app. I'll just share some screenshots, the project structure and the technologies I used and how it works. Cool?
##

<<<<<<< HEAD
=======
## 📂 Project Structure

![Project-Structure](https://github.com/lucasferreira09/SaveTube-Java-Swing/blob/02036f427120fe979e2be07695e98970a9f3545a/screenshots/project_structure.png)
##
## 🤖 Technologies used

> ### Jawa Swing | Yt-dlp | Ffmpeg | ProcessBuilder | BufferedReader | Threads | Callback | MVC Pattern

>>>>>>> 4f6db116365a02b427f75fab0dee75b430713b58
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

![VIDEOS-OPTIONS](https://github.com/lucasferreira09/SaveTube-Java-Swing/blob/02036f427120fe979e2be07695e98970a9f3545a/screenshots/video_options.png)

##


## 🎵 You can download only the audio, if you want to.
<<<<<<< Updated upstream
![AUDIO](https://github.com/lucasferreira09/SaveTube-Java-Swing/blob/02036f427120fe979e2be07695e98970a9f3545a/screenshots/audio.png)
=======
<<<<<<< HEAD
![AUDIO](screenshots\audio.png)

#
# ✍️ **CREATION**
#
## 📂 Project Structure

![Project-Structure](screenshots/project_structure.png)
##
## 🤖 Technologies used

> ### <span style="color:red"> **Jawa Swing | Yt-dlp | Ffmpeg | ProcessBuilder | BufferedReader | Threads | Callback | MVC Pattern** </span>
# 
#
# 🤔 How did I make this application?👨‍💻

### First of all, I need to get what the Ytdlp returns.
### Then process it, and show only what is necessary to the user, in a cool interface.

## Like this👇
![YTDLP-RETURN](screenshots/ytdlp_return_information.png)

## The  <span style="color:red"> **getInformationEachVideo()** </span> method of the DownloaderSystem class takes this function. It retrieves the **title, quality, size, code and thumbnail.**

![DOWNLOADER-SYSTEM-CLASS](screenshots/downloader_system_class.png)

## The <span style="color:red"> **DownloaderSystem** </span> class from the model package is the application's heart. It <span style="color:red"> **handles everything related to processing video and audio data**</span>. Without it, there would be no application.

### All of the information that Ytdlp returns is stored in an ArrayList.
### The line contains the code, quality, size and other irrelevant information. So, I have to extract this for each video option.
### Each video option's quality is added to a HashMap as a key and the value for that key is an ArrayList containing the code and size of the corresponding video option.

> ### For example, suppose this is a line that Ytdlp returns:
> ### <span style="color:red">  -- 323 mp4 1920x1080 00 | 500mb 434k m3u8 | dsds.234434 3245k video_only </span>
> ### I need to extract '323', '1920x1080' and '500mb'

### 
### Then, put it into the HashMap, like this:

> * ### Create an ArrayList and add the code and size ('323' and '500mb').
> * ### Create a HashMap and add the quality as the key ('1080'), and the ArrayList you just created as the value.
#
#
## 🖥️ Then, the controller's methods will display each video option of this HashMap to the user in a cool interface.












=======
![AUDIO](https://github.com/lucasferreira09/SaveTube-Java-Swing/blob/02036f427120fe979e2be07695e98970a9f3545a/screenshots/audio.png)
>>>>>>> 4f6db116365a02b427f75fab0dee75b430713b58
>>>>>>> Stashed changes
