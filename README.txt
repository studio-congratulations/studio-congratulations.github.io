
# Studio Congratulations | Creative Portfolio

A high-performance, video-first portfolio site designed to showcase 3D renders, character animations, and ComfyUI generative workflows. Hosted on GitHub Pages.

[🔗 View Live Portfolio](https://studio-congratulations.github.io/)

## 🎨 Focus Areas
- **3D Motion Design:** High-quality video renders (Cinematic 4D, Blender, etc.)
- **Generative AI:** Custom ComfyUI workflows and neural style transfers.
- **Character Animation:** Short-form loops and YouTube-embedded storytelling.

## 🛠️ Tech Stack
- **Frontend:** HTML5, CSS3 (Tailwind CSS)
- **Interactions:** Vanilla JavaScript (Data-driven grid)
- **Icons:** Lucide Icons
- **Deployment:** GitHub Pages

## 🚀 How to Add New Work
The site is built to be "dynamic" through a simple data array. You don't need to touch the HTML structure to add a new project.

1.  **Prepare your media:** 
    *   Upload 3D/Animation MP4s to the `/videos` folder.
    *   Upload thumbnails to the `/img` folder.
2.  **Update `index.html`:**
    Find the `const projects = [...]` array at the bottom of the file and add a new block:

```javascript
{
    title: "Project Name",
    category: "3d", // Options: '3d', 'animation', 'comfyui', 'youtube'
    thumbnail: "./img/my-thumbnail.jpg",
    videoUrl: "./videos/my-render.mp4", // Or YouTube ID
    isYouTube: false
}