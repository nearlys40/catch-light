# Catchlight

A field guide to light for beginner photographers. It's an interactive site that shows what gear to use, where to put it, and how the light actually falls on a face.

Live site: https://nearlys40.github.io/catch-light/ (Thai) and https://nearlys40.github.io/catch-light/index-en.html (English)

## What's in it

- **Fundamentals** - four small labs: hard vs soft light, the inverse square law, light direction, and colour temperature.
- **Studio playground** - drag up to four lights and a reflector around a floor plan and see the result from the camera's position. You can change the modifier, power, height, feathering, Kelvin and gels. It tells you which portrait pattern you've made (loop, Rembrandt, split, butterfly and so on), and shows the lighting ratio, a histogram and a close-up of the catchlight in the eye.
- **Setup library** - 12 common setups, each with a diagram, gear list, steps and the mistakes people usually make. Any of them can be loaded straight into the playground.
- **Natural light** - move the sun through the day, try overcast and open shade, and play with window light.
- **Product lighting** - bright-field and dark-field for glass, strip lights, and why matte objects need a different approach.
- **Quiz and glossary** - guess the setup from a render, and look up terms.

## How it works

Everything is in one HTML file with no dependencies. The head is a 2.5D model: a generated depth map and normal map, shaded per pixel on a canvas. Large sources are sampled across their surface so shadows soften the way they should, light falls off with distance, and the catchlights are real reflections of the modifier's shape.

It's a simplified simulation. It's good for learning the principles, but it isn't physically exact.

## Running it

Open `index.html` in a browser. That's it. It works offline too.

There's a Thai version (`index.html`) and an English one (`index-en.html`), and you can switch between them from the top right corner.
