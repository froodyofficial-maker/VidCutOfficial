# VidCut — Social Video Editor

A browser-first social video editor prototype built with HTML/CSS/JS.

## Updated editing controls
- Screen shake uses real screen movement in preview, with start/end intensity keyframes.
- Shake and zoom have editable graph curves. Drag the start/end graph points or use the sliders.
- Zoom has start/end scale keyframes.
- Transition layers replace the old `+` cut button. Add a layer, move the playhead to a cut, select the layer, then click a transition preset.
- The timeline playhead is draggable by clicking/dragging anywhere on the timeline.
- `Shift + D` splits the clip at the current playhead.
- CC presets remain previewable.
- MP4 export remains browser-based through FFmpeg.wasm.

## GitHub Pages
Push the contents of this folder to a repository and enable **Settings → Pages → Deploy from branch**.

For local development:

```bash
python -m http.server 4173
```

Then visit `http://localhost:4173`.

FFmpeg.wasm is loaded from jsDelivr on export, so exporting needs internet access unless you self-host the FFmpeg assets.
