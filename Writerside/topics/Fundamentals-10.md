# Video, Audio & Media in HTML

## Introduction

Welcome to the exciting realm of multimedia integration in HTML. This comprehensive guide will walk you through the
essential elements and attributes to seamlessly incorporate video and audio into your web pages. Whether you're a
beginner or an experienced developer, this guide will provide detailed insights into the intricacies of multimedia
elements in HTML.

## The Video Tag and Attributes

The `<video>` tag is the cornerstone for embedding videos in HTML. Let's explore the key attributes that enhance the
functionality and appearance of your video elements.

### SRC Attribute and Video Sizing

The `src` attribute specifies the source URL of the video file, while sizing attributes control the dimensions.

```html

<video src="video.mp4" width="640" height="360"></video>
```

- **`src`:** Specifies the source URL of the video file.
- **`width` and `height`:** Set the dimensions of the video player.

## Making Video Responsive

Ensure your videos adapt to different screen sizes with responsive design techniques.

```css
video {
    max-width: 100%;
    height: auto;
}
```

## Video Controls

Enhance user interaction by adding controls for play, pause, volume, and more.

```html

<video controls>
    <source src="video.mp4" type="video/mp4">
</video>
```

## AutoPlay Attribute

Automatically start playing the video when the page loads using the `autoplay` attribute.

```html

<video autoplay>
    <source src="video.mp4" type="video/mp4">
</video>
```

## Loop Attribute

Enable video looping for continuous playback with the `loop` attribute.

```html

<video loop>
    <source src="video.mp4" type="video/mp4">
</video>
```

## Muted Attribute

Control the audio by muting it using the `muted` attribute.

```html

<video muted>
    <source src="video.mp4" type="video/mp4">
</video>
```

## Poster Attribute

Enhance visual appeal by adding a poster image that displays before the video starts.

```html

<video poster="video-poster.jpg">
    <source src="video.mp4" type="video/mp4">
</video>
```

## Dimensions: Width and Height

Adjust the dimensions of the video player for optimal display on your webpage.

```html

<video width="800" height="450">
    <source src="video.mp4" type="video/mp4">
</video>
```

## Introduction to Audio

Transition to audio elements, understanding how to embed and customize audio playback.

```html

<audio controls>
    <source src="audio.mp3" type="audio/mp3">
</audio>
```

## Looping Audio

Implement audio looping for repetitive playback using the `loop` attribute.

```html

<audio controls loop>
    <source src="audio.mp3" type="audio/mp3">
</audio>
```

## Repeat Feature for MP3

Explore the repeat feature specifically for MP3 audio files.

```html

<audio controls>
    <source src="audio.mp3" type="audio/mp3" loop>
</audio>
```

## Preload Attribute

Optimize the loading experience with the `preload` attribute, determining when to load media files.

### Different Types of Preload Attribute

The `preload` attribute comes with different values to control how the browser loads the media:

- **`auto`:** The default value. The browser decides when and what to preload.
- **`metadata`:** Preloads only metadata, such as duration and dimensions.
- **`none`:** Disables preloading.

```html

<video preload="auto">
    <source src="video.mp4" type="video/mp4">
</video>
```

Get ready to master multimedia integration in HTML, unlocking the potential to create dynamic and engaging web pages
with seamlessly embedded videos and audio elements.