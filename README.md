# multiplayer-agents

UI prototype for a multiplayer agent workspace: a shared tree of agents that several people can watch, prompt, and steer at once.

## What's in it

`index.html` is a single self-contained page (no build step).

- **2D tree** — ink-on-paper view. Branches hold agents; the selected branch is highlighted and its edges animate. Drag to pan, scroll or pinch to zoom, click a branch to zoom into it, press `F` to fit the whole tree.
- **3D tree** — the same data drawn as a toy tree on an island (three.js, toon shading). Root at the top, agents at the bottom. Drag to orbit, scroll to zoom, double-click to fly to a node.
- **View** menu (mission bar) switches 2D / 3D and toggles the mini map, 3D labels, and idle auto-orbit. The choice is remembered; `#2d` / `#3d` in the URL also set it.
- **Inspector** (right) — the selected agent's status, pending decision with countdown / hold / approve, recent decisions, instructions in effect (inherited down the tree), and transcript.
- **Jump** (`⌘K`) — search agents, branches, and open decisions.
- **Composer** — message a whole branch or one agent; click the `To:` pill to switch.

## Run it

Open `index.html` in a browser. Three.js loads from a CDN, so the 3D view needs a network connection.

All agents, people, and decisions are example data.
