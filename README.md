**<h1>Introduction</h1>**
INTUZ is presenting an interesting Video Editing Control to integrate inside your Android based application. 
Video Trimmer is a simple component, which lets you trim your videos files on the fly. You can see preview video before trimming your selected video.
Please follow the below steps to integrate this control in your next project.

<br/><br/>
**<h1>Features</h1>**
* Easy & Fast to make video modification.
* You can select a range of video to be trimmed.
* Ability to pick/capture a video and trim it.
* Ability to play selected range of video before trimming.
* Video quality remain as it have in original files.
* You can play video range before actually trimming the video.
* Fully customised design layout.

<br/><br/>
<img src="Screenshots/videotrimmer.gif" width="300" alt="Screenshots/VideoTrim1.png">



<br/><br/>
**<h1>Getting Started</h1>**

To use this component in your project you need to perform below steps:

1) Start <b>VideoTrimmerActivity</b> with startActivityForResult with your video path:

```
startActivityForResult(new Intent(MainActivity.this, VideoTrimmerActivity.class).putExtra("EXTRA_PATH", path), VIDEO_TRIM);
```
2) Handle your <b>onActivityResult</b> for getting trimmer video path:
```
if (requestCode == VIDEO_TRIM) { 
   if (resultCode == RESULT_OK) { 
       if (data != null) { 
          String videoPath = data.getExtras().getString("INTENT_VIDEO_FILE"); 
          Toast.makeText(MainActivity.this, "Video stored at " + videoPath, Toast.LENGTH_LONG).show();
                         } 
                     }
                 }
```

<br/><br/>
**<h1>Bugs and Feedback</h1>**
For bugs, questions and discussions please use the Github Issues.

<br/><br/>
**<h1>License</h1>**
The MIT License (MIT)
<br/><br/>
Copyright (c) 2018 INTUZ
<br/><br/>
Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions: 
<br/><br/>
THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

<br/><br/>
<h1>Acknowledgments</h1>
<a href="https://github.com/titansgroup/k4l-video-trimmer">k4l-video-trimmer</a>

<br/>
<h1></h1>
<a href="https://www.intuz.com/" target="_blank"><img src="Screenshots/logo.jpg"></a>


