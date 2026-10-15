<div align="center">

# Black Hole: Beura Observatory

### Explore the extreme physics of a black hole, right in your browser.

An interactive black hole simulation designed to stay responsive on low-end PCs and mobile devices. Explore a glowing accretion disk, gravitational lensing, the event-horizon shadow, photon paths, black-hole mass and spin, and gravitational time dilation — without installing an app.

<p>
  <a href="https://blackhole-pocket.vercel.app">
    <img src="https://img.shields.io/badge/LAUNCH_BLACK_HOLE-Open_the_live_simulation-F0B368?style=for-the-badge&logo=vercel&logoColor=111111" alt="Launch the Black Hole interactive simulation" />
  </a>
</p>

<p>
  <strong><a href="https://blackhole-pocket.vercel.app">blackhole-pocket.vercel.app ↗</a></strong>
</p>

<p>
  <img src="https://img.shields.io/badge/Rendering-WebGL-7C9BE8?style=flat-square" alt="WebGL rendering" />
  <img src="https://img.shields.io/badge/Performance-Adaptive_quality-36A889?style=flat-square" alt="Adaptive render quality" />
  <img src="https://img.shields.io/badge/Interface-Mobile_friendly-E5A85B?style=flat-square" alt="Mobile-friendly controls" />
  <img src="https://img.shields.io/badge/Build-Single_HTML_file-6F7B8A?style=flat-square" alt="Single HTML file" />
</p>

</div>

---

## What is Black Hole: Beura Observatory?

**Black Hole: Beura Observatory** is a lightweight, browser-based black hole simulator and educational astronomy experience. It lets you manipulate an illustrative black hole system and see how mass, spin, viewing angle, observer distance, and accretion-disk properties influence the scene.

The simulation uses WebGL shaders to render a dynamic star field, a dark central shadow, a luminous accretion disk, and gravitational-lensing-inspired optical effects. It also includes scientific readouts and small learning labs for photon trajectories and gravitational time dilation.

It is designed as an interactive learning and visualisation tool, not as a replacement for observational data or a full general-relativistic research code.

## Highlights

- **Interactive black hole simulation:** Rotate the view, change inclination, and zoom toward or away from the black hole.
- **Accretion disk controls:** Adjust disk radius, brightness, density, temperature, and animation speed.
- **Black hole parameters:** Explore mass over several orders of magnitude and adjust the dimensionless spin parameter in the model.
- **Gravitational lensing mode:** Emphasise the distortion of background light around the black-hole shadow.
- **Scientific overlay:** Inspect schematic markers for the shadow, innermost stable circular orbit (ISCO), outer disk edge, and spin axis.
- **Photon-ray lab:** Adjust the photon impact parameter and observe whether the modelled ray escapes or is captured.
- **Gravitational time-dilation lab:** Explore the Schwarzschild relation for a static clock outside the event horizon.
- **Astronomy presets:** Switch between illustrative stellar-mass and supermassive cases, Sgr A*-inspired and M87*-inspired settings, an extreme-spin case, and a disk-free view.
- **Learning panel:** Read concise explanations of the event horizon, photon sphere, black-hole shadow, ISCO, lensing, Doppler beaming, and the model’s limits.
- **No installation required:** Open the live simulation in a modern browser.

## Built for smoother performance

A visually rich simulation should not demand a high-end graphics card just to be usable. The renderer includes adjustable quality presets and an adaptive quality step-down when frame timing stays slow.

| Setting | Intended use |
| --- | --- |
| **Low** | Start here on entry-level phones, integrated graphics, or older laptops |
| **Balanced** | A practical default between detail and responsiveness |
| **High** | More rendering detail on capable devices |
| **Ultra** | Highest available preset for devices with additional graphics headroom |

The simulation caps its internal rendering scale relative to the device pixel ratio, and its quality controls trade image detail for rendering workload. Actual performance varies with browser, GPU, screen resolution, thermal conditions, and other running apps. For the smoothest experience on a low-end device, begin with **Low** or **Balanced**.

If WebGL is unavailable, the app displays a static 2D impression instead of the live shader-rendered scene.

## Controls

- **Mouse or one-finger drag:** Orbit the view.
- **Mouse wheel or pinch:** Zoom.
- **Arrow keys:** Rotate the view.
- **+ / −:** Zoom in or out.
- **R:** Reset the view.
- **1–5:** Switch visual modes.
- **Escape:** Exit Deep Space mode.

On small screens, use the panel buttons along the bottom edge to access controls, data, labs, and learning notes.

## Physics and scientific scope

The app combines interactive visualisation with selected equations and approximations, including:

- Schwarzschild radius: `Rs = 2GM/c²`
- Schwarzschild gravitational time dilation for a static clock outside the horizon
- The Schwarzschild photon-sphere radius and approximate shadow scale
- A spin-dependent ISCO calculation
- A simplified photon-ray integration lab and disk-emission colour model

**Important limitation:** this is an educational, Schwarzschild-inspired visual model with a frame-dragging-inspired twist. It is **not** a full Kerr geodesic ray tracer, and its accretion-disk imagery is not a real telescope observation. Presets described as “inspired” are approximate visual starting points, not exact reproductions of observed systems. Read the in-app “What this model is” note for more detail.

## Technology

- Single-file HTML application
- CSS and vanilla JavaScript
- WebGL and GLSL shaders for the main real-time scene
- Canvas 2D for the scientific overlay and WebGL fallback
- Pointer, touch, wheel, and keyboard interaction
- No framework or package installation required

## Run locally

1. Download or clone this repository.
2. Open `index.html` in a modern browser.
3. For the full animated scene, use a browser with WebGL enabled.

The simulation is self-contained in `index.html`; no build step or package installation is required.

## Live deployment

The production experience is hosted on Vercel:

**[Open Black Hole: Beura Observatory](https://blackhole-pocket.vercel.app)**

The live deployment is intended for desktop, tablet, and mobile browsers. If you experience low frame rates, switch the render quality to Low or Balanced.

## License

This project is proprietary. All rights are reserved; no reuse, redistribution, or derivative-work licence is granted by default. See [LICENSE](LICENSE) for the terms.

---

<p align="center">
  <sub>Built by Satyajit Beura · Beura Observatory</sub>
</p>
