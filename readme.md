# DoodlePad
> good doodle pad

A simple doodle pad to use with canvas contexes

## Demo
[demo](https://brecert.github.io/doodlepad/)

## Notes

Make sure the canvas container has this css applied to it

```
touch-action: none;
```

to prevent strokes from being mis-inputed and cancelled

## Example
```js
import { PaintingContext } from 'https://unpkg.com/doodlepad'

const canvas = document.createElement('canvas')
canvas.width = window.innerWidth
canvas.height = window.innerHeight

const ctx = canvas.getContext('2d')
const paint = new PaintingContext(ctx)

paint.strokeSize = 5
paint.strokeSmoothing = 0.5

document.body.appendChild(canvas)
```