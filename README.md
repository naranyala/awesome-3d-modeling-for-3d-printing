# Awesome 3D Modeling for 3D Printing [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A curated list of resources, tools, software, and utilities related to 3D modeling for 3D printing.

[**3D printing**](https://en.wikipedia.org/wiki/3D_printing) is the construction of a three-dimensional object from a CAD model or a digital 3D model. This list focuses on **3D modeling tools, software, and resources** useful for creating models intended for 3D printing.

**Contributing:** Please read the [contribution guidelines](#contribute) before adding resources.

---

## Contents

- [3D Printing Technologies](#3d-printing-technologies)
- [CAD Software](#cad-software)
  - [Free & Open Source](#free--open-source)
  - [Commercial & Professional](#commercial--professional)
  - [Cloud-Based & Collaborative](#cloud-based--collaborative)
  - [Code-Driven & Parametric](#code-driven--parametric)
  - [Beginner-Friendly](#beginner-friendly)
- [Sculpting & Mesh Editing](#sculpting--mesh-editing)
- [Mesh Repair & Optimization](#mesh-repair--optimization)
- [AI-Powered 3D Generation](#ai-powered-3d-generation)
- [Slicers](#slicers)
  - [FDM Slicers](#fdm-slicers)
  - [Resin Slicers](#resin-slicers)
- [3D Scanning & Photogrammetry](#3d-scanning--photogrammetry)
- [Topology Optimization & Generative Design](#topology-optimization--generative-design)
- [Lattice & Infill Design](#lattice--infill-design)
- [Model Analysis & Printability Checkers](#model-analysis--printability-checkers)
- [Parametric Model Libraries & Component Generators](#parametric-model-libraries--component-generators)
- [File Formats](#file-formats)
- [Online 3D Model Repositories](#online-3d-model-repositories)
  - [Community-Driven (Free)](#community-driven-free)
  - [Marketplaces (Free & Paid)](#marketplaces-free--paid)
  - [Engineering-Focused](#engineering-focused)
  - [Self-Hostable](#self-hostable)
  - [Search Engines](#search-engines)
- [Online Tools & Utilities](#online-tools--utilities)
- [Design Guidelines](#design-guidelines)
- [Developer Tools & Automation](#developer-tools--automation)
- [Learning Resources](#learning-resources)
  - [Books](#books)
  - [YouTube Channels](#youtube-channels)
  - [Courses & Tutorials](#courses--tutorials)
- [Communities & Forums](#communities--forums)
- [Related Awesome Lists](#related-awesome-lists)

---

## 3D Printing Technologies

| Technology | Process | Materials | Layer Height | Accuracy | Surface Finish | Cost Range | Typical Applications |
|------------|---------|-----------|--------------|----------|----------------|------------|---------------------|
| **FDM** (Fused Deposition Modeling) | Extruded thermoplastic filament | PLA, PETG, ABS, ASA, Nylon, TPU, PC, PEEK | 0.05–0.4 mm | ±0.3 mm (<100 mm); ±0.3% (larger) | Medium (visible layer lines) | $150–$5,000+ (desktop); $5,000–$50,000+ (industrial) | Prototypes, functional parts, education, tooling |
| **SLA** (Stereolithography) | UV laser cures photopolymer resin | Standard, Tough, Flexible, Castable, Dental resins | 0.01–0.1 mm | ±0.1 mm | High (smooth surface) | $200–$3,000 (desktop); $3,000–$15,000+ (professional) | Miniatures, dental, jewelry, visual models, molds |
| **DLP** (Digital Light Processing) | Projected UV light cures entire layer | Photopolymer resins (same as SLA) | 0.01–0.05 mm | ±0.05–0.1 mm | High (smooth surface) | $200–$5,000 | Similar to SLA; faster for full-layer prints |
| **LCD / mSLA** (Masked SLA) | UV LCD screen cures resin layer | Standard and specialty resins | 0.01–0.05 mm | ±0.05–0.1 mm | High | $150–$1,500 | Entry-level resin printing, miniatures |
| **SLS** (Selective Laser Sintering) | Laser sinters powder bed | Nylon (PA11, PA12), TPU, glass/carbon-filled nylon | 0.06–0.15 mm | ±0.2 mm | Medium-high (slightly grainy) | $10,000–$100,000+ | Functional prototypes, small series, enclosures |
| **MJF** (Multi Jet Fusion) | Fusing agent + infrared energy on powder bed | Nylon PA12, PA11, glass-filled nylon | 0.08 mm | ±0.2 mm | Medium-high | $15,000–$130,000+ | End-use parts, functional housings, tooling |
| **SLM / DMLS** (Selective Laser Melting / Direct Metal Laser Sintering) | Laser melts metal powder | Stainless steel, titanium, aluminum, Inconel, cobalt chrome | 0.02–0.06 mm | ±0.1–0.2 mm | Medium (requires post-machining for tight tolerances) | $50,000–$500,000+ | Aerospace, medical implants, tooling, metal components |
| **Material Jetting (PolyJet)** | UV-cured photopolymer droplets | Photopolymers (rigid, flexible, transparent, biocompatible) | 0.014–0.03 mm | ±0.1–0.2 mm | Very high | $50,000–$500,000+ | Multi-material/color prototypes, visual models, medical |
| **Binder Jetting** | Liquid binder on powder bed | Sand (molding), metal (sintered), gypsum (full-color) | 0.1 mm | ±0.2–0.5 mm | Medium (porous; requires infiltration) | $10,000–$500,000+ | Sand casting molds, metal parts, full-color models |

---

## CAD Software

### Free & Open Source

| Tool | License | Platforms | File Formats | Repository | Stars (approx.) | Last Updated | Description |
|------|---------|-----------|--------------|------------|-----------------|--------------|-------------|
| [**FreeCAD**](https://www.freecad.org/) | LGPL-2.1 | Win / Mac / Linux | STEP, IGES, STL, OBJ, SVG, DXF, FCStd | [GitHub](https://github.com/FreeCAD/FreeCAD) | 18k+ | Active | Parametric 3D CAD modeler with workbench architecture; supports engineering simulation (FEM), CNC path generation, and 2D drafting |
| [**OpenSCAD**](https://www.openscad.org/) | GPL-2.0 | Win / Mac / Linux | STL, OFF, AMF, 3MF, DXF, SVG | [GitHub](https://github.com/openscad/openscad) | 8k+ | Active | Script-based solid 3D CAD modeller; uses CSG (Constructive Solid Geometry); deterministic and reproducible modeling |
| [**Blender**](https://www.blender.org/) | GPL-3.0 | Win / Mac / Linux | STL, OBJ, FBX, GLTF, PLY, 3MF, BLEND | [GitHub](https://projects.blender.org/blender/blender) | N/A | Active | 3D creation suite; mesh, sculpt, curve, and geometry nodes; 3D Print Toolbox add-on for mesh analysis; not parametric |
| [**SolveSpace**](https://solvespace.com/) | GPL-3.0 | Win / Mac / Linux | STEP, STL, SVG, DXF | [GitHub](https://github.com/solvespace/solvespace) | 4.5k+ | Active | Parametric 2D/3D CAD; constraint-based sketcher; linkage and mechanism simulation; lightweight (~30 MB) |
| [**build123d**](https://github.com/gumyr/build123d) | MIT | Cross-platform (Python) | STEP, STL, 3MF, SVG | [GitHub](https://github.com/gumyr/build123d) | 600+ | Active | Python CAD library built on OpenCASCADE; fluent API for parametric part design; exports to STL/STEP |
| [**CadQuery**](https://github.com/CadQuery/cadquery) | Apache-2.0 | Cross-platform (Python) | STEP, STL, AMF, 3MF, SVG | [GitHub](https://github.com/CadQuery/cadquery) | 3.5k+ | Active | Python-based parametric CAD library; scriptable modeling with OpenCASCADE kernel; integrates with Jupyter notebooks |
| [**SDF**](https://github.com/fogleman/sdf) | MIT | Cross-platform (Python) | STL, OFF, OBJ | [GitHub](https://github.com/fogleman/sdf) | 2k+ | Active | Python library for generating Signed Distance Fields (SDFs); useful for implicit modeling and 3D printing |
| [**Truck**](https://truck.rs/) | Apache-2.0 / MIT | Rust / WASM | STEP, STL, IGES | [GitHub](https://github.com/truck-rs/truck) | 1k+ | Active | 3D CAD kernel in Rust; boundary representation (B-Rep), mesh processing, and STEP file I/O; experimental browser CAD |

### Commercial & Professional

| Tool | License | Platforms | File Formats | Pricing | Description |
|------|---------|-----------|--------------|---------|-------------|
| [**Autodesk Fusion 360**](https://www.autodesk.com/products/fusion-360/) | Commercial (subscription) | Win / Mac | STEP, IGES, STL, OBJ, FBX, SMT, F3D | Free (personal/hobbyist, < $400/yr revenue); Paid (commercial: ~$600/yr) | Cloud-based CAD/CAM/CAE; parametric, direct, mesh, surface modeling; simulation, rendering, toolpath generation |
| [**SolidWorks**](https://www.solidworks.com/) | Commercial (perpetual/subscription) | Windows | STEP, IGES, STL, OBJ, 3MF, SLDPRT, SLDASM | ~$4,500 (perpetual) + $1,300/yr (maintenance); Student: ~$99/yr | Parametric solid modeling; assemblies, drawings, simulation; widely used in mechanical engineering education and industry |
| [**Autodesk Inventor**](https://www.autodesk.com/products/inventor/) | Commercial (subscription) | Windows | STEP, IGES, STL, OBJ, IPT, IAM | ~$2,100/yr | 3D mechanical design; sheet metal, frame generator, tube & pipe; integrated with AutoCAD |
| [**Rhinoceros 3D (Rhino)**](https://www.rhino3d.com/) | Commercial (perpetual) | Win / Mac | 3DM, STEP, IGES, STL, OBJ, FBX, DWG, DXF | $995 (commercial); $195 (student) | NURBS-based modeling; freeform surfaces; Grasshopper for visual scripting/parametric design; used in architecture, jewelry, industrial design |
| [**AutoCAD**](https://www.autodesk.com/products/autocad/) | Commercial (subscription) | Win / Mac | DWG, DXF, DWF, STL, OBJ, 3DS | ~$1,955/yr | 2D drafting and 3D modeling; architectural and engineering applications; parametric constraints |
| [**Shapr3D**](https://www.shapr3d.com/) | Commercial (subscription) | iPad / Win / Mac | STEP, IGES, STL, OBJ, 3MF, SHAPR | Free (2 documents, low-res export); Paid: ~$300/yr | Parasolid kernel; Apple Pencil/stylus support; direct modeling; Siemens engine; optimized for tablet workflows |
| [**Plasticity**](https://plasticity.xyz/) | Commercial (perpetual) | Win / Mac | STEP, OBJ, STL, FBX | ~$299 (one-time) | CAD for concept design; boolean workflows, fillets/chamfers, non-destructive history; targets artists and designers |
| [**Siemens NX**](https://www.sw.siemens.com/en-US/products/nx/) | Commercial (subscription) | Win / Linux | STEP, IGES, JT, STL, Parasolid | ~$10,000+/yr | Integrated CAD/CAM/CAE; synchronous technology; surfacing, assembly, simulation; used in automotive and aerospace |
| [**Creo Parametric**](https://www.ptc.com/en/products/creo) | Commercial (subscription) | Windows | STEP, IGES, STL, OBJ, PRT, ASM | ~$2,400/yr (license); ~$900/yr (maintenance) | Parametric and direct modeling; simulation, additive manufacturing, NC toolpaths; formerly Pro/ENGINEER |
| [**Solid Edge**](https://www.sw.siemens.com/en-US/products/solid-edge/) | Commercial (subscription) | Windows | STEP, IGES, STL, OBJ, Parasolid | Free (Community Edition, < $1M revenue); Paid (commercial: ~$2,500/yr) | Synchronous technology for parametric + direct modeling; sheet metal, welding, piping |
| [**ZBrush**](https://www.maxon.net/en/zbrush) | Commercial (perpetual/subscription) | Win / Mac | STL, OBJ, FBX, PLY, ZTL | $895 (perpetual); $360/yr (subscription) | Digital sculpting; high-poly models (millions of polygons); dynamesh, ZRemesher; used for characters, organic forms, miniatures |
| [**Cinema 4D**](https://www.maxon.net/en/cinema-4d) | Commercial (subscription) | Win / Mac | STL, OBJ, FBX, GLTF, C4D | ~$720/yr | 3D modeling, animation, rendering; MoGraph module; used in motion graphics and visualization |

### Cloud-Based & Collaborative

| Tool | License | Platforms | Pricing | Description |
|------|---------|-----------|---------|-------------|
| [**Onshape**](https://www.onshape.com/) | Commercial (subscription) | Browser / iOS / Android | Free (public documents); Paid: ~$1,500/yr | Full-cloud CAD; real-time multi-user editing; built-in PDM; FeatureScript for custom features; created by SolidWorks founders |
| [**Vectary**](https://www.vectary.com/) | Commercial (subscription) | Browser | Free (1 project); Paid: ~$20/mo | Browser-based 3D modeling with AR preview; real-time rendering; collaborative; targets web/AR design |
| [**Clara.io**](https://clara.io/) | Free / Commercial | Browser | Free | Cloud-based 3D modeling, animation, and rendering; supports V-Ray; collaborative editing |
| [**Fusion 360 Web**](https://www.autodesk.com/products/fusion-360/) | Commercial (subscription) | Browser | Free (limited features); Same as desktop | Browser-based viewer and editor; limited compared to desktop app but runs in browser |

### Code-Driven & Parametric

| Tool | Language | Kernel | Description |
|------|----------|--------|-------------|
| [**OpenSCAD**](https://www.openscad.org/) | OpenSCAD language | CGAL / Manifold | Declarative CSG modeling; parametric via variables and modules; reproducible builds |
| [**CadQuery**](https://github.com/CadQuery/cadquery) | Python | OpenCASCADE | Fluent API for building parametric models; scriptable; Jupyter integration |
| [**build123d**](https://github.com/gumyr/build123d) | Python | OpenCASCADE | Pythonic API for solid modeling; algebraic operations; integrates with OCP |
| [**DeclaraCAD**](https://declarecad.com/) | Python + Enaml | OpenCASCADE | GUI-based code CAD; parametric modeling with Python scripts |
| [**SDF (Python)**](https://github.com/fogleman/sdf) | Python | N/A (SDF generation) | Implicit modeling via signed distance functions; mesh export |

### Beginner-Friendly

| Tool | Platforms | Cost | Export Formats | Description |
|------|-----------|------|----------------|-------------|
| [**Tinkercad**](https://www.tinkercad.com/) | Browser | Free | STL, OBJ, SVG, GLB | Browser-based; shape grouping, hole tool, alignment; Codeblocks for programmatic design; integrates with Thingiverse |
| [**SketchUp Free**](https://app.sketchup.com/) | Browser | Free (web); Pro: ~$300/yr | SKP, STL (Pro), PNG | Push/pull modeling; 3D Warehouse library; extensions (Pro); used in architecture and woodworking |
| [**3D Slash**](https://www.3dslash.net/) | Browser / Win / Mac / Linux | Free; Paid: ~$24/yr | STL, OBJ, PLY | Block-based modeling (voxel-like); Minecraft-inspired interface; designed for education |
| [**SelfCAD**](https://www.selfcad.com/) | Browser | Free (limited); Paid: ~$19.99/mo | STL, OBJ, 3MF | All-in-one modeling + slicing; guided tutorials; targets beginners and intermediate users |

---

## Sculpting & Mesh Editing

| Tool | License | Platforms | Pricing | Description |
|------|---------|-----------|---------|-------------|
| [**Blender**](https://www.blender.org/) | GPL-3.0 | Win / Mac / Linux | Free | Sculpt mode with dynamic topology; remesh; voxel remesh; multiresolution modifier; 3D Print Toolbox add-on |
| [**ZBrush**](https://www.maxon.net/en/zbrush) | Commercial | Win / Mac | Paid | DynaMesh, ZRemesher, NanoMesh, FiberMesh; up to billions of polygons; 3D print export and scale tools |
| [**Meshmixer**](https://www.meshmixer.com/) | Freeware (Autodesk) | Windows / Mac (discontinued, v3.5.0 final) | Free | Mesh sculpting, stamp brushes, make pattern tool; automatic repair, hollowing, support generation; no longer updated |
| [**3DCoat**](https://3dcoat.com/) | Commercial | Win / Mac / Linux | Paid (~$399) | Voxel-based sculpting; retopology tools; PBR texturing; 3D print preparation |
| [**Nomad Sculpt**](https://nomadsculpt.com/) | Commercial | iPad / Android | Paid (~$15 one-time) | Mobile sculpting; dynamic topology, boolean operations; export to STL/OBJ; optimized for tablet use |
| [**Mudbox**](https://www.autodesk.com/products/mudbox/) | Commercial | Win / Mac | Paid (subscription) | Digital sculpting and texture painting; layer-based workflow; integrates with Maya/3ds Max |
| [**Sculptris**](https://pixologic.com/sculptris/) | Freeware (discontinued) | Win / Mac | Free | Simplified sculpting by Pixologic; predecessor to ZBrush Core; no longer developed |

---

## Mesh Repair & Optimization

| Tool | License | Platforms | Pricing | Supported Formats | Capabilities |
|------|---------|-----------|---------|-------------------|--------------|
| [**Meshmixer**](https://www.meshmixer.com/) | Freeware (Autodesk) | Windows / Mac | Free (discontinued, v3.5.4 final released 2024) | STL, OBJ | Auto-repair, hole filling, mesh analysis, inspector tool, make solid, reduce |
| [**MeshLab**](https://www.meshlab.net/) | GPL-3.0 | Win / Mac / Linux | Free | PLY, STL, OBJ, 3DS, COLLADA, X3D | Mesh cleaning, filter scripts, duplicate removal, hole closing, remeshing, simplification |
| [**FreeCAD (Mesh Workbench)**](https://www.freecad.org/) | LGPL-2.1 | Win / Mac / Linux | Free | STL, OBJ, Mesh formats | Mesh evaluation, repair, boolean with solids, convert to solid, fill holes |
| [**Blender (3D Print Toolbox)**](https://www.blender.org/) | GPL-3.0 | Win / Mac / Linux | Free | STL, OBJ, PLY, others | Mesh analysis: non-manifold edges, faces, overhangs, wall thickness, volume calculation |
| [**PrusaSlicer (Netfabb Repair)**](https://github.com/prusa3d/PrusaSlicer) | AGPL-3.0 | Win / Mac / Linux | Free | STL, OBJ, 3MF, AMF | Built-in netfabb repair engine on import; fixes non-manifold geometry, inverted normals |
| [**Netfabb**](https://www.autodesk.com/products/netfabb) | Commercial (Autodesk) | Windows | Included with Fusion 360 (Netfabb add-on) | STL, 3MF, AMF, STEP | Automatic repair, part nesting, support generation, simulation, lattice structures |
| [**Materialise Magics**](https://www.materialise.com/en/software/magics) | Commercial | Windows | Paid (enterprise quote) | STL, 3MF, STEP, IGES | Repair, support generation, slicing, build preparation, part nesting, sintering compensation |
| [**LimitState:FIX**](https://www.limitstate.com/) | Commercial | Windows | Paid (~£25/mo) | STL, OBJ | Automatic repair of bad STLs; non-manifold, self-intersection, inverted normals |
| [**MeshInspector**](https://meshinspector.com/) | Commercial | Web / Win / Mac / Linux | Free (basic); Paid ($9.99+/mo) | STL, OBJ, 3MF | Auto-repair, manual mesh editing, measurement, wall thickness analysis |
| [**Microsoft 3D Builder**](https://apps.microsoft.com/store/detail/3d-builder/9wzdncrfj3t6) | Freeware | Windows 10/11 | Free | STL, OBJ, PLY, 3MF, FBX, GLB | One-click repair; scale, rotate, split models; basic 3D print preparation |
| [**Formware STL Repair**](https://formware.co/) | Freeware | Browser | Free | STL | Web-based upload and repair; identifies unclosed shells and non-manifold edges |
| [**Admesh**](https://github.com/admesh/admesh) | GPL-2.0 | Linux / Mac (CLI) | Free | STL | Command-line STL analyzer and repair; finds and fixes bad facets, degenerate faces |
| [**JustFixSTL**](https://www.justfixstl.com/) | Freeware | Browser | Free | STL, OBJ, PLY | Online mesh repair; fixes non-manifold edges, normals, holes; no upload required |

---

## AI-Powered 3D Generation

| Tool | Input Types | Output Formats | Pricing | Platform | Description |
|------|-------------|----------------|---------|----------|-------------|
| [**Meshy**](https://www.meshy.ai/) | Text prompt, single image | GLB, FBX, OBJ, STL | Free (credits/day); Paid: ~$24/mo | Web / API | Text-to-3D and image-to-3D; PBR texture generation; topology controls; generation in < 2 min |
| [**Tripo AI**](https://www.tripo3d.ai/) | Text prompt, single image | GLB, FBX, STL, OBJ | Free (600 credits/mo); Paid: ~$19/mo | Web / API | Text/image to 3D in ~8 seconds; 2-min refinement mode; 100+ template categories |
| [**3D AI Studio**](https://www.3daistudio.com/) | Text prompt, single/multi-view image | GLB, OBJ, FBX, STL | Free (limited); Paid: ~$29/mo | Web | Image-to-3D with multi-view support; texture refinement; API available |
| [**MakerWorld Image to 3D**](https://makerworld.com/) | Single image (PNG/JPEG) | 3MF (Bambu-ready) | Free (10 exports/mo via Bambu account) | Web (MakerLab) | Powered by Tripo AI; integrated with Bambu Studio; basic editing (rotation, scale, base) |
| [**Sloyd AI**](https://www.sloyd.ai/) | Text prompt, parameters | GLB, FBX, OBJ, STL | Free (limited); Paid: ~$9.99/mo | Web / API | Parametric hard-surface generation; clean topology; adjustable UV maps; game-ready assets |
| [**Luma AI Genie**](https://lumalabs.ai/genie) | Text prompt | GLB, OBJ | Free; Paid tiers | Web / iOS / Discord | Text-to-3D via Discord bot or web; high-fidelity results; NeRF and Gaussian Splatting support |
| [**CSM AI**](https://csm.ai/) | Single image, video | GLB, OBJ, FBX | Free (limited); Paid: ~$99/mo | Web / API | Image/video to 3D; cube-to-3D pipeline; targets game/AR asset creation |
| [**Alpha3D**](https://www.alpha3d.io/) | Single/multi-view image | GLB, OBJ | Paid (custom pricing) | Web / API | High-volume image-to-3D; batch processing; API for enterprise pipelines |
| [**Kaedim**](https://www.kaedim3d.com/) | Single image | FBX, OBJ | Paid (~$399+/mo) | Web | AI + human-reviewed output; targets game studios; clean topology, production-ready |
| [**Spline AI**](https://spline.design/ai) | Text prompt, image | GLB, SPLINE | Free (limited); Paid: ~$12/mo | Web | Text-to-3D within Spline editor; interactive 3D design; web embed support |
| [**Rodin (HyperHuman)**](https://hyperhuman.deemos.com/) | Text prompt, image | GLB, OBJ, FBX | Free (limited); Paid: ~$20/mo | Web | Text/image-to-3D; detailed geometry; PBR material support |

---

## Slicers

### FDM Slicers

| Tool | License | Platforms | Pricing | File Formats | Description |
|------|---------|-----------|---------|--------------|-------------|
| [**Ultimaker Cura**](https://ultimaker.com/software/ultimaker-cura/) | LGPL-3.0 | Win / Mac / Linux | Free | STL, OBJ, 3MF, AMF, X3D, BMP, GIF, JPG, PNG | 400+ settings; support generation; Marketplace for plugins; 1M+ users; generates G-code for 70+ printer brands |
| [**PrusaSlicer**](https://github.com/prusa3d/PrusaSlicer) | AGPL-3.0 | Win / Mac / Linux | Free | STL, OBJ, 3MF, AMF, PRUSA | Forked from Slic3r; organic supports; multi-material; cut tool; configurable G-code; printer profiles for 200+ models |
| [**OrcaSlicer**](https://github.com/SoftFever/OrcaSlicer) | AGPL-3.0 | Win / Mac / Linux | Free | STL, OBJ, 3MF, AMF | Fork of PrusaSlicer/BambuStudio; sandpaper/patterned infill |
| [**BambuStudio**](https://github.com/bambulab/BambuStudio) | AGPL-3.0 | Win / Mac / Linux | Free | STL, OBJ, 3MF, AMF | Fork of PrusaSlicer; optimized for Bambu Lab printers; multi-process support; cloud printing integration |
| [**Slic3r**](https://slic3r.org/) | AGPL-3.0 | Win / Mac / Linux | Free | STL, OBJ, AMF, 3MF | Original open-source slicer; variable layer height; concentric infill; command-line interface; development slowed |
| [**Simplify3D**](https://www.simplify3d.com/) | Commercial | Win / Mac | Paid (~$199 one-time) | STL, 3MF, OBJ | Multi-process printing; advanced support structures; detailed G-code preview; no subscription model |
| [**Kiri:Moto**](https://grid.space/kirimoto/) | AGPL-3.0 | Browser | Free | STL, OBJ | Browser-based; supports FDM, SLA, CNC, laser; no installation required; uses Three.js for rendering |
| [**MatterControl**](https://mattercontrol.com/) | AGPL-3.0 | Win / Mac / Linux | Free | STL, OBJ, AMF, GCODE | Design + slice + print in one; built-in CAD tools; print queue management; MatterHackers integration |

### Resin Slicers

| Tool | License | Platforms | Pricing | Description |
|------|---------|-----------|---------|-------------|
| [**Chitubox**](https://www.chitubox.com/) | Commercial | Win / Mac / Linux | Free (basic); Paid: ~$179/yr | Leading resin slicer; hollowing, drainage holes, automatic/manual supports; anti-aliasing; supports 40+ printer brands |
| [**Lychee Slicer**](https://lychee3d.com/) | Commercial | Win / Mac / Linux | Free (basic); Paid: ~$120/yr | Automatic supports with island detection; resin validator; hollowing with wall thickness control; overhang detection |
| [**Voxeldance Tango**](https://www.voxeldance.com/) | Commercial | Windows | Paid (quote) | DLP/LCD slicing; nesting, support generation; volume printing optimization; targets industrial resin printing |
| [**Photon Workshop**](https://photonworkshop.com/) | Commercial | Win / Mac | Free | Elegoo's slicer for Mars/Saturn printers; manual support generation; hollowing; basic resin slicing |

---

## 3D Scanning & Photogrammetry

| Tool | License | Platforms | Pricing | Input | Output | Description |
|------|---------|-----------|---------|-------|--------|-------------|
| [**Polycam**](https://poly.cam/) | Commercial | iOS / Android / Web | Free (5 saves/mo); Paid: ~$70/yr | Photos, LiDAR, video | OBJ, GLB, STL, PLY, FBX | Mobile scanning app; LiDAR mode for iPhone/iPad Pro; photogrammetry mode for all devices; web viewer |
| [**RealityCapture**](https://www.capturingreality.com/) | Commercial (Epic Games) | Windows | Free (revenue < $1M/yr); Paid (revenue > $1M) | Photos, laser scans | OBJ, FBX, STL, PLY | Photogrammetry software; alignment, meshing, texturing; integrates with Unreal Engine |
| [**Meshroom**](https://alicevision.org/#meshroom) | MPL-2.0 | Win / Linux | Free | Photos | OBJ, FBX, STL | Open-source photogrammetry; AliceVision pipeline; node-based UI; requires NVIDIA GPU (CUDA) |
| [**Agisoft Metashape**](https://www.agisoft.com/) | Commercial | Win / Mac / Linux | Standard: ~$179; Professional: ~$3,499 | Photos, laser scans | OBJ, FBX, STL, PLY, DEM, Orthomosaic | Professional photogrammetry; dense cloud, DEM generation; georeferencing; batch processing |
| [**Pix4D**](https://www.pix4d.com/) | Commercial | Win / Mac | Paid (~$350/mo) | Drone imagery, photos | Point cloud, DSM, orthomosaic, 3D mesh | Survey-grade mapping; agriculture, construction, mining; cloud processing |
| [**3DF Zephyr**](https://www.3dflow.net/3df-zephyr-3d-reconstruction-software/) | Commercial | Windows | Free (50 photos/project); Paid: ~$299–$11,900 | Photos, video | OBJ, FBX, STL, PLY | Automatic 3D reconstruction; aerial photogrammetry support; free version limited to 50 images |
| [**Artec Studio**](https://www.artec3d.com/portable-3d-scanners-software/artec-studio-16) | Commercial | Windows | Paid (included with Artec scanners) | Structured light / laser scans | OBJ, STL, PLY, STEP | Professional 3D scanning software; mesh fusion, texture mapping; HD mode for fine detail |
| [**KIRI Engine**](https://www.kiriengine.com/) | Commercial | iOS / Android / Web | Free (5 exports/day); Paid: ~$5/mo | Photos | OBJ, STL, GLB | AI-assisted mobile scanning; mask tool; cloud processing |
| [**Qlone**](https://www.qlone.pro/) | Commercial | iOS / Android | Free (low-res); Paid: ~$5/export | Photos | OBJ, PLY, STL | Mobile 3D scanning; quick processing |
| [**Geomagic Design X**](https://www.3dsystems.com/software/geomagic-design-x) | Commercial | Windows | Paid (~$9,900 perpetual + $2,600/yr) | 3D scans (STL, PLY) | STEP, IGES, Parasolid | Scan-to-CAD reverse engineering; automatic surface extraction; mesh-to-solid conversion |
| [**Skanect**](https://skanect.manus.com/) | Commercial | Win / Mac | Free (limited); Paid: ~$490 | Structured light / depth cameras (Kinect, RealSense) | STL, OBJ, PLY, VRML | 3D scanning for body scanning, face scanning; watertight mesh export; coloring |

---

## Topology Optimization & Generative Design

| Tool | License | Platforms | Pricing | Description | Link |
|------|---------|-----------|---------|-------------|------|
| [**Autodesk Fusion 360 (Generative Design)**](https://www.autodesk.com/products/fusion-360/features/generative-design) | Commercial | Win / Mac | Included with Fusion 360 | Cloud-based generative design; defines loads/constraints, generates optimized geometry | [Website](https://www.autodesk.com/products/fusion-360/features/generative-design) |
| [**Solid Edge (Generative Design)**](https://solidedge.siemens.com/en/solutions/products/3d-design/next-generation-design/generative-design/) | Commercial | Windows | Included with Solid Edge | Topology optimization integrated with CAD; preserves design intent | [Website](https://solidedge.siemens.com/en/solutions/products/3d-design/next-generation-design/generative-design/) |
| [**ANSYS Discovery**](https://www.ansys.com/products/3d-design/ansys-discovery) | Commercial | Windows | ~$6,000/yr | Real-time simulation-driven design; topology optimization; generative exploration | [Website](https://www.ansys.com/products/3d-design/ansys-discovery) |
| [**nTopology (nTop)**](https://www.ntopology.com/) | Commercial | Windows | Quote-based | Implicit modeling; lattice structures; topology optimization; field-driven design | [Website](https://www.ntopology.com/) |
| [**3DXpert**](https://www.3dsystems.com/software/3dxpert) | Commercial | Windows | Quote-based | Topology optimization; lattice generation; support generation; slicing for AM | [Website](https://www.3dsystems.com/software/3dxpert) |
| [**Altair Inspire**](https://altair.com/inspire) | Commercial | Win / Mac | ~$5,000+ | Topology optimization, lattice generation, structure optimization | [Website](https://altair.com/inspire) |
| [**ToPy**](https://github.com/williamhunter/topy) | GPL-3.0 | Cross-platform (Python) | Free | Python-based topology optimization; open-source | [GitHub](https://github.com/williamhunter/topy) |

## Lattice & Infill Design

| Tool | License | Platforms | Pricing | Description | Link |
|------|---------|-----------|---------|-------------|------|
| [**nTopology (nTop)**](https://www.ntopology.com/) | Commercial | Windows | Quote-based | TPMS (gyroid, Schwarz D); variable-density lattices; field-driven thickness | [Website](https://www.ntopology.com/) |
| [**3DXpert**](https://www.3dsystems.com/software/3dxpert) | Commercial | Windows | Quote-based | Built-in lattice generation; skin-core lattice structures; conformal lattices | [Website](https://www.3dsystems.com/software/3dxpert) |
| [**Blender (Geometry Nodes)**](https://www.blender.org/) | GPL-3.0 | Win / Mac / Linux | Free | Procedural lattice generation; TPMS via math nodes; customizable patterns | [Website](https://www.blender.org/) |
| [**FreeCAD (Lattice2 Workbench)**](https://wiki.freecad.org/Part_Lattice2_Workbench) | LGPL-2.1 | Win / Mac / Linux | Free | Parametric lattice generation; boolean operations with lattices | [Wiki](https://wiki.freecad.org/Part_Lattice2_Workbench) |
| [**Rhino + Grasshopper (Pufferfish)**](https://www.rhino3d.com/) | Commercial | Win / Mac | Paid (~$995) | Visual scripting for lattice design; Pufferfish plugin for morphing lattices | [Website](https://www.rhino3d.com/) |
| [**OpenSCAD (Lattice Scripts)**](https://www.openscad.org/) | GPL-2.0 | Win / Mac / Linux | Free | Code-driven lattice generation via modules; customizable unit cells | [Website](https://www.openscad.org/) |
| [**Gyroid Infill Generator**](https://gyroid.inf) | Free | Browser | Free | Generates gyroid TPMS infill patterns for FDM slicing; customizable parameters | [Website](https://gyroid.inf) |
| [**Cubic Cubes (InFiLL)**](https://github.com/YetAnotherARS/InFiLL) | MIT | Cross-platform (Python) | Free | TPMS infill generator; gyroid, diamond, Schwein; exports to STL | [GitHub](https://github.com/YetAnotherARS/InFiLL) |

## Model Analysis & Printability Checkers

| Tool | License | Platforms | Pricing | Description | Link |
|------|---------|-----------|---------|-------------|------|
| [**Blender (3D Print Toolbox)**](https://www.blender.org/) | GPL-3.0 | Win / Mac / Linux | Free | Checks non-manifold geometry, overhangs, wall thickness, volume, surface area | [Website](https://www.blender.org/) |
| [**Netfabb (Analysis Tools)**](https://www.autodesk.com/products/netfabb) | Commercial | Windows | Included with Fusion 360 | Wall thickness, overhang, support volume, build simulation; deviation analysis | [Website](https://www.autodesk.com/products/netfabb) |
| [**Materialise Magics (Analysis)**](https://www.materialise.com/en/software/magics) | Commercial | Windows | Quote-based | Wall thickness, overhang, shrinkage compensation, support optimization | [Website](https://www.materialise.com/en/software/magics) |
| [**Meshmixer (Analysis)**](https://www.meshmixer.com/) | Freeware | Windows / Mac | Free | Overhang analysis; thickness map; stress visualization; support preview | [Website](https://www.meshmixer.com/) |

## Parametric Model Libraries & Component Generators

| Tool | Type | Platforms | Pricing | Description |
|------|------|-----------|---------|-------------|
| [**McMaster-Carr CAD Models**](https://www.mcmaster.com/) | Component library | Browser | Free | Standard hardware (screws, nuts, bearings); STEP format; design-ready |
| [**TraceParts**](https://www.traceparts.com/) | Component library | Browser | Free | Standard parts (fasteners, bearings, motors); CAD models in STEP, native formats |
| [**GrabCAD Community**](https://grabcad.com/library) | Model repository | Browser | Free | User-submitted CAD models; STEP, SLDPRT, native formats |
| [**Misumi CAD**](https://us.misumi-ec.com/) | Component library | Browser | Free | Standard mechanical components; configurable models; STEP download |
| [**BOSCH Rexroth eCatalog**](https://www.boschrexroth.com/) | Component library | Browser | Free | Linear motion, structural framing; CAD models for mechanical design |
| [**FreeCAD Library**](https://github.com/FreeCAD/FreeCAD-library) | Component library | FreeCAD | Free (via Addon Manager) | 1000+ parametric parts; fasteners, gears, bearings, structural shapes |
| [**MSC CADDock**](https://www.mscsoftware.com/) | Component library | Browser | Free | Engineering components; pulleys, springs, fasteners |

---

## File Formats

| Format | Extension | Type | Geometry | Color | Texture | Metadata | Open Standard | Primary Use |
|--------|-----------|------|----------|-------|---------|------------|---------------|-------------|
| **STL** | .stl | Mesh (triangles) | Yes | No | No | No | Yes (de facto) | Most common 3D printing format; surface geometry only |
| **OBJ** | .obj | Mesh (faces) | Yes | Via .mtl | Via .mtl | No | Yes | Multi-color printing; rendering; widely supported |
| **3MF** | .3mf | Package (XML-based) | Yes | Yes | Yes | Materials, print settings | Yes (3MF Consortium) | Modern 3D printing; full print job in one file |
| **STEP** | .step, .stp | B-Rep (parametric) | Yes | No | No | Features, constraints | Yes (ISO 10303) | CAD exchange between systems; preserves design history |
| **AMF** | .amf | XML-based mesh | Yes (curved triangles) | Yes | Yes | Materials, constellations | Yes (ASTM F42) | Successor to STL; supports lattice, color, materials |
| **PLY** | .ply | Mesh | Yes | Yes | Yes | Custom properties | Yes | 3D scanning; photogrammetry; point clouds |
| **FBX** | .fbx | Scene graph | Yes | Yes | Yes | Animation, hierarchy | No (Autodesk) | Game assets; animation; cross-application transfer |
| **GLB / glTF** | .glb, .gltf | JSON + binary | Yes | Yes | Yes (PBR) | Animation, skinning | Yes (Khronos) | Web 3D; AR/VR; real-time rendering |
| **DXF** | .dxf | Vector (2D/3D) | Yes | Yes | No | Layers, blocks | Yes (OpenDWG) | Laser cutting; 2D profiles; CNC |
| **IGES** | .iges, .igs | B-Rep / surface | Yes | No | No | No | Yes (ANSI) | Legacy CAD data exchange; being replaced by STEP |
| **X3D** | .x3d | XML-based scene | Yes | Yes | Yes | Animation | Yes (ISO/IEC) | Web 3D visualization; VRML successor |
| **USD / USDZ** | .usd, .usdz | Scene graph | Yes | Yes | Yes | Animation, variants | Yes (Pixar) | AR content; Pixar's Universal Scene Description |

---

## Online 3D Model Repositories

### Community-Driven (Free)

| Repository | Operator | Accounts Required | API | File Formats | Notable Features | Link |
|------------|----------|-------------------|-----|--------------|------------------|------|
| [**Printables**](https://www.printables.com/) | Prusa Research | Yes (free) | No (undocumented) | STL, 3MF, OBJ, GCODE | Pre-sliced files; rewards system; make/it made tracking; contests | [Website](https://www.printables.com/) |
| [**Thingiverse**](https://www.thingiverse.com/) | UltiMaker | Yes (free) | Yes (REST API) | STL, OBJ, PNG, GCODE | Largest free library; Codeblocks; Collections; MakerBot integration | [Website](https://www.thingiverse.com/) |
| [**MakerWorld**](https://makerworld.com/) | Bambu Lab | Yes (free) | No | STL, 3MF, OBJ, AMF, GCODE | Bambu Studio integration; AI image-to-3D; rewards; ~10M monthly active users | [Website](https://makerworld.com/) |
| [**Creality Cloud**](https://www.crealitycloud.com/) | Creality | Yes (free) | No | STL, 3MF, OBJ, GCODE | Cloud slicer; fleet management; model library | [Website](https://www.crealitycloud.com/) |
| [**YouMagine**](https://www.youmagine.com/) | UltiMaker | Yes (free) | No | STL, OBJ, 3MF | Open-source designs; CC-licensed models | [Website](https://www.youmagine.com/) |
| [**NIH 3D Print Exchange**](https://3dprint.nih.gov/) | National Institutes of Health | No | Yes (API) | STL, OBJ, PLY | Scientific/biomedical models; peer-reviewed submissions | [Website](https://3dprint.nih.gov/) |
| [**Smithsonian 3D**](https://3d.si.edu/) | Smithsonian Institution | No | No | OBJ, PLY, GLB | Digitized museum artifacts; open access | [Website](https://3d.si.edu/) |
| [**e-NABLE Community**](https://www.enablecommunity.org/) | e-NABLE | Yes (free) | No | STL | 3D-printed prosthetics; volunteer network | [Website](https://www.enablecommunity.org/) |
| [**NASA 3D Resources**](https://nasa3d.arc.nasa.gov/) | NASA | No | No | OBJ, STL, PLY, BLEND | Spacecraft, planetary, and rover models | [Website](https://nasa3d.arc.nasa.gov/) |

### Marketplaces (Free & Paid)

| Repository | Accounts Required | Commission | File Formats | Model Count | Notable Features | Link |
|------------|-------------------|------------|--------------|-------------|------------------|------|
| [**Cults3D**](https://cults3d.com/) | Yes (free to browse) | 20% to creator | STL, OBJ, 3MF, SVG, DXF, PNG, GCODE | 2.9M+ | Creator-focused; IP enforcement; no AI-generated model policy | [Website](https://cults3d.com/) |
| [**MyMiniFactory**](https://www.myminifactory.com/) | Yes (free) | 15–20% to creator | STL, OBJ, ZTL | 200k+ | Expert-tested guarantee; tabletop gaming focus; Patreon integration | [Website](https://www.myminifactory.com/) |
| [**CGTrader**](https://www.cgtrader.com/) | Yes (free) | 50–70% to creator | All major formats | 4M+ | Both printable and render models; AR viewer; B2B services | [Website](https://www.cgtrader.com/) |
| [**TurboSquid**](https://www.turbosquid.com/) | Yes (free) | 40–60% to creator | All major formats | 1.5M+ | Shutterstock subsidiary; royalty-free licensing; high-quality assets | [Website](https://www.turbosquid.com/) |
| [**Sketchfab**](https://sketchfab.com/) | Yes (free) | 70% to creator | GLB, GLTF, OBJ, FBX, STL | 1M+ 3D models | Epic Games subsidiary; 3D viewer with AR; scanning community | [Website](https://sketchfab.com/) |
| [**Free3D**](https://free3d.com/) | No (free to download) | Varies | STL, OBJ, 3DS, BLEND, MAX | 50k+ | Mixed free/paid; no account needed for free downloads | [Website](https://free3d.com/) |
| [**Pinshape**](https://www.pinshape.com/) | Yes (free) | 15% to creator | STL, OBJ | 50k+ | Part of UltiMaker; print result sharing with metadata | [Website](https://www.pinshape.com/) |
| [**3D Kitbash**](https://www.3dkitbash.com/) | Yes (free to browse) | Varies | STL | Curated selection | High-quality miniatures and diorama pieces | [Website](https://www.3dkitbash.com/) |

### Engineering-Focused

| Repository | Description | File Formats | Link |
|------------|-------------|--------------|------|
| [**GrabCAD**](https://grabcad.com/library) | Engineering community by Stratasys; CAD models with design intent | STEP, SLDPRT, IPT, STL, IGES | [Website](https://grabcad.com/library) |
| [**MakerRepo**](https://makerrepo.io/) | Git-based platform for parametric CAD models; version control for designs | STEP, STL, FCStd | [Website](https://makerrepo.io/) |

### Self-Hostable

| Tool | License | Language | Database | Description |
|------|---------|----------|----------|-------------|
| [**Manyfold**](https://manyfold.app/) | MIT | Ruby on Rails | SQLite / PostgreSQL | Self-hosted 3D model library; tagging, categories, preview generation; imports STL/3MF/OBJ |
| [**Thangs**](https://thangs.com/) | Commercial | — | — | Geometric search engine; personal library; sync with local storage; visual matching |

### Search Engines

| Tool | Indexed Repositories | Description | Link |
|------|---------------------|-------------|------|
| [**Yeggi**](https://www.yeggi.com/) | 10M+ models across 150+ sites | 3D model search engine; filters by free/paid, category | [Website](https://www.yeggi.com/) |
| [**STLFinder**](https://www.stlfinder.com/) | Multiple repositories | Aggregates STL files; category and price filters | [Website](https://www.stlfinder.com/) |
| [**Thangs**](https://thangs.com/) | Proprietary index | Geometric matching; visual search; personal library sync | [Website](https://thangs.com/) |

---

## Online Tools & Utilities

| Tool | Type | Platforms | Pricing | Description |
|------|------|-----------|---------|-------------|
| [**Polyvia3D**](https://polyvia3d.com/) | File conversion/repair | Browser | Free (local processing) | Browser-based via WebAssembly; repair, convert, merge; no server upload |
| [**CADProps**](https://www.cadprops.com/tools/step-to-stl/) | CAD-to-mesh conversion | Browser | Pricing not stated; sign-in required | Converts STEP/STP models to STL meshes for slicer import; files are uploaded for server processing |
| [**3D Box Generator**](https://www.thingiverse.com/apps/box-generator) | Parametric generator | Browser | Free | Generates parametric box STL files; customizable parameters |
| [**gcode.ws**](https://gcode.ws/) | G-code viewer | Browser | Free | Web-based G-code visualization; layer-by-layer preview; travel moves, extrusion analysis |
| [**Filameter**](https://filameter.io/) | Cost calculator | Browser | Free | Estimates filament usage and cost from STL; basic slicer simulation |
| [**Filwiz**](https://filwiz.com/) | Filament cost calculator | Browser | Free | Density-based filament calculator; compares materials |
| [**Lithophane Generator**](https://lithophanemaker.com/) | Image-to-STL | Browser | Free | Converts photos to lithophane 3D models; adjustable thickness, curves |
| [**SVG to STL**](https://svg2stl.com/) | 2D-to-3D conversion | Browser | Free | Extrudes SVG paths to 3D; adjustable extrusion depth |
| [**Image to Lithophane**](https://itslitho.com/) | Image processing | Browser | Free | Online lithophane generator; flat, curved, cylindrical shapes |
| [**STL Volume Calculator**](https://make.bernis.dev/) | Volume calculator | Browser | Free | Calculates volume, surface area, bounding box from STL |
| [**3D Model Metrics**](https://3d-model-metrics.netlify.app/) | Model analysis | Browser | Free | Analyzes wall thickness, dimensions, triangle count, manifold errors |

---

## Design Guidelines

### FDM Design Guidelines

| Parameter | Minimum Value | Recommended Value | Notes |
|-----------|--------------|-------------------|-------|
| **Wall Thickness (vertical)** | 0.8 mm | 1.2 mm+ | 2+ perimeters at 0.4 mm nozzle |
| **Wall Thickness (horizontal/top)** | 0.8 mm | 1.0–1.2 mm+ | 4–6 top/bottom layers minimum |
| **Wall Thickness (unsupported/tall)** | 1.0 mm | 1.5 mm+ | Increases with height-to-thickness ratio |
| **Wall Thickness (structural/load-bearing)** | 1.5 mm | 2.0–3.0 mm+ | 3+ perimeters; 20%+ infill |
| **Tolerance (features < 100 mm)** | ±0.3 mm | ±0.2 mm (tuned) | Depends on printer; affected by thermal contraction, belt tension, steps/mm |
| **Tolerance (features > 100 mm)** | ±0.3% | ±0.2% (tuned) | Scale-dependent; thermal contraction affects larger parts |
| **Clearance (moving parts)** | 0.5 mm | 0.6–0.8 mm | Gap between moving parts to prevent fusion |
| **Press Fit** | +0.1 mm interference | +0.15–0.2 mm interference | Interference fit; test fit required |
| **Snap Fit** | +0.2 mm clearance | +0.25–0.3 mm clearance | Temporary deformation for assembly |
| **Overhang (without support)** | 45° from vertical | ≤45° from vertical | >45° may require supports; surface quality degrades |
| **Overhang (with support)** | Up to 60° | ≤50° | >60° even with supports risks heat buildup and poor surface |
| **Bridging (reliable)** | 10 mm | ≤10 mm | Minimal sag with proper cooling and tension |
| **Bridging (possible, some droop)** | 10–30 mm | — | First-layer drooping expected; may need support |
| **Bridging (> 30 mm)** | — | Add center column or support | Unsupported spans >30 mm likely to fail |
| **Hole Diameter (vertical)** | 1.0 mm | ≥2.0 mm | Smaller holes may not print; bell-shaped deformation |
| **Hole Diameter (horizontal)** | 2.0 mm | ≥3.0 mm | Horizontal holes need teardrop shape to avoid supports |
| **Hole Compensation** | +0.2 mm | +0.2–0.4 mm over nominal | Holes print smaller than designed; compensate in CAD |
| **Minimum Feature Size** | 0.4 mm (nozzle diameter) | 0.8–1.0 mm | Related to nozzle size; 0.2 mm layer height common |
| **Thread Size (minimum)** | M3 | M4+ | Tapped threads: M3 minimum; printed threads: M5+ recommended |
| **Infill (decorative)** | 5–10% | 10–15% | Gyroid or grid patterns for balanced strength |
| **Infill (functional)** | 20% | 20–50% | Gyroid, honeycomb, or cubic for isotropic strength |
| **Infill (structural)** | 40% | 50–100% | Solid for maximum strength; 3+ perimeters |

### SLA/DLP Design Guidelines

| Parameter | Minimum Value | Recommended Value | Notes |
|-----------|--------------|-------------------|-------|
| **Wall Thickness (unsupported)** | 0.4 mm | 0.6 mm+ | Thin walls may break during support removal |
| **Wall Thickness (supported)** | 0.3 mm | 0.4 mm+ | Connected to other geometry for stability |
| **Tolerance** | ±0.1 mm | ±0.15 mm | Higher accuracy than FDM; resin shrinkage ~0.3% |
| **Minimum Detail Size** | 0.1–0.2 mm | 0.3–0.5 mm | Depends on XY resolution (25–50 μm typical) |
| **Overhang** | 30° from vertical | ≤30° from vertical | Shallower overhangs reduce support marks |
| **Hole Diameter** | 0.5 mm | ≥1.0 mm | Small holes may clog with uncured resin |
| **Drain Holes (hollow parts)** | 3–5 mm | 5–8 mm+ | Allows resin drainage; 2+ holes recommended |
| **Support Spacing** | 0.5–1.0 mm from surface | 0.5 mm offset | Supports leave marks; offset from critical surfaces |

### SLS Design Guidelines

| Parameter | Minimum Value | Notes |
|-----------|--------------|-------|
| **Wall Thickness** | 0.7–1.0 mm | Unfused powder supports geometry; no separate supports needed |
| **Tolerance** | ±0.2 mm | Depends on material and machine; nylon shrinks ~3% |
| **Clearance (moving parts)** | 0.5–1.0 mm | Interlocking parts can be printed assembled |
| **Hole Diameter** | 1.0 mm | Unfused powder must be removable |
| **Escape Holes (hollow parts)** | 5 mm+ | Required for powder removal |

### General Design Best Practices

- **Orient parts strategically**: Strongest in X/Y plane; weakest in Z (layer adhesion ~60% of bulk strength for FDM)
- **Minimize support usage**: Design self-supporting angles (<45° for FDM); use teardrop holes for horizontal channels
- **Add fillets and chamfers**: Reduces stress concentration; improves printability at edges
- **Design for assembly**: Split large parts; use alignment pins, screw bosses, snap fits
- **Account for anisotropy**: FDM parts are weaker along layer lines; orient load-bearing features perpendicular to layers
- **Test fit before full print**: Print small-scale or single-feature tests to validate dimensions
- **Use standard hardware**: Design for M3, M4, M5 screws and heat-set inserts where possible
- **Consider shrinkage**: PLA ~0.2%, ABS ~0.5–0.7%, Nylon ~1.5%; compensate in design or slicer scaling

---

## Developer Tools & Automation

| Tool | Language | Type | Description | Link |
|------|----------|------|-------------|------|
| [**CadQuery**](https://github.com/CadQuery/cadquery) | Python | CAD library | Parametric CAD scripting with OpenCASCADE kernel; Jupyter integration | [GitHub](https://github.com/CadQuery/cadquery) |
| [**build123d**](https://github.com/gumyr/build123d) | Python | CAD library | Fluent API for solid modeling; algebraic operations; OCP-based | [GitHub](https://github.com/gumyr/build123d) |
| [**trimesh**](https://github.com/mikedh/trimesh) | Python | Mesh library | Load, analyze, and manipulate triangular meshes; repair, convex hull, boolean operations | [GitHub](https://github.com/mikedh/trimesh) |
| [**numpy-stl**](https://github.com/WoLpH/numpy-stl) | Python | STL library | Fast STL file reading/writing using numpy; mesh analysis | [GitHub](https://github.com/WoLpH/numpy-stl) |
| [**pyThreeMF**](https://github.com/3MFConsorium/pyThreeMF) | Python | 3MF library | Python bindings for lib3MF; read/write 3MF files | [GitHub](https://github.com/3MFConsorium/pyThreeMF) |
| [**Ulipper**](https://github.com/ChronicusDev/ulipper) | Python | CLI utility | Upload G-code files to OctoPrint/Klipper from command line | [GitHub](https://github.com/ChronicusDev/ulipper) |
| [**Moonraker API**](https://moonraker.readthedocs.io/en/latest/web_api/) | REST API | API | Web API for Klipper; enables remote print control, file management, and monitoring | [Docs](https://moonraker.readthedocs.io/en/latest/web_api/) |
| [**OctoPrint API**](https://docs.octoprint.org/en/master/api/) | REST API | API | Control OctoPrint instances programmatically; job control, file management, settings | [Docs](https://docs.octoprint.org/en/master/api/) |
| [**Bambu Lab API**](https://wiki.bambulab.com/en/) | MQTT / LAN API | API | Local and cloud control for Bambu Lab printers; send prints, monitor status, control hardware | [Wiki](https://wiki.bambulab.com/en/) |
| [**CuraEngine CLI**](https://github.com/Ultimaker/CuraEngine) | CLI | Slicer engine | Command-line slicing engine for Cura profiles; automation and CI/CD integration | [GitHub](https://github.com/Ultimaker/CuraEngine) |
| [**PrusaSlicer CLI**](https://github.com/prusa3d/PrusaSlicer) | CLI | Slicer engine | Command-line slicing with config bundles; batch processing | [GitHub](https://github.com/prusa3d/PrusaSlicer) |
| [**OrcaSlicer CLI**](https://github.com/SoftFever/OrcaSlicer) | CLI | Slicer engine | Command-line slicing; inherits PrusaSlicer CLI features | [GitHub](https://github.com/SoftFever/OrcaSlicer) |
| [**admesh**](https://github.com/admesh/admesh) | C / CLI | Mesh repair | Command-line STL analysis and repair; degenerate facets, normals, adjacency | [GitHub](https://github.com/admesh/admesh) |
| [**MeshLab Server**](https://www.meshlab.net/) | Python scripting (via filters) | Mesh processing | Batch mesh processing via filter scripts; XML filter chains | [Website](https://www.meshlab.net/) |
| [**Blender Python API (bpy)**](https://docs.blender.org/api/current/) | Python | 3D scripting | Full Blender control via Python scripts; mesh generation, sculpting, export | [Docs](https://docs.blender.org/api/current/) |
| [**FreeCAD Python API**](https://wiki.freecad.org/Power_users_hub) | Python | 3D scripting | Parametric modeling via Python scripts; workbench automation | [Wiki](https://wiki.freecad.org/Power_users_hub) |
| [**OpenSCAD CLI**](https://en.wikibooks.org/wiki/OpenSCAD_User_Manual/Using_OpenSCAD_in_a_command_line_environment) | CLI | Rendering | Command-line STL/OFF/AMF rendering from .scad files; automation | [Wiki](https://en.wikibooks.org/wiki/OpenSCAD_User_Manual/Using_OpenSCAD_in_a_command_line_environment) |

---

## Learning Resources

### Books

| Title | Author | Year | ISBN | Topics | Level | Link |
|-------|--------|------|------|--------|-------|------|
| **The 3D Printing Handbook** | Ben Redwood, Samuel Tackett, Brian Garret | 2017 | 978-0997971703 | Technologies, design for AM, materials, processes, applications | All levels | [3D Hubs](https://www.3dhubs.com/3d-printing-book/) |
| **3D Printing for Beginners** | Benjamin Dixon | 2023 | 978-1732848917 | FDM setup, slicer configuration, troubleshooting, first prints | Beginner | [Amazon](https://www.amazon.com/3D-Printing-Beginners-Benjamin-Dixon/dp/1732848912/) |
| **How to Make Money with 3D Printing** | Benjamin Dixon | 2023 | 978-1732848948 | Business models, pricing, selling prints, IP considerations | Intermediate | [Amazon](https://www.amazon.com/Make-Money-3D-Printing-Business/dp/1732848947/) |
| **Make: 3D Printing** | Lydia Sloan Cline | 2012 | 978-1449309151 | Technology overview, design basics, practical projects | Beginner | [Amazon](https://www.amazon.com/Make-3D-Printing-Technologies-Design/dp/1449309151/) |
| **The Beginner's Guide to 3D Printing** | Matthew Zody | 2015 | 978-1641526424 | Printer types, setup, materials, first projects | Beginner | [Amazon](https://www.amazon.com/3D-Printing-Beginners-Essential-Know/dp/1641526424/) |
| **3D Printing: The Definitive Handbook** |— | 2022 | 978-B0B8WQ2V1Z | From first print to advanced techniques; materials, troubleshooting | All levels | [Amazon](https://www.amazon.com/PRINTING-Definitive-Handbook-UPDATED-EXPANDED/dp/B0B8WQ2V1Z/) |
| **Additive Manufacturing Technologies** | Ian Gibson, David Rosen, Brent Stucker | 2021 (3rd ed.) | 978-1071607752 | Academic textbook: AM processes, materials, design, applications | Advanced | [Springer](https://www.springer.com/gp/book/9781071607756) |
| **Design for Additive Manufacturing** | Alexander M. Meerson, et al. | 2020 | 978-0128167167 | DfAM principles, topology optimization, lattice structures | Advanced | [Elsevier](https://www.elsevier.com/books/design-for-additive-manufacturing/meerson/978-0-12-816716-4) |

### YouTube Channels

| Channel | Focus | Upload Frequency | Subscribers (approx.) | Link |
|---------|-------|------------------|----------------------|------|
| [**Maker's Muse**](https://www.youtube.com/c/MakersMuse) | 3D printing tutorials, printer reviews, design tips | Weekly | 500k+ | [YouTube](https://www.youtube.com/c/MakersMuse) |
| [**CNC Kitchen**](https://www.youtube.com/c/KNCKitchen) | Engineering analysis, material properties, 3D printing science | Weekly | 500k+ | [YouTube](https://www.youtube.com/c/KNCKitchen) |
| [**3D Printing Nerd**](https://www.youtube.com/c/3DPrintingNerd) | Printer reviews, interviews, news, tutorials | 2–3×/week | 400k+ | [YouTube](https://www.youtube.com/c/3DPrintingNerd) |
| [**Teaching Tech**](https://www.youtube.com/c/TeachingTech) | 3D printing, Klipper setup, firmware, printer builds | Weekly | 400k+ | [YouTube](https://www.youtube.com/c/TeachingTech) |
| [**CHEP**](https://www.youtube.com/c/CheapEasyPrintableThings) | Budget 3D printing, practical prints, upgrades | Weekly | 300k+ | [YouTube](https://www.youtube.com/c/CheapEasyPrintableThings) |
| [**Chris's Basement**](https://www.youtube.com/c/ChrisBriscoe) | Printer reviews, Bambu Lab content, comparisons | Weekly | 300k+ | [YouTube](https://www.youtube.com/c/ChrisBriscoe) |
| [**Ellis 3D Printer Geek**](https://www.youtube.com/c/Ellis3DPrinterGeek) | Klipper configuration, firmware, advanced techniques | Weekly | 200k+ | [YouTube](https://www.youtube.com/c/Ellis3DPrinterGeek) |
| [**Thomas Sanladerer**](https://www.youtube.com/c/ThomasSanladerer) | 3D printing analysis, industry commentary, reviews | Weekly | 200k+ | [YouTube](https://www.youtube.com/c/ThomasSanladerer) |
| [**3DJake**](https://www.youtube.com/c/3DJake) | Printer reviews, tutorials, product showcases | 2–3×/week | 200k+ | [YouTube](https://www.youtube.com/c/3DJake) |
| [**Williams Workshop**](https://www.youtube.com/c/WilliamsWorkshop) | Beginner guides, practical prints, tips | Weekly | 100k+ | [YouTube](https://www.youtube.com/c/WilliamsWorkshop) |
| [**Nerdforge**](https://www.youtube.com/c/Nerdforge) | Fusion 360 tutorials, functional prints, design | Weekly | 100k+ | [YouTube](https://www.youtube.com/c/Nerdforge) |
| [**Product Review 3D**](https://www.youtube.com/c/ProductReview3D) | Filament and accessory reviews | Weekly | 50k+ | [YouTube](https://www.youtube.com/c/ProductReview3D) |

### Courses & Tutorials

| Resource | Format | Topics | Pricing | Provider | Link |
|----------|--------|--------|---------|----------|------|
| **Prusa Academy** | Video tutorials | FDM, resin printing, maintenance, troubleshooting | Free | Prusa Research | [Website](https://academy.prusa3d.com/) |
| **Autodesk 3D Printing Courses** | Online courses | Fusion 360, Tinkercad, generative design | Free | Autodesk | [Website](https://www.autodesk.com/support/technical/3d-printing) |
| **3D Printing Specialization (Coursera)** | University course (5 courses) | 3D printing basics, software, hardware, applications | Free (audit); $49/mo (certificate) | University of Illinois (Coursera) | [Website](https://www.coursera.org/specializations/3dprinting) |
| **Blender Guru Donut Tutorial** | Video tutorial series | Blender basics, modeling, sculpting, rendering | Free | Blender Guru (YouTube) | [YouTube](https://www.youtube.com/playlist?list=PLjEaoINr3zgEq0u2MzVgAaHEBt--xLB6U) |
| **Product Design Online (Fusion 360)** | Video tutorial series | Fusion 360 for product design, 3D modeling | Free | Product Design Online (YouTube) | [YouTube](https://www.youtube.com/playlist?list=PL0G1-Eg1YV59T0KvL8Fz7dU4jQ6yRu5tK) |
| **SolidProfessor** | Subscription tutorials | SolidWorks, CAD, 3D printing | $395/yr | SolidProfessor | [Website](https://www.solidprofessor.com/) |
| **Udemy 3D Printing Courses** | Video courses (various) | Blender, Fusion 360, 3D printing, Cura | $15–$200 (sales frequent) | Udemy | [Website](https://www.udemy.com/topic/3d-printing/) |
| **Teaching Tech Klipper Guide** | Written/video guide | Klipper installation, configuration, tuning | Free (donations) | Teaching Tech | [Website](https://teachingtechyt.github.io/klipper.html) |

---

## Communities & Forums

| Community | Platform | Members | Activity Level | Focus | Link |
|-----------|----------|---------|----------------|-------|------|
| **r/3Dprinting** | Reddit | 1.5M+ | Very high | General 3D printing discussions, showcases, help | [Reddit](https://www.reddit.com/r/3Dprinting/) |
| **r/FixMyPrint** | Reddit | 100k+ | High | Troubleshooting and print quality help | [Reddit](https://www.reddit.com/r/FixMyPrint/) |
| **r/functionalprint** | Reddit | 100k+ | Moderate | Functional 3D printed designs and engineering | [Reddit](https://www.reddit.com/r/functional_print/) |
| **r/BambuLab** | Reddit | 200k+ | Very high | Bambu Lab printer users: tips, mods, troubleshooting | [Reddit](https://www.reddit.com/r/BambuLab/) |
| **r/prusa3d** | Reddit | 100k+ | Moderate | Prusa printer users community | [Reddit](https://www.reddit.com/r/prusa3d/) |
| **r/klippers** | Reddit | 100k+ | High | Klipper firmware: configs, macros, troubleshooting | [Reddit](https://www.reddit.com/r/klippers/) |
| **r/Blender** | Reddit | 1M+ | Very high | Blender 3D: modeling, sculpting, rendering help | [Reddit](https://www.reddit.com/r/blender/) |
| **r/FreeCAD** | Reddit | 50k+ | Moderate | FreeCAD users: tutorials, troubleshooting | [Reddit](https://www.reddit.com/r/FreeCAD/) |
| **r/OpenSCAD** | Reddit | 10k+ | Low–Moderate | OpenSCAD scripting and code-driven design | [Reddit](https://www.reddit.com/r/openscad/) |
| **r/ResinPrinting** | Reddit | 100k+ | High | SLA/DLP/LCD resin printing: troubleshooting, reviews | [Reddit](https://www.reddit.com/r/ResinPrinting/) |
| **3D Printing Forum** | Forum | 50k+ | Moderate | Hardware, software, materials discussions | [Website](https://www.3dprintingforum.com/) |
| **All3DP Forum** | Forum | 20k+ | Low–Moderate | General 3D printing Q&A | [Website](https://forum.all3dp.com/) |
| **3D Printing Discord** | Discord | 50k+ | Very high | Real-time chat for troubleshooting and discussion | [Discord](https://discord.gg/3dprinting) |
| **Klipper Discord** | Discord | 30k+ | Very high | Klipper configuration, macros, troubleshooting | [Discord](https://discord.klipper3d.org/) |
| **Facebook: 3D Printing For Noobs** | Facebook Group | 100k+ | High | Beginner-friendly Q&A and support | [Facebook](https://www.facebook.com/groups/3DPrintingForNoobs) |

---

## Related Awesome Lists

- [**Awesome 3D Printing**](https://github.com/ad-si/awesome-3d-printing) — 3D printing resources: printers, slicers, scanners, repositories
- [**Awesome 3D**](https://github.com/yinjiaoyang/awesome-3d) — 3D ecosystems, tools, viewers, rendering, Web3D
- [**Awesome CAD**](https://github.com/nicolaysen/awesome-cad) — Open-source CAD tools and libraries
- [**Awesome Blender**](https://github.com/agarrharr/awesome-blender) — Blender addons, resources, tutorials
- [**Awesome FreeCAD**](https://github.com/nanowish/awesome-freecad) — FreeCAD macros, addons, workbenches
- [**Awesome Klipper**](https://github.com/fsarmento/awesome-klipper) — Klipper firmware plugins, macros, configurations
- [**Awesome Slicers**](https://github.com/duckMayn/awesome-slicers) — Slicer software and slicing algorithms
- [**3D Printing Wiki (Voron)**](https://wiki.vorondesign.com/) — Voron printer builds, Klipper configs, tuning guides
- [**Ellis Klipper Guide**](https://ellis3dp.com/Print-Tuning-Guide/) — Comprehensive Klipper configuration and setup guide
- [**Teaching Tech Klipper**](https://teachingtechyt.github.io/klipper.html) — Step-by-step Klipper installation and setup

---

## Contribute

Contributions are welcome. Please follow the guidelines below:

### What to Add

- Tools, software, or resources related to 3D modeling for 3D printing
- CAD software, sculpting tools, and mesh editors
- Topology optimization, generative design, and lattice tools
- Developer tools, APIs, and automation utilities
- Mesh repair, analysis, and printability checkers
- Texture, surface detail, and displacement tools
- Learning resources (books, courses, tutorials, documentation)
- Communities, forums, and discussion groups
- 3D model repositories and marketplaces
- Design guidelines and best practices

### How to Contribute

1. Fork this repository
2. Add your resource to the appropriate section
3. Include: name, description, license/pricing, platforms, and a working link
4. Verify the resource is not already listed
5. Submit a Pull Request

### Criteria

- **Relevance**: Must relate to 3D modeling, 3D printing, or supporting workflows
- **Accuracy**: Information should be current and verifiable
- **Completeness**: Include pricing, platforms, and file formats where applicable
- **No Duplicates**: Check existing entries; if a resource fits multiple categories, place it in the most relevant section
- **Neutral Tone**: Describe what the tool does; avoid subjective claims like "best" or "amazing"

---

## License

[![CC0](https://licensebuttons.net/p/zero/1.0/88x31.png)](https://creativecommons.org/publicdomain/zero/1.0/)

This work is dedicated to the public domain under the Creative Commons Zero 1.0 Universal license.

---

<div align="center">
  <strong>3D Modeling for 3D Printing — Resources & Tools</strong>
</div>
