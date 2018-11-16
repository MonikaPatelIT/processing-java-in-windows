## Set up processing-java on windows

I came know about `processing-java` from David Shiffman video tutorials [15.6: Tweeting images with Processing - Twitter Bot Tutorial](https://www.youtube.com/watch?v=mUoIPmZ4KwA)

I had issue installing and using processing-java as most of had so thought write down notes for myself and share to others to help.

### 1. Download processing-java 
Here is link you can download latest version [https://processing.org/download/](https://processing.org/download/)

### 2. UnZip and check it's working?
Now you just unzip the folder you just downloaded and using command line  run the following command to check it's working or not
```
processing-java
```
You will see the list of commands if it's working.

![image](https://user-images.githubusercontent.com/9668906/48587612-aeb1f880-e998-11e8-9d46-86d648afa3b9.png)

### 3. Set `Path` enviroment element.
Now you copy across the extracted folder 'processing-java' into your C:\Program Files and edit enviroment variable for path.
![image](https://user-images.githubusercontent.com/9668906/48592602-17f03680-e9ae-11e8-8a0a-24ab1e998c96.png)


### 4. Draw something using processing.exe
![image](https://user-images.githubusercontent.com/9668906/48592523-a7e1b080-e9ad-11e8-9515-24185d20bb25.png)
following code will give you doted pattern
```
void setup(){
size(600,400);
background(21);
for(int i=0; i<1000; i++){
  float x= random(width);
  float y= random(height);
  float r= random(100,255);
  float b= random(100,255);
  noStroke();
  fill(r,0,b,100);
  ellipse(x,y,16,16);
}
save("output.png");
exit(); // will close the image automatically after few second
}
```
![image](https://user-images.githubusercontent.com/9668906/48592678-5ab20e80-e9ae-11e8-8fbb-68774bb27f8e.png)

### 5. 'Save as' the sketch in your project folder
  It's not compulsory to save it. but easier if you do so.

### 6. Run the Sketch 

```
processing-java --sketch="C:\Users\MonikaP.SCANTECH\Documents\Visual Studio 2017\WebSites\node-twit-bot\rainbow" --run
```
![image](https://user-images.githubusercontent.com/9668906/48593517-fbee9400-e9b1-11e8-9e39-b413668e633e.png)




