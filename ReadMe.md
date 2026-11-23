# 360° Image & Video Viewer

A lightweight, browser-based viewer for 360-degree images and videos. No additional setup required, just open the HTML file in any modern browser.


<div align="left">
 <img src="examples/example_image.png" width="710px">
</div>

Try it out here: https://progamergov.github.io/html-360-viewer

Supports:

* 360° panoramic **images**, most formats supported by browsers, like [JPEG](https://en.wikipedia.org/wiki/JPEG) (includes '.jpg'), [PNG](https://en.wikipedia.org/wiki/PNG), [WebP](https://en.wikipedia.org/wiki/WebP), etc.
* 360° **videos** in [.mp4](https://en.wikipedia.org/wiki/MP4_file_format) and [.webm](https://en.wikipedia.org/wiki/WebM) format. Works as a 360 video player.
* Monoscopic 360 images and stereo images in **top-bottom** and **left-right** layouts


## 🧪 Compatibility

Works on all major web browsers that [A-Frame](https://aframe.io/docs/1.8.0/introduction/faq.html) supports.

* [Firefox](https://en.wikipedia.org/wiki/Firefox)
* [Chrome](https://en.wikipedia.org/wiki/Google_Chrome) (including Chromium based browsers like [Brave](https://en.wikipedia.org/wiki/Brave_(web_browser)) & [Opera](https://en.wikipedia.org/wiki/Opera_(web_browser)))
* [Microsoft Edge](https://en.wikipedia.org/wiki/Microsoft_Edge)
* [Safari](https://www.apple.com/ca/safari/)

Works on [all VR headsets supported by A-Frame](https://aframe.io/docs/1.8.0/introduction/vr-headsets-and-webxr-browsers.html).

* [Meta Quest](https://en.wikipedia.org/wiki/Meta_Quest) (all versions)
* [Valve Index](https://en.wikipedia.org/wiki/Valve_Index)
* [HTC Vive](https://en.wikipedia.org/wiki/HTC_Vive)
* [Vive Focus](https://en.wikipedia.org/wiki/HTC_Vive)
* [Apple Vision Pro](https://en.wikipedia.org/wiki/Apple_Vision_Pro)
* [Oculus Go](https://en.wikipedia.org/wiki/Oculus_Go)
* [Oculus Rift](https://en.wikipedia.org/wiki/Oculus_Rift)

## 🚀 Features

* **Drag & Drop** support for instant media viewing
* **Stereo toggle** switch between monoscopic and stereo images (mono/top-bottom/side-by-side)
* **Zooming** via mouse wheel or pinch gesture
* **Interactive panning** with mouse or touch
* **Fullscreen** mode via the bottom right button. Opens in VR headset if supported.
* **Screenshot** functionality (UI hidden in capture)
* **Video controls**: play/pause, timeline slider


## 📦 Getting Started

**Option 1 – Local Use**

1. Download or clone this repository.
2. Open `viewer360.html` in your browser.
3. Drag and drop a supported 360° image or video file, or click "Select Media" to browse.

**Option 2 – Web Demo**

1. Visit the [live demo](https://progamergov.github.io/html-360-viewer) in your browser.
2. Upload a 360° image or video to start viewing.

**Option 3 – Local Copy**

1. Copy the full contents of `viewer360.html` into a new text file.
2. Rename the file to something like `viewer360.html` (make sure it ends in `.html`).
3. Open it in your browser.


## 🕹️ Controls

| Action             | How to Use                                   |
| ------------------ | -------------------------------------------- |
| Pan View           | Left-click + drag or touch + drag            |
| Zoom               | Mouse wheel or pinch gesture                 |
| Fullscreen         | Browser fullscreen and VR headset control    |
| Stereo Toggle      | Bottom-left "Stereo" button                  |
| Screenshot         | Camera icon at bottom center                 |
| Upload/Reset Media | "Upload" button below controls               |
| Play/Pause Video   | Play/pause button on video controls          |
| Seek in Video      | Use the timeline slider                      |


## 🔗 URL Parameters

Media can be loaded directly from an external URL by passing **hash parameters** after the `#` in the viewer URL. This only works when the viewer is hosted on a local or remote web server (it does not work when the file is opened directly from disk).

Links created before the switch that pass query parameters (`?url=...`, `?stereo=...`) still work: those parameters are moved into the hash automatically.

| Parameter      | Description                                                 | Values                                                                                            |
| -------------- | ----------------------------------------------------------- | ------------------------------------------------------------------------------------------------- |
| `url` or `src` | Direct link to the media to load (image or MP4/WebM video)  | Any valid media URL                                                                               |
| `stereo`       | Stereo viewing mode to use when loading an image            | `0` monoscopic (default), `1` or `tb`/`vertical` for top/bottom, `2` or `lr`/`horizontal` for left/right |

**Example**

```
https://progamergov.github.io/html-360-viewer#url=https://example.com/example_image.jpg&stereo=1
```


## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.


## 🔬 Citation

If you use this library in your research or project, please refer to the included [CITATION.cff](CITATION.cff) file or cite it as follows:

### BibTeX
```bibtex
@misc{egan2025html360viewer,
  title={Browser-Based Viewer for 360 Images and Videos},
  author={Egan, Ben},
  year={2025},
  publisher={GitHub},
  howpublished={\url{https://github.com/ProGamerGov/html-360-viewer}}
}
```

### APA Style
```
Egan, B. (2025). Browser-Based Viewer for 360 Images and Videos [Computer software]. GitHub. https://github.com/ProGamerGov/html-360-viewer
```
