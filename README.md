# SphereOs

> A zero-build, drop-in 3D image sphere. Paste it into any page, add your photos, and go.

<img width="304" height="88" alt="Image" src="https://github.com/user-attachments/assets/ab9fcc2e-d83e-4fc2-b378-bbe1a4cdca67" />



---

## What is this?

SphereOs renders a sphere of floating image cards using Three.js. No bundler. No dependencies to install. One HTML file, one copy-paste, and it lives inside your hero section, portfolio, or gallery page with a transparent background.

<img width="1113" height="864" alt="Image" src="https://github.com/user-attachments/assets/50d0b5e0-3d89-445d-a3b5-f775bb015615" /> 




---

## Get your own component

1. Open the editor and adjust the **Sphere Radius** and **Rotation Speed** sliders to your liking.
2. Click the **copy button** (bottom-right on desktop, top-right on mobile).
3. Paste the copied code into any HTML file or framework.

> The values you set before copying are baked into the component as defaults. If you want a slower, wider sphere, set it first—then copy.

---

## Add your images

In the copied code, find the `CONFIG` object at the top:

```js
const CONFIG = {
    imageUrls: [
        // Add your image URLs here
    ],
    sphereRadius: 1.0,
    rotationSpeed: 0.05
};
```

Replace the comments with direct image URLs:

```js
imageUrls: [
    'https://your-cdn.com/photo-1.jpg',
    'https://your-cdn.com/photo-2.jpg',
    'https://your-cdn.com/photo-3.jpg'
]
```

## The Exact Prompt to Give your Coding agent
Paste this into Claude Code, Cursor, or any AI builder:
```md
I have a 3D sphere gallery with 64 card placeholders. The code has an "imageUrls" array in the "CONFIG" object. Replace the empty strings with these 64 image URLs: [paste your URLs here]. Keep the array format exactly as it is with commas and quotes.
```



The sphere has 64 cards. Images map in order—first URL to the first card, second to the second, and so on. Any cards without an image stay as clean white placeholders.

---

## Notes

- Images must be hosted online (HTTPS). Local paths only work if you are running a local dev server.
- The canvas is transparent by default, so your page background shows through.
- Drag to orbit. Scroll (or use the radius slider in the editor) to expand and contract the sphere.

---

## License

MIT

