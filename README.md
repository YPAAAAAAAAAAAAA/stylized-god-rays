# God Rays

A single full-bleed WebGL scene: an after-school classroom at sunset. Warm shafts come through the window panes, land on the floor and the desks, and pick out the dust in the air.

This post plays that one effect. There is no menu, carousel, or debug panel.

## Credit

The shot, the sunset grade, and the window-light idea come from [cortiz2894/stylized-components](https://github.com/cortiz2894/stylized-components) (`/god-rays`), MIT © Christian Ortiz (Cortiz). See `LICENSE`.

The published scene is a procedural classroom (boxes, window openings, dust points, and layered light sheets). It does not ship the upstream classroom model.

## Play

`play.html` auto-starts a WebGL2 scene (no WebGPU) inside the phone frame. Drag to look around the shot.

## iPhone WebGL

- Renderer is WebGL2 only. There is no WebGPU path.
- The drawing buffer is 1:1 with the iframe, so the first frame stays cheap on a phone GPU.
- Touch drag turns the view. There is no pointer lock, keyboard shortcut, or fullscreen gate.
- Nothing fetches a texture. A failed image, if one were added, would paint black and would not show a broken-image mark.
