# HTML

- [Laurel's HTML basics](https://www.youtube.com/watch?v=CkzbI1Tv_rQ)
- Comment out: Command (Mac OS) or Ctrl (Windows) + /

### HTML tags for text

```
<p>, <span>, <br>, <hr>
<div>, <h1>, <h2>...<h6> 
<b>, <i>, <em>
<ul>, <ol>, <li>
```

### HTML `<a>` tag
```
<a href="maps.google.com"> Get direction from Google Maps!</a>
<a href="maps.google.com" target="_blank"> This will pop up from a new tab </a>
<a href="mailto:example@gmail.com"> Send me a walk! </a>
```

### HTML tags for media
```
<img src="url" alt="alternative text">
```

### HTML [Video](https://www.w3schools.com/html/html5_video.asp) and [Audio](https://www.w3schools.com/html/html5_audio.asp)

```
<video width="320" height="240" autoplay muted>
    <source src="movie.mp4" type="video/mp4">
    Your browser does not support the video tag.
</video>
```
```
<audio controls autoplay>
    <source src="horse.ogg" type="audio/ogg">
    <source src="horse.mp3" type="audio/mpeg">
    Your browser does not support the audio element.
</audio>
```

```
<a href = "https://www.art.yale.edu/">, <a href = "style.css">
<img src = "assets/my-image.png">
```
- What are some self-closing tags in HTML?

### HTML Boilerplate
```
<html>
    <head>
        <title> 
            this is the document title!
        </title>
    </head>
    <body> 
        Hello world!
    </body>
</html>
```
- HTML5 [boilerplate](https://www.freecodecamp.org/news/basic-html5-template-boilerplate-code-example/)

### HTML [`class`](https://developer.mozilla.org/en-US/docs/Web/HTML/Global_attributes/class) and [`id`](https://developer.mozilla.org/en-US/docs/Web/HTML/Global_attributes/id)

```
<div class="section" id="banner"></div>
```