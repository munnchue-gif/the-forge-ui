# Master Write-Up Page

Target Source: `/home/mancier/core_Forge-unziped`

## 📂 Directory Structure

```text
/home/mancier/core_Forge-unziped/
├── 📄 .gitignore
├── 📄 .npmrc
├── 📄 AGENTS.md
├── 📄 CLAUDE.md
├── 📄 FORGE_TRANSFER.md
├── 📄 README.md
├── 📁 base44/
│   ├── 📄 config.jsonc
│   ├── 📁 connectors/
│   │   ├── 📄 github.jsonc
│   │   ├── 📄 googledocs.jsonc
│   │   ├── 📄 googledrive.jsonc
│   │   ├── 📄 googlesheets.jsonc
│   │   ├── 📄 googleslides.jsonc
│   │   └── 📄 hugging_face.jsonc
│   └── 📁 entities/
│       ├── 📄 BridgeConnection.jsonc
│       ├── 📄 ConnectionEvent.jsonc
│       ├── 📄 FileReview.jsonc
│       ├── 📄 ForgeControl.jsonc
│       ├── 📄 ForgePiece.jsonc
│       ├── 📄 ForgeTask.jsonc
│       └── 📄 User.jsonc
├── 📄 components.json
├── 📄 eslint.config.js
├── 📄 index.html
├── 📄 jsconfig.json
├── 📄 package-lock.json
├── 📄 package.json
├── 📄 postcss.config.js
├── 📁 src/
│   ├── 📄 App.jsx
│   ├── 📁 api/
│   │   └── 📄 base44Client.js
│   ├── 📁 components/
│   │   ├── 📄 AuthLayout.jsx
│   │   ├── 📄 GoogleIcon.jsx
│   │   ├── 📄 ProtectedRoute.jsx
│   │   ├── 📄 ScrollToTop.jsx
│   │   ├── 📄 UserNotRegisteredError.jsx
│   │   ├── 📁 bridge/
│   │   │   ├── 📄 BridgeSettings.jsx
│   │   │   ├── 📄 ConcoctPanel.jsx
│   │   │   ├── 📄 ConnectionGuide.jsx
│   │   │   ├── 📄 HealthPanel.jsx
│   │   │   ├── 📄 LedgerPanel.jsx
│   │   │   ├── 📄 LiveFeed.jsx
│   │   │   ├── 📄 MintPanel.jsx
│   │   │   ├── 📄 PanelShell.jsx
│   │   │   ├── 📄 TaskRow.jsx
│   │   │   ├── 📄 TroubleshootPanel.jsx
│   │   │   └── 📄 WrapsPanel.jsx
│   │   ├── 📁 deck/
│   │   │   ├── 📄 AddControlDialog.jsx
│   │   │   ├── 📄 BoardControlStrip.jsx
│   │   │   ├── 📄 NeonButton.jsx
│   │   │   ├── 📄 NeonSlider.jsx
│   │   │   ├── 📄 NeonToggle.jsx
│   │   │   ├── 📄 deckColors.js
│   │   │   └── 📄 useControls.js
│   │   ├── 📁 forge/
│   │   │   ├── 📄 CodeBlock.jsx
│   │   │   ├── 📄 GradeBadge.jsx
│   │   │   ├── 📄 PieceCard.jsx
│   │   │   ├── 📄 PieceEditForm.jsx
│   │   │   ├── 📄 cheatSheet.js
│   │   │   ├── 📄 gradeConfig.js
│   │   │   └── 📄 installSteps.js
│   │   ├── 📁 review/
│   │   │   ├── 📄 DropZone.jsx
│   │   │   ├── 📄 ReviewCard.jsx
│   │   │   └── 📄 reviewGrader.js
│   │   ├── 📁 sockets/
│   │   │   ├── 📄 AddConnectionDialog.jsx
│   │   │   ├── 📄 ConnectionCard.jsx
│   │   │   ├── 📄 HistoryLog.jsx
│   │   │   ├── 📄 SocketDock.jsx
│   │   │   └── 📄 socketKinds.js
│   │   └── 📁 ui/
│   │       ├── 📄 accordion.jsx
│   │       ├── 📄 alert-dialog.jsx
│   │       ├── 📄 alert.jsx
│   │       ├── 📄 aspect-ratio.jsx
│   │       ├── 📄 avatar.jsx
│   │       ├── 📄 badge.jsx
│   │       ├── 📄 breadcrumb.jsx
│   │       ├── 📄 button.jsx
│   │       ├── 📄 calendar.jsx
│   │       ├── 📄 card.jsx
│   │       ├── 📄 carousel.jsx
│   │       ├── 📄 chart.jsx
│   │       ├── 📄 checkbox.jsx
│   │       ├── 📄 collapsible.jsx
│   │       ├── 📄 command.jsx
│   │       ├── 📄 context-menu.jsx
│   │       ├── 📄 dialog.jsx
│   │       ├── 📄 drawer.jsx
│   │       ├── 📄 dropdown-menu.jsx
│   │       ├── 📄 form.jsx
│   │       ├── 📄 hover-card.jsx
│   │       ├── 📄 image.jsx
│   │       ├── 📄 input-otp.jsx
│   │       ├── 📄 input.jsx
│   │       ├── 📄 label.jsx
│   │       ├── 📄 menubar.jsx
│   │       ├── 📄 navigation-menu.jsx
│   │       ├── 📄 pagination.jsx
│   │       ├── 📄 popover.jsx
│   │       ├── 📄 progress.jsx
│   │       ├── 📄 radio-group.jsx
│   │       ├── 📄 resizable.jsx
│   │       ├── 📄 scroll-area.jsx
│   │       ├── 📄 select.jsx
│   │       ├── 📄 separator.jsx
│   │       ├── 📄 sheet.jsx
│   │       ├── 📄 sidebar.jsx
│   │       ├── 📄 skeleton.jsx
│   │       ├── 📄 slider.jsx
│   │       ├── 📄 sonner.jsx
│   │       ├── 📄 switch.jsx
│   │       ├── 📄 table.jsx
│   │       ├── 📄 tabs.jsx
│   │       ├── 📄 textarea.jsx
│   │       ├── 📄 toast.jsx
│   │       ├── 📄 toaster.jsx
│   │       ├── 📄 toggle-group.jsx
│   │       ├── 📄 toggle.jsx
│   │       ├── 📄 tooltip.jsx
│   │       └── 📄 use-toast.jsx
│   ├── 📁 hooks/
│   │   ├── 📄 use-mobile.jsx
│   │   └── 📄 use-size.jsx
│   ├── 📄 index.css
│   ├── 📁 lib/
│   │   ├── 📄 AuthContext.jsx
│   │   ├── 📄 PageNotFound.jsx
│   │   ├── 📄 app-params.js
│   │   ├── 📄 connectionVault.js
│   │   ├── 📄 forgeBridge.js
│   │   ├── 📄 query-client.js
│   │   └── 📄 utils.js
│   ├── 📄 main.jsx
│   ├── 📁 pages/
│   │   ├── 📄 Board.jsx
│   │   ├── 📄 CheatSheet.jsx
│   │   ├── 📄 ControlDeck.jsx
│   │   ├── 📄 ForgeLink.jsx
│   │   ├── 📄 ForgotPassword.jsx
│   │   ├── 📄 InstallGuide.jsx
│   │   ├── 📄 Login.jsx
│   │   ├── 📄 PieceDetail.jsx
│   │   ├── 📄 Register.jsx
│   │   ├── 📄 ResetPassword.jsx
│   │   └── 📄 ReviewBay.jsx
│   └── 📁 utils/
│       └── 📄 index.ts
├── 📄 tailwind.config.js
└── 📄 vite.config.js
```

---

# 📄 File Contents Manifest


---

## File: `vite.config.js`

```text
import base44 from "@base44/vite-plugin"
import react from '@vitejs/plugin-react'
import { defineConfig } from 'vite'

// https://vite.dev/config/
export default defineConfig({
  plugins: [
    base44({
      // Support for legacy code that imports the base44 SDK with @/integrations, @/entities, etc.
      // can be removed if the code has been updated to use the new SDK imports from @base44/sdk
      legacySDKImports: process.env.BASE44_LEGACY_SDK_IMPORTS === 'true',
      hmrNotifier: true,
      navigationNotifier: true,
      analyticsTracker: true,
      visualEditAgent: true
    }),
    react(),
  ]
});

```

---

## File: `tailwind.config.js`

```text
/** @type {import('tailwindcss').Config} */
module.exports = {
    darkMode: ["class"],
    content: ["./index.html", "./src/**/*.{ts,tsx,js,jsx}"],
  theme: {
  	extend: {
  		borderRadius: {
  			lg: 'var(--radius)',
  			md: 'calc(var(--radius) - 2px)',
  			sm: 'calc(var(--radius) - 4px)'
  		},
  		colors: {
  			background: 'hsl(var(--background))',
  			foreground: 'hsl(var(--foreground))',
  			card: {
  				DEFAULT: 'hsl(var(--card))',
  				foreground: 'hsl(var(--card-foreground))'
  			},
  			popover: {
  				DEFAULT: 'hsl(var(--popover))',
  				foreground: 'hsl(var(--popover-foreground))'
  			},
  			primary: {
  				DEFAULT: 'hsl(var(--primary))',
  				foreground: 'hsl(var(--primary-foreground))'
  			},
  			secondary: {
  				DEFAULT: 'hsl(var(--secondary))',
  				foreground: 'hsl(var(--secondary-foreground))'
  			},
  			muted: {
  				DEFAULT: 'hsl(var(--muted))',
  				foreground: 'hsl(var(--muted-foreground))'
  			},
  			accent: {
  				DEFAULT: 'hsl(var(--accent))',
  				foreground: 'hsl(var(--accent-foreground))'
  			},
  			destructive: {
  				DEFAULT: 'hsl(var(--destructive))',
  				foreground: 'hsl(var(--destructive-foreground))'
  			},
  			border: 'hsl(var(--border))',
  			input: 'hsl(var(--input))',
  			ring: 'hsl(var(--ring))',
  			chart: {
  				'1': 'hsl(var(--chart-1))',
  				'2': 'hsl(var(--chart-2))',
  				'3': 'hsl(var(--chart-3))',
  				'4': 'hsl(var(--chart-4))',
  				'5': 'hsl(var(--chart-5))'
  			},
  			sidebar: {
  				DEFAULT: 'hsl(var(--sidebar-background))',
  				foreground: 'hsl(var(--sidebar-foreground))',
  				primary: 'hsl(var(--sidebar-primary))',
  				'primary-foreground': 'hsl(var(--sidebar-primary-foreground))',
  				accent: 'hsl(var(--sidebar-accent))',
  				'accent-foreground': 'hsl(var(--sidebar-accent-foreground))',
  				border: 'hsl(var(--sidebar-border))',
  				ring: 'hsl(var(--sidebar-ring))'
  			}
  		},
  		fontFamily: {
  			heading: ['var(--font-heading)'],
  			body: ['var(--font-body)'],
  			display: ['var(--font-display)'],
  			mono: ['var(--font-mono)']
  		},
  		keyframes: {
  			'accordion-down': {
  				from: {
  					height: '0'
  				},
  				to: {
  					height: 'var(--radix-accordion-content-height)'
  				}
  			},
  			'accordion-up': {
  				from: {
  					height: 'var(--radix-accordion-content-height)'
  				},
  				to: {
  					height: '0'
  				}
  			}
  		},
  		animation: {
  			'accordion-down': 'accordion-down 0.2s ease-out',
  			'accordion-up': 'accordion-up 0.2s ease-out'
  		}
  	}
  },
  plugins: [require("tailwindcss-animate")],
}

```

---

## File: `eslint.config.js`

```text
import globals from "globals";
import pluginJs from "@eslint/js";
import pluginReact from "eslint-plugin-react";
import pluginReactHooks from "eslint-plugin-react-hooks";
import pluginUnusedImports from "eslint-plugin-unused-imports";

export default [
  {
    files: [
      "src/components/**/*.{js,mjs,cjs,jsx}",
      "src/pages/**/*.{js,mjs,cjs,jsx}",
      "src/Layout.jsx",
    ],
    ignores: ["src/lib/**/*", "src/components/ui/**/*"],
    ...pluginJs.configs.recommended,
    ...pluginReact.configs.flat.recommended,
    languageOptions: {
      globals: globals.browser,
      parserOptions: {
        ecmaVersion: 2022,
        sourceType: "module",
        ecmaFeatures: {
          jsx: true,
        },
      },
    },
    settings: {
      react: {
        version: "detect",
      },
    },
    plugins: {
      react: pluginReact,
      "react-hooks": pluginReactHooks,
      "unused-imports": pluginUnusedImports,
    },
    rules: {
      "no-unused-vars": "off",
      "react/jsx-uses-vars": "error",
      "react/jsx-uses-react": "error",
      "unused-imports/no-unused-imports": "error",
      "unused-imports/no-unused-vars": [
        "warn",
        {
          vars: "all",
          varsIgnorePattern: "^_",
          args: "after-used",
          argsIgnorePattern: "^_",
        },
      ],
      "react/prop-types": "off",
      "react/react-in-jsx-scope": "off",
      "react/no-unknown-property": [
        "error",
        { ignore: ["cmdk-input-wrapper", "toast-close"] },
      ],
      "react-hooks/rules-of-hooks": "error",
    },
  },
];

```

---

## File: `README.md`

```text
# Base44 Project

Use this repository to run and edit the app locally, then publish changes back through Base44.

Any change pushed to the repo will also be reflected in the Base44 Builder.

## Prerequisites

1. Clone the repository using the project's Git URL.
2. Navigate to the project directory.
3. Install dependencies: `npm install`.
4. Install the Base44 CLI: `npm install -g base44@latest`.

See the [Base44 CLI docs](https://docs.base44.com/developers/references/cli/get-started/overview) if you want to run Base44 commands directly.

## Run Locally

Run the full local development environment from the project root:

```bash
base44 dev
```

`base44 dev` starts the local Base44 development backend and, when this app is configured for it, also starts the frontend dev server for you. Use the frontend URL printed by the command.

For example, when the Base44 project config includes a `serveCommand`, `base44 dev` can launch the frontend too:

```json5
{
  "site": {
    "serveCommand": "npm run dev"
  }
}
```

In a Base44 project this lives in `base44/config.jsonc`.

## Run Only The Frontend

If you only want to work on the frontend against the hosted Base44 backend, run:

```bash
npm run dev
```

Open the local URL printed by Vite.

## Use The Hosted Backend

For frontend-only development, create or update `.env.local` in the project root:

```bash
VITE_BASE44_APP_ID=your_app_id
VITE_BASE44_APP_BASE_URL=https://your-app.base44.app
```

`VITE_BASE44_APP_ID` identifies the Base44 app.

`VITE_BASE44_APP_BASE_URL` tells the Base44 Vite plugin where to send local `/api` requests. Point it at your deployed Base44 app URL when you want the local frontend to use the hosted backend.

When you use `base44 dev`, the command injects the local Base44 values for you, so `.env.local` is mainly needed for frontend-only workflows.

## Publish Your Changes

After pushing your changes to git, open the Base44 dashboard and publish the app:

```bash
base44 dashboard open
```

## Docs & Support

Documentation: [https://docs.base44.com/Integrations/Using-GitHub](https://docs.base44.com/Integrations/Using-GitHub)

Base44 CLI command reference: [https://docs.base44.com/developers/references/cli/commands/introduction](https://docs.base44.com/developers/references/cli/commands/introduction)

Support: [https://app.base44.com/support](https://app.base44.com/support)

```

---

## File: `.gitignore`

```text
#env
.env
.env.*

# Logs
/logs
*.log
npm-debug.log*
yarn-debug.log*
yarn-error.log*
pnpm-debug.log*
lerna-debug.log*

node_modules
dist
dist-ssr
*.local

# Editor directories and files
.vscode/*
!.vscode/extensions.json
.idea
.DS_Store
*.suo
*.ntvs*
*.njsproj
*.sln
*.sw?

.env
.vite
base44/.app.jsonc

```

---

## File: `components.json`

```text
{
  "$schema": "https://ui.shadcn.com/schema.json",
  "style": "new-york",
  "rsc": false,
  "tsx": false,
  "tailwind": {
    "config": "tailwind.config.js",
    "css": "src/index.css",
    "baseColor": "neutral",
    "cssVariables": true,
    "prefix": ""
  },
  "aliases": {
    "components": "@/components",
    "utils": "@/lib/utils",
    "ui": "@/components/ui",
    "lib": "@/lib",
    "hooks": "@/hooks"
  },
  "iconLibrary": "lucide"
}
```

---

## File: `AGENTS.md`

```text
# AGENTS.md

## Project Context

This is a Base44 app repository. Treat it as user-owned application code, keep changes focused on the user's request, and preserve existing project conventions.

Start with `README.md` for local setup, environment variables, and publish workflow.

## Base44 References

- CLI overview: https://docs.base44.com/developers/references/cli/get-started/overview.md
- Agent skills: https://docs.base44.com/developers/backend/overview/skills.md

If your agent supports Agent Skills, install or update Base44 skills before Base44-specific work:

```bash
npx skills add base44/skills
```

## Key Files

- `src/`: frontend application source.
- `src/api/base44Client.js`: frontend Base44 SDK client.
- `vite.config.js`: Vite config and Base44 Vite plugin setup.
- `.env.local`: local-only environment values; never commit secrets.

## Working Notes

- Use `base44 dev` as the default local development command when you need the local Base44 backend. It can run the backend and frontend together.
- When docs or code mention the frontend being started automatically, that usually means the Base44 project config includes `site.serveCommand`, for example `"serveCommand": "npm run dev"` in `base44/config.jsonc`.
- Use `npm run dev` only for frontend-only work against the hosted Base44 backend.
- Prefer the existing Base44 CLI workflow over adding new npm scripts for Base44-specific tasks.
- Reuse the existing SDK client and Vite plugin patterns before adding new Base44 integration paths.
- Run the relevant checks from `package.json` before finishing code changes.

```

---

## File: `postcss.config.js`

```text
export default {
  plugins: {
    tailwindcss: {},
    autoprefixer: {},
  },
}

```

---

## File: `FORGE_TRANSFER.md`

```text
# THE FORGE — Full Transfer Document
> Hand this to any AI model. It contains the complete state of the project: the app, the Forge fabric concepts, where we are, and what's next.
> Last updated: 2026-07-22 · GitHub: connected as `munnchue-gif` (repo scope)

---

## 1. What this project is (two halves)

**Half A — The Forge (`forge_ng`)**: a local Python "AI fabric" that runs bare-metal on a Pop!_OS machine (Arrow Lake NPU + RTX 5080). Stdlib-only by design, 119 passing tests. It is a living resident process (systemd service), not a library.

**Half B — This web app (Base44, React + Tailwind)**: the command bridge / operator console for the Forge. Dark starship-bridge aesthetic (Orbitron/Exo 2/Share Tech Mono, amber + cyan on deep navy).

The two halves talk over HTTPS through a Cloudflare tunnel: the app is "the glass" — a read-only window plus gate-signed capability requests. Secrets never live in the app's database.

## 2. Forge core concepts (the vocabulary)

- **The Substance** — alien fabric coating the system; one material, many forms.
- **The Skeleton** — the hard frame: 7 organs, all built and GREEN.
- **Gate** — the ONE door; every privileged action is signed/verified through it (multi-tenant, replay-exact policy). Known gaps: false-replay on identical legit actions (needs nonce), unescaped `|` delimiter in signed strings (security fix pending).
- **SubstanceBus** — deaf sections + the Overseer's omnipresent tap. Gap: silent drops under load, not thread-safe.
- **Overseer** — Watcher (observe) + Commander (act-through-gate). Next: level-3 command vocabulary.
- **Capabilities** — the verbs: Spawn/Mount/Egress/NpuEval + Conform/Splice/Reclaim.
- **Wrap** — the mold that IS the training; seal identity, reclaim/repour models. Next: persistent vector store (L2).
- **VectorConduit** — the NPU bond loop (bonded, not fused). Currently on HeuristicSeat; real Arrow Lake NPU seat is the next brick.
- **Concoctinator** — sandbox/testing grounds (concoct + strip verbs, observe-mode by design).
- **Design laws**: "Pieces & LEGO" (snap-on/off modularity, war-jeep philosophy), "deaf by default, one door, nothing bare," "nothing thrown away" (The Wardrobe = recycle yard), "baptism not code" (The Awakening — gains from structure, not scale).
- **Sockets & Layers** (concept, YELLOW) — snap whole capabilities on. **Capsule Shrink & Restore** (ORANGE) — suspend/resume a Forge personality; data-pack format undefined.

Grading system used everywhere: GREEN (solid) / YELLOW (needs work) / RED (broken) / PURPLE (abstract) / ORANGE (undefined).

## 3. The app — pages & data

| Route | Page | Purpose |
|---|---|---|
| `/` | Board | Command board: all Forge pieces, graded + filterable, plus a live Bridge Controls strip |
| `/piece/:id` | PieceDetail | Full detail + editing of one piece |
| `/deck` | ControlDeck | Codeless operator console — sliders/toggles/buttons sync in real time; the Forge polls them |
| `/forge` | ForgeLink | "The glass": Sockets, Live Feed (SSE), Health, Wraps, Ledger, Mint, Concoct, Tasks |
| `/review` | ReviewBay | Drop files for graded reviews (FileReview) |
| `/install` | InstallGuide | Master install: bare-metal Pop!_OS setup, 8 steps |
| `/cheatsheet` | CheatSheet | Quick reference |

**Entities**: `ForgePiece` (the board), `ForgeControl` (live deck controls), `ForgeTask` (open work items), `FileReview`, `BridgeConnection` (socket keychain — endpoint metadata only), `ConnectionEvent` (bridge history log).

**Security model**: tokens/CF Access secrets live ONLY in the browser (`localStorage` via `src/lib/connectionVault.js` + `src/lib/forgeBridge.js`). The database stores endpoint metadata + history, never keys. `bridgeFetch` injects `Authorization`, `CF-Access-Client-Id`, `CF-Access-Client-Secret` headers; the live feed streams SSE over fetch (EventSource can't carry CF headers).

**Socket keychain (newest feature)**: register any endpoint (WSL, GitHub, Cloudflare, GPU offloader, DB, custom), pin favorites, one-press "Bridge in" (applies config + health check + logs a ConnectionEvent), "Capture live connection" saves the currently-working bridge as a socket.

## 4. The transport chain (how app ↔ Forge connect)

1. Pop!_OS machine runs the bridge: `python -m forge_ng.bridge` (endpoints: `/health`, `/feed` SSE, `/wraps`, `/ledger`, `/mint`, `/concoct/preview`).
2. `cloudflared tunnel run forge` exposes it publicly behind Cloudflare Access.
3. App's Forge Link settings hold the tunnel URL + CF service-token credentials (browser-only).
4. Separately, the Forge polls the app's `ForgeControl` entity via the Base44 data API (`forge_ng/bridge.py` DeckBridge — one-way pull, zero verbs of attack surface).

## 5. Master install — the facts

- The Install Guide (`/install`) installs the **Forge fabric on the PC**, NOT this web app. The app lives here (Base44 hosted) — nothing to install for it.
- It is current as of this writing: env setup → 119-test green check → NPU wiring (intel_vpu + Level Zero + OpenVINO) → kernel bootstrap `main.py` → NpuSeat skeleton → systemd service → DeckBridge poller.
- The bootstrap/bridge Python blocks are **templates** — import paths/signatures must be adapted to the exact forge_ng code on the machine.
- Prereqs before installing: forge_ng source on the machine, kernel 6.8+, Python 3.11+, and (for the deck bridge) the App ID + API key from this app's dashboard (Settings → API).
- After install: yes — all Forge-side fixes happen directly on the machine; app-side fixes happen here. The two evolve independently and meet at the bridge contract.

## 6. Version transfer

- **App**: Base44 keeps version history; GitHub repo sync (connected) gives full git history — branch/tag to snapshot versions.
- **Forge**: standard git on the PC (`git tag v0.x && git push`), pushed to a GitHub repo under `munnchue-gif`. Conceptually this is "Capsule Shrink & Restore" — until that's built, git IS the capsule.

## 7. Where we left off + open tasks

**Detour just completed**: socket keychain + connection history on Forge Link (done, seeded with 6 sockets — the placeholder URLs need replacing with real endpoints).

**Open ForgeTasks (the human's part)**:
1. Verify PC power and network (Pop!_OS machine on + connected).
2. Validate the local bridge process is listening (localhost:8787).
3. Check Cloudflare tunnel status (`cloudflared tunnel status`).
4. Configure the Forge Bridge URL in the app's connection settings.
5. Validate CF Access service tokens in settings.
6. Once connected: press **Capture live connection** in Forge Link → Sockets, and fix/delete placeholder sockets.

**Next bricks on the fabric (the main road we return to)**:
- Gate: nonce field (fix false replay) + escape/hash the `|` delimiter (security).
- SubstanceBus: drop logging + thread safety.
- VectorConduit: bind the real Arrow Lake NPU seat (OpenVINOSeat) — install Step 4/6.
- Wrap: persistent vector store (L2).
- Concepts: build The Embedded Tailor (unblocks Sockets & Layers), define the capsule data-pack format.

## 8. For the receiving model

You now have full context. Rules of the road: everything is LEGO (snap-on pieces, clean interfaces), nothing is thrown away (grade it, don't delete it), one door (all privileged action through the Gate), secrets stay client-side, and the app is glass — logic lives in the Forge.
```

---

## File: `package-lock.json`

```text
{
  "name": "base44-app",
  "version": "0.0.0",
  "lockfileVersion": 3,
  "requires": true,
  "packages": {
    "": {
      "name": "base44-app",
      "version": "0.0.0",
      "dependencies": {
        "@base44/sdk": "^0.8.40",
        "@base44/vite-plugin": "^1.0.30",
        "@hello-pangea/dnd": "^17.0.0",
        "@hookform/resolvers": "^4.1.2",
        "@radix-ui/react-accordion": "^1.2.3",
        "@radix-ui/react-alert-dialog": "^1.1.6",
        "@radix-ui/react-aspect-ratio": "^1.1.2",
        "@radix-ui/react-avatar": "^1.1.3",
        "@radix-ui/react-checkbox": "^1.1.4",
        "@radix-ui/react-collapsible": "^1.1.3",
        "@radix-ui/react-context-menu": "^2.2.6",
        "@radix-ui/react-dialog": "^1.1.6",
        "@radix-ui/react-dropdown-menu": "^2.1.6",
        "@radix-ui/react-hover-card": "^1.1.6",
        "@radix-ui/react-label": "^2.1.2",
        "@radix-ui/react-menubar": "^1.1.6",
        "@radix-ui/react-navigation-menu": "^1.2.5",
        "@radix-ui/react-popover": "^1.1.6",
        "@radix-ui/react-progress": "^1.1.2",
        "@radix-ui/react-radio-group": "^1.2.3",
        "@radix-ui/react-scroll-area": "^1.2.3",
        "@radix-ui/react-select": "^2.1.6",
        "@radix-ui/react-separator": "^1.1.2",
        "@radix-ui/react-slider": "^1.2.3",
        "@radix-ui/react-slot": "^1.1.2",
        "@radix-ui/react-switch": "^1.1.3",
        "@radix-ui/react-tabs": "^1.1.3",
        "@radix-ui/react-toast": "^1.2.2",
        "@radix-ui/react-toggle": "^1.1.2",
        "@radix-ui/react-toggle-group": "^1.1.2",
        "@radix-ui/react-tooltip": "^1.1.8",
        "@stripe/react-stripe-js": "^3.0.0",
        "@stripe/stripe-js": "^5.2.0",
        "@tanstack/react-query": "^5.84.1",
        "canvas-confetti": "^1.9.4",
        "class-variance-authority": "^0.7.1",
        "clsx": "^2.1.1",
        "cmdk": "^1.0.0",
        "date-fns": "^3.6.0",
        "embla-carousel-react": "^8.5.2",
        "framer-motion": "^11.16.4",
        "html2canvas": "^1.4.1",
        "input-otp": "^1.4.2",
        "jspdf": "^4.2.1",
        "lodash": "^4.17.21",
        "lucide-react": "^0.475.0",
        "moment": "^2.30.1",
        "next-themes": "^0.4.4",
        "react": "^18.2.0",
        "react-day-picker": "^8.10.1",
        "react-dom": "^18.2.0",
        "react-hook-form": "^7.54.2",
        "react-hot-toast": "^2.6.0",
        "react-leaflet": "^4.2.1",
        "react-markdown": "^9.0.1",
        "react-quill": "^2.0.0",
        "react-resizable-panels": "^2.1.7",
        "react-router-dom": "^6.26.0",
        "recharts": "^2.15.4",
        "sonner": "^2.0.1",
        "tailwind-merge": "^3.0.2",
        "tailwindcss-animate": "^1.0.7",
        "three": "^0.171.0",
        "vaul": "^1.1.2",
        "zod": "^3.24.2"
      },
      "devDependencies": {
        "@eslint/js": "^9.19.0",
        "@types/node": "^22.13.5",
        "@types/react": "^18.2.66",
        "@types/react-dom": "^18.2.22",
        "@vitejs/plugin-react": "^4.3.4",
        "autoprefixer": "^10.4.20",
        "baseline-browser-mapping": "^2.8.32",
        "eslint": "^9.19.0",
        "eslint-plugin-react": "^7.37.4",
        "eslint-plugin-react-hooks": "^5.0.0",
        "eslint-plugin-react-refresh": "^0.4.18",
        "eslint-plugin-unused-imports": "^4.3.0",
        "globals": "^15.14.0",
        "postcss": "^8.5.3",
        "tailwindcss": "^3.4.17",
        "typescript": "^5.8.2",
        "vite": "^6.1.0"
      }
    },
    "node_modules/@alloc/quick-lru": {
      "version": "5.2.0",
      "resolved": "https://registry.npmjs.org/@alloc/quick-lru/-/quick-lru-5.2.0.tgz",
      "integrity": "sha512-UrcABB+4bUrFABwbluTIBErXwvbsU/V7TZWfmbgJfbkwiBuziS9gxdODUyuiecfdGQ85jglMW6juS3+z5TsKLw==",
      "license": "MIT",
      "engines": {
        "node": ">=10"
      },
      "funding": {
        "url": "https://github.com/sponsors/sindresorhus"
      }
    },
    "node_modules/@babel/code-frame": {
      "version": "7.29.7",
      "resolved": "https://registry.npmjs.org/@babel/code-frame/-/code-frame-7.29.7.tgz",
      "integrity": "sha512-Aup7aUOfpbAUg2ROOJN6Iw5f9DMBlzu0mIkm/malLQFN/YQgO48wCj0Kxa3sEHJvPVFg7siR+qRInwXd2qhQKw==",
      "license": "MIT",
      "dependencies": {
        "@babel/helper-validator-identifier": "^7.29.7",
        "js-tokens": "^4.0.0",
        "picocolors": "^1.1.1"
      },
      "engines": {
        "node": ">=6.9.0"
      }
    },
    "node_modules/@babel/compat-data": {
      "version": "7.29.7",
      "resolved": "https://registry.npmjs.org/@babel/compat-data/-/compat-data-7.29.7.tgz",
      "integrity": "sha512-locTkQyKvwIEgBzVrn8693ebc97F2U8ZHjbXwDXJ5Fn2TCpNwTlKcaKLkdHop5c/icOFE7qt7Q9JC5hnKNa6Gg==",
      "dev": true,
      "license": "MIT",
      "engines": {
        "node": ">=6.9.0"
      }
    },
    "node_modules/@babel/core": {
      "version": "7.29.7",
      "resolved": "https://registry.npmjs.org/@babel/core/-/core-7.29.7.tgz",
      "integrity": "sha512-RgHBCvtjbOK2gXSNBNIkNoEc9qoVEtau3hj8gEqKQuL3HZAibKarWFEI3Lfm6EYKkLalOh8eSrj9b+ch9H/VBA==",
      "dev": true,
      "license": "MIT",
      "dependencies": {
        "@babel/code-frame": "^7.29.7",
        "@babel/generator": "^7.29.7",
        "@babel/helper-compilation-targets": "^7.29.7",
        "@babel/helper-module-transforms": "^7.29.7",
        "@babel/helpers": "^7.29.7",
        "@babel/parser": "^7.29.7",
        "@babel/template": "^7.29.7",
        "@babel/traverse": "^7.29.7",
        "@babel/types": "^7.29.7",
        "@jridgewell/remapping": "^2.3.5",
        "convert-source-map": "^2.0.0",
        "debug": "^4.1.0",
        "gensync": "^1.0.0-beta.2",
        "json5": "^2.2.3",
        "semver": "^6.3.1"
      },
      "engines": {
        "node": ">=6.9.0"
      },
      "funding": {
        "type": "opencollective",
        "url": "https://opencollective.com/babel"
      }
    },
    "node_modules/@babel/generator": {
      "version": "7.29.7",
      "resolved": "https://registry.npmjs.org/@babel/generator/-/generator-7.29.7.tgz",
      "integrity": "sha512-DkXD5OJQaAQIdZ1bt3UZdEnHAn9Imd3IVBdX03UFe+ony9Ojw5pzr9YVKGDY1jt+Gcn/FnGkNf8r+Vj5NOJWtQ==",
      "license": "MIT",
      "dependencies": {
        "@babel/parser": "^7.29.7",
        "@babel/types": "^7.29.7",
        "@jridgewell/gen-mapping": "^0.3.12",
        "@jridgewell/trace-mapping": "^0.3.28",
        "jsesc": "^3.0.2"
      },
      "engines": {
        "node": ">=6.9.0"
      }
    },
    "node_modules/@babel/helper-compilation-targets": {
      "version": "7.29.7",
      "resolved": "https://registry.npmjs.org/@babel/helper-compilation-targets/-/helper-compilation-targets-7.29.7.tgz",
      "integrity": "sha512-wem6WaBj4NaVYVdNhLPPVacES6ZJ+KBBfSkTMD3YZxbP3rm3Di85tJU5ljaUNhaOynt+Aj0xruhYuzQBt8n71g==",
      "dev": true,
      "license": "MIT",
      "dependencies": {
        "@babel/compat-data": "^7.29.7",
        "@babel/helper-validator-option": "^7.29.7",
        "browserslist": "^4.24.0",
        "lru-cache": "^5.1.1",
        "semver": "^6.3.1"
      },
      "engines": {
        "node": ">=6.9.0"
      }
    },
    "node_modules/@babel/helper-globals": {
      "version": "7.29.7",
      "resolved": "https://registry.npmjs.org/@babel/helper-globals/-/helper-globals-7.29.7.tgz",
      "integrity": "sha512-3nQVUAtvkKH9zahfWgw96Jc/uFOmjACE1kQz82E2lqWmHBgjzbNlsC22nuQTfahmWeQtTq5nQ/4Nnd2A1wj4zA==",
      "license": "MIT",
      "engines": {
        "node": ">=6.9.0"
      }
    },
    "node_modules/@babel/helper-module-imports": {
      "version": "7.29.7",
      "resolved": "https://registry.npmjs.org/@babel/helper-module-imports/-/helper-module-imports-7.29.7.tgz",
      "integrity": "sha512-ejHwrQQYcm9xnTivShn2IDOlIzInN34AXskvq9QicvCtEzq1Vzclu/tKF8Jq1Cg8JG2GL6/EmjgsCT7lXepE3g==",
      "dev": true,
      "license": "MIT",
      "dependencies": {
        "@babel/traverse": "^7.29.7",
        "@babel/types": "^7.29.7"
      },
      "engines": {
        "node": ">=6.9.0"
      }
    },
    "node_modules/@babel/helper-module-transforms": {
      "version": "7.29.7",
      "resolved": "https://registry.npmjs.org/@babel/helper-module-transforms/-/helper-module-transforms-7.29.7.tgz",
      "integrity": "sha512-UPUVSyXbOh627KiCIGQSgwWzGeBKLkaJ9PJEdrngIwMSzxLR4jS4+f1f1jb7VzBbg8nFLaYotvVPFCTqdrmTAg==",
      "dev": true,
      "license": "MIT",
      "dependencies": {
        "@babel/helper-module-imports": "^7.29.7",
        "@babel/helper-validator-identifier": "^7.29.7",
        "@babel/traverse": "^7.29.7"
      },
      "engines": {
        "node": ">=6.9.0"
      },
      "peerDependencies": {
        "@babel/core": "^7.0.0"
      }
    },
    "node_modules/@babel/helper-plugin-utils": {
      "version": "7.28.6",
      "resolved": "https://registry.npmjs.org/@babel/helper-plugin-utils/-/helper-plugin-utils-7.28.6.tgz",
      "integrity": "sha512-S9gzZ/bz83GRysI7gAD4wPT/AI3uCnY+9xn+Mx/KPs2JwHJIz1W8PZkg2cqyt3RNOBM8ejcXhV6y8Og7ly/Dug==",
      "dev": true,
      "license": "MIT",
      "engines": {
        "node": ">=6.9.0"
      }
    },
    "node_modules/@babel/helper-string-parser": {
      "version": "7.29.7",
      "resolved": "https://registry.npmjs.org/@babel/helper-string-parser/-/helper-string-parser-7.29.7.tgz",
      "integrity": "sha512-Pb5ijPrZ89GDH8223L4UP8i6QApWxs04RbPQJTeWDV0/keR2E36MeKnyr6LYmUUvqRRI+Iv87SuF1W6ErINzYw==",
      "license": "MIT",
      "engines": {
        "node": ">=6.9.0"
      }
    },
    "node_modules/@babel/helper-validator-identifier": {
      "version": "7.29.7",
      "resolved": "https://registry.npmjs.org/@babel/helper-validator-identifier/-/helper-validator-identifier-7.29.7.tgz",
      "integrity": "sha512-qehxGkRj55h/ff8EMaJ+cYhyaKlHIxqYDn682wQD7RNp9UujOQsHog2uS0r2vzr4pW+sXf90NeeayjcNaX3fFg==",
      "license": "MIT",
      "engines": {
        "node": ">=6.9.0"
      }
    },
    "node_modules/@babel/helper-validator-option": {
      "version": "7.29.7",
      "resolved": "https://registry.npmjs.org/@babel/helper-validator-option/-/helper-validator-option-7.29.7.tgz",
      "integrity": "sha512-N9ZErrD+yW5geCDtBqnOoxmR8+tNKiGuxKlDpuJxfsqpa2dFcexaziGAE/qoHLiDDreVNMupxGmSoNlyvsA3gw==",
      "dev": true,
      "license": "MIT",
      "engines": {
        "node": ">=6.9.0"
      }
    },
    "node_modules/@babel/helpers": {
      "version": "7.29.7",
      "resolved": "https://registry.npmjs.org/@babel/helpers/-/helpers-7.29.7.tgz",
      "integrity": "sha512-1k2lAGRMfHTcwuNYcCNUmaUffmQv8KWMfh2iJUUeRlwlwH4FdNG7mfPI10NPfLHJFThE4Tyr4mv7kTNZOiPuBg==",
      "dev": true,
      "license": "MIT",
      "dependencies": {
        "@babel/template": "^7.29.7",
        "@babel/types": "^7.29.7"
      },
      "engines": {
        "node": ">=6.9.0"
      }
    },
    "node_modules/@babel/parser": {
      "version": "7.29.7",
      "resolved": "https://registry.npmjs.org/@babel/parser/-/parser-7.29.7.tgz",
      "integrity": "sha512-hnORnjP/1P/zFEndoeX+n+t1RwWRJiJpM/jO7FW32Kn9r5+sJB2JWOdYo4L6k78j15eCwY3Gm/7364B1EMwtNg==",
      "license": "MIT",
      "dependencies": {
        "@babel/types": "^7.29.7"
      },
      "bin": {
        "parser": "bin/babel-parser.js"
      },
      "engines": {
        "node": ">=6.0.0"
      }
    },
    "node_modules/@babel/plugin-transform-react-jsx-self": {
      "version": "7.27.1",
      "resolved": "https://registry.npmjs.org/@babel/plugin-transform-react-jsx-self/-/plugin-transform-react-jsx-self-7.27.1.tgz",
      "integrity": "sha512-6UzkCs+ejGdZ5mFFC/OCUrv028ab2fp1znZmCZjAOBKiBK2jXD1O+BPSfX8X2qjJ75fZBMSnQn3Rq2mrBJK2mw==",
      "dev": true,
      "license": "MIT",
      "dependencies": {
        "@babel/helper-plugin-utils": "^7.27.1"
      },
      "engines": {
        "node": ">=6.9.0"
      },
      "peerDependencies": {
        "@babel/core": "^7.0.0-0"
      }
    },
    "node_modules/@babel/plugin-transform-react-jsx-source": {
      "version": "7.27.1",
      "resolved": "https://registry.npmjs.org/@babel/plugin-transform-react-jsx-source/-/plugin-transform-react-jsx-source-7.27.1.tgz",
      "integrity": "sha512-zbwoTsBruTeKB9hSq73ha66iFeJHuaFkUbwvqElnygoNbj/jHRsSeokowZFN3CZ64IvEqcmmkVe89OPXc7ldAw==",
      "dev": true,
      "license": "MIT",
      "dependencies": {
        "@babel/helper-plugin-utils": "^7.27.1"
      },
      "engines": {
        "node": ">=6.9.0"
      },
      "peerDependencies": {
        "@babel/core": "^7.0.0-0"
      }
    },
    "node_modules/@babel/runtime": {
      "version": "7.28.6",
      "resolved": "https://registry.npmjs.org/@babel/runtime/-/runtime-7.28.6.tgz",
      "integrity": "sha512-05WQkdpL9COIMz4LjTxGpPNCdlpyimKppYNoJ5Di5EUObifl8t4tuLuUBBZEpoLYOmfvIWrsp9fCl0HoPRVTdA==",
      "license": "MIT",
      "engines": {
        "node": ">=6.9.0"
      }
    },
    "node_modules/@babel/template": {
      "version": "7.29.7",
      "resolved": "https://registry.npmjs.org/@babel/template/-/template-7.29.7.tgz",
      "integrity": "sha512-puq+Gf35oI24FeN11LkoUQFqv9uwNeWpxXZi/Ji3rRIoKAzKnxRaZ+Gkj0vKS9ZCiTESfng1N9LyOyXvo+m+Gg==",
      "license": "MIT",
      "dependencies": {
        "@babel/code-frame": "^7.29.7",
        "@babel/parser": "^7.29.7",
        "@babel/types": "^7.29.7"
      },
      "engines": {
        "node": ">=6.9.0"
      }
    },
    "node_modules/@babel/traverse": {
      "version": "7.29.7",
      "resolved": "https://registry.npmjs.org/@babel/traverse/-/traverse-7.29.7.tgz",
      "integrity": "sha512-EhlfNQtZ+NK22w5BM61ciuiq1m58ed33Wr1Xan//ZRTy6hgjnwyCffRYwzsGXdASJSUJ1guZILsErh1eQcl+zw==",
      "license": "MIT",
      "dependencies": {
        "@babel/code-frame": "^7.29.7",
        "@babel/generator": "^7.29.7",
        "@babel/helper-globals": "^7.29.7",
        "@babel/parser": "^7.29.7",
        "@babel/template": "^7.29.7",
        "@babel/types": "^7.29.7",
        "debug": "^4.3.1"
      },
      "engines": {
        "node": ">=6.9.0"
      }
    },
    "node_modules/@babel/types": {
      "version": "7.29.7",
      "resolved": "https://registry.npmjs.org/@babel/types/-/types-7.29.7.tgz",
      "integrity": "sha512-4zBIxpPzowiZpusoFkyGVwakdRJUyuH5PxQ/PrqghfdFWWasvnCdPfQXHrenDai+gyLARulZjZowCOj6fjT4pA==",
      "license": "MIT",
      "dependencies": {
        "@babel/helper-string-parser": "^7.29.7",
        "@babel/helper-validator-identifier": "^7.29.7"
      },
      "engines": {
        "node": ">=6.9.0"
      }
    },
    "node_modules/@base44/sdk": {
      "version": "0.8.40",
      "resolved": "https://registry.npmjs.org/@base44/sdk/-/sdk-0.8.40.tgz",
      "integrity": "sha512-eU9M5yo3EEbvbLqZrLo70I1RWC+TkV+zQ9KGXuyXF4pQX2rLiB5IVL5LwUZMnOwiMjr2kga+9UEMc5Kv+6vSzQ==",
      "license": "MIT",
      "dependencies": {
        "axios": "^1.18.1",
        "socket.io-client": "^4.8.3",
        "uuid": "^13.0.2"
      }
    },
    "node_modules/@base44/vite-plugin": {
      "version": "1.0.30",
      "resolved": "https://registry.npmjs.org/@base44/vite-plugin/-/vite-plugin-1.0.30.tgz",
      "integrity": "sha512-KFO+HP3TUf/2vg5cW0LFV7/nHHQyAYqXqPi6jq/hQB64JWhvZBXLlQIwQU0y5mu0JVliFOgLNcwHdwC8J+ekjg==",
      "license": "MIT",
      "dependencies": {
        "@babel/generator": "^7.28.5",
        "@babel/parser": "^7.28.5",
        "@babel/traverse": "^7.28.5",
        "@babel/types": "^7.28.5"
      }
    },
    "node_modules/@esbuild/aix-ppc64": {
      "version": "0.25.12",
      "resolved": "https://registry.npmjs.org/@esbuild/aix-ppc64/-/aix-ppc64-0.25.12.tgz",
      "integrity": "sha512-Hhmwd6CInZ3dwpuGTF8fJG6yoWmsToE+vYgD4nytZVxcu1ulHpUQRAB1UJ8+N1Am3Mz4+xOByoQoSZf4D+CpkA==",
      "cpu": [
        "ppc64"
      ],
      "dev": true,
      "license": "MIT",
      "optional": true,
      "os": [
        "aix"
      ],
      "engines": {
        "node": ">=18"
      }
    },
    "node_modules/@esbuild/android-arm": {
      "version": "0.25.12",
      "resolved": "https://registry.npmjs.org/@esbuild/android-arm/-/android-arm-0.25.12.tgz",
      "integrity": "sha512-VJ+sKvNA/GE7Ccacc9Cha7bpS8nyzVv0jdVgwNDaR4gDMC/2TTRc33Ip8qrNYUcpkOHUT5OZ0bUcNNVZQ9RLlg==",
      "cpu": [
        "arm"
      ],
      "dev": true,
      "license": "MIT",
      "optional": true,
      "os": [
        "android"
      ],
      "engines": {
        "node": ">=18"
      }
    },
    "node_modules/@esbuild/android-arm64": {
      "version": "0.25.12",
      "resolved": "https://registry.npmjs.org/@esbuild/android-arm64/-/android-arm64-0.25.12.tgz",
      "integrity": "sha512-6AAmLG7zwD1Z159jCKPvAxZd4y/VTO0VkprYy+3N2FtJ8+BQWFXU+OxARIwA46c5tdD9SsKGZ/1ocqBS/gAKHg==",
      "cpu": [
        "arm64"
      ],
      "dev": true,
      "license": "MIT",
      "optional": true,
      "os": [
        "android"
      ],
      "engines": {
        "node": ">=18"
      }
    },
    "node_modules/@esbuild/android-x64": {
      "version": "0.25.12",
      "resolved": "https://registry.npmjs.org/@esbuild/android-x64/-/android-x64-0.25.12.tgz",
      "integrity": "sha512-5jbb+2hhDHx5phYR2By8GTWEzn6I9UqR11Kwf22iKbNpYrsmRB18aX/9ivc5cabcUiAT/wM+YIZ6SG9QO6a8kg==",
      "cpu": [
        "x64"
      ],
      "dev": true,
      "license": "MIT",
      "optional": true,
      "os": [
        "android"
      ],
      "engines": {
        "node": ">=18"
      }
    },
    "node_modules/@esbuild/darwin-arm64": {
      "version": "0.25.12",
      "resolved": "https://registry.npmjs.org/@esbuild/darwin-arm64/-/darwin-arm64-0.25.12.tgz",
      "integrity": "sha512-N3zl+lxHCifgIlcMUP5016ESkeQjLj/959RxxNYIthIg+CQHInujFuXeWbWMgnTo4cp5XVHqFPmpyu9J65C1Yg==",
      "cpu": [
        "arm64"
      ],
      "dev": true,
      "license": "MIT",
      "optional": true,
      "os": [
        "darwin"
      ],
      "engines": {
        "node": ">=18"
      }
    },
    "node_modules/@esbuild/darwin-x64": {
      "version": "0.25.12",
      "resolved": "https://registry.npmjs.org/@esbuild/darwin-x64/-/darwin-x64-0.25.12.tgz",
      "integrity": "sha512-HQ9ka4Kx21qHXwtlTUVbKJOAnmG1ipXhdWTmNXiPzPfWKpXqASVcWdnf2bnL73wgjNrFXAa3yYvBSd9pzfEIpA==",
      "cpu": [
        "x64"
      ],
      "dev": true,
      "license": "MIT",
      "optional": true,
      "os": [
        "darwin"
      ],
      "engines": {
        "node": ">=18"
      }
    },
    "node_modules/@esbuild/freebsd-arm64": {
      "version": "0.25.12",
      "resolved": "https://registry.npmjs.org/@esbuild/freebsd-arm64/-/freebsd-arm64-0.25.12.tgz",
      "integrity": "sha512-gA0Bx759+7Jve03K1S0vkOu5Lg/85dou3EseOGUes8flVOGxbhDDh/iZaoek11Y8mtyKPGF3vP8XhnkDEAmzeg==",
      "cpu": [
        "arm64"
      ],
      "dev": true,
      "license": "MIT",
      "optional": true,
      "os": [
        "freebsd"
      ],
      "engines": {
        "node": ">=18"
      }
    },
    "node_modules/@esbuild/freebsd-x64": {
      "version": "0.25.12",
      "resolved": "https://registry.npmjs.org/@esbuild/freebsd-x64/-/freebsd-x64-0.25.12.tgz",
      "integrity": "sha512-TGbO26Yw2xsHzxtbVFGEXBFH0FRAP7gtcPE7P5yP7wGy7cXK2oO7RyOhL5NLiqTlBh47XhmIUXuGciXEqYFfBQ==",
      "cpu": [
        "x64"
      ],
      "dev": true,
      "license": "MIT",
      "optional": true,
      "os": [
        "freebsd"
      ],
      "engines": {
        "node": ">=18"
      }
    },
    "node_modules/@esbuild/linux-arm": {
      "version": "0.25.12",
      "resolved": "https://registry.npmjs.org/@esbuild/linux-arm/-/linux-arm-0.25.12.tgz",
      "integrity": "sha512-lPDGyC1JPDou8kGcywY0YILzWlhhnRjdof3UlcoqYmS9El818LLfJJc3PXXgZHrHCAKs/Z2SeZtDJr5MrkxtOw==",
      "cpu": [
        "arm"
      ],
      "dev": true,
      "license": "MIT",
      "optional": true,
      "os": [
        "linux"
      ],
      "engines": {
        "node": ">=18"
      }
    },
    "node_modules/@esbuild/linux-arm64": {
      "version": "0.25.12",
      "resolved": "https://registry.npmjs.org/@esbuild/linux-arm64/-/linux-arm64-0.25.12.tgz",
      "integrity": "sha512-8bwX7a8FghIgrupcxb4aUmYDLp8pX06rGh5HqDT7bB+8Rdells6mHvrFHHW2JAOPZUbnjUpKTLg6ECyzvas2AQ==",
      "cpu": [
        "arm64"
      ],
      "dev": true,
      "license": "MIT",
      "optional": true,
      "os": [
        "linux"
      ],
      "engines": {
        "node": ">=18"
      }
    },
    "node_modules/@esbuild/linux-ia32": {
      "version": "0.25.12",
      "resolved": "https://registry.npmjs.org/@esbuild/linux-ia32/-/linux-ia32-0.25.12.tgz",
      "integrity": "sha512-0y9KrdVnbMM2/vG8KfU0byhUN+EFCny9+8g202gYqSSVMonbsCfLjUO+rCci7pM0WBEtz+oK/PIwHkzxkyharA==",
      "cpu": [
        "ia32"
      ],
      "dev": true,
      "license": "MIT",
      "optional": true,
      "os": [
        "linux"
      ],
      "engines": {
        "node": ">=18"
      }
    },
    "node_modules/@esbuild/linux-loong64": {
      "version": "0.25.12",
      "resolved": "https://registry.npmjs.org/@esbuild/linux-loong64/-/linux-loong64-0.25.12.tgz",
      "integrity": "sha512-h///Lr5a9rib/v1GGqXVGzjL4TMvVTv+s1DPoxQdz7l/AYv6LDSxdIwzxkrPW438oUXiDtwM10o9PmwS/6Z0Ng==",
      "cpu": [
        "loong64"
      ],
      "dev": true,
      "license": "MIT",
      "optional": true,
      "os": [
        "linux"
      ],
      "engines": {
        "node": ">=18"
      }
    },
    "node_modules/@esbuild/linux-mips64el": {
      "version": "0.25.12",
      "resolved": "https://registry.npmjs.org/@esbuild/linux-mips64el/-/linux-mips64el-0.25.12.tgz",
      "integrity": "sha512-iyRrM1Pzy9GFMDLsXn1iHUm18nhKnNMWscjmp4+hpafcZjrr2WbT//d20xaGljXDBYHqRcl8HnxbX6uaA/eGVw==",
      "cpu": [
        "mips64el"
      ],
      "dev": true,
      "license": "MIT",
      "optional": true,
      "os": [
        "linux"
      ],
      "engines": {
        "node": ">=18"
      }
    },
    "node_modules/@esbuild/linux-ppc64": {
      "version": "0.25.12",
      "resolved": "https://registry.npmjs.org/@esbuild/linux-ppc64/-/linux-ppc64-0.25.12.tgz",
      "integrity": "sha512-9meM/lRXxMi5PSUqEXRCtVjEZBGwB7P/D4yT8UG/mwIdze2aV4Vo6U5gD3+RsoHXKkHCfSxZKzmDssVlRj1QQA==",
      "cpu": [
        "ppc64"
      ],
      "dev": true,
      "license": "MIT",
      "optional": true,
      "os": [
        "linux"
      ],
      "engines": {
        "node": ">=18"
      }
    },
    "node_modules/@esbuild/linux-riscv64": {
      "version": "0.25.12",
      "resolved": "https://registry.npmjs.org/@esbuild/linux-riscv64/-/linux-riscv64-0.25.12.tgz",
      "integrity": "sha512-Zr7KR4hgKUpWAwb1f3o5ygT04MzqVrGEGXGLnj15YQDJErYu/BGg+wmFlIDOdJp0PmB0lLvxFIOXZgFRrdjR0w==",
      "cpu": [
        "riscv64"
      ],
      "dev": true,
      "license": "MIT",
      "optional": true,
      "os": [
        "linux"
      ],
      "engines": {
        "node": ">=18"
      }
    },
    "node_modules/@esbuild/linux-s390x": {
      "version": "0.25.12",
      "resolved": "https://registry.npmjs.org/@esbuild/linux-s390x/-/linux-s390x-0.25.12.tgz",
      "integrity": "sha512-MsKncOcgTNvdtiISc/jZs/Zf8d0cl/t3gYWX8J9ubBnVOwlk65UIEEvgBORTiljloIWnBzLs4qhzPkJcitIzIg==",
      "cpu": [
        "s390x"
      ],
      "dev": true,
      "license": "MIT",
      "optional": true,
      "os": [
        "linux"
      ],
      "engines": {
        "node": ">=18"
      }
    },
    "node_modules/@esbuild/linux-x64": {
      "version": "0.25.12",
      "resolved": "https://registry.npmjs.org/@esbuild/linux-x64/-/linux-x64-0.25.12.tgz",
      "integrity": "sha512-uqZMTLr/zR/ed4jIGnwSLkaHmPjOjJvnm6TVVitAa08SLS9Z0VM8wIRx7gWbJB5/J54YuIMInDquWyYvQLZkgw==",
      "cpu": [
        "x64"
      ],
      "dev": true,
      "license": "MIT",
      "optional": true,
      "os": [
        "linux"
      ],
      "engines": {
        "node": ">=18"
      }
    },
    "node_modules/@esbuild/netbsd-arm64": {
      "version": "0.25.12",
      "resolved": "https://registry.npmjs.org/@esbuild/netbsd-arm64/-/netbsd-arm64-0.25.12.tgz",
      "integrity": "sha512-xXwcTq4GhRM7J9A8Gv5boanHhRa/Q9KLVmcyXHCTaM4wKfIpWkdXiMog/KsnxzJ0A1+nD+zoecuzqPmCRyBGjg==",
      "cpu": [
        "arm64"
      ],
      "dev": true,
      "license": "MIT",
      "optional": true,
      "os": [
        "netbsd"
      ],
      "engines": {
        "node": ">=18"
      }
    },
    "node_modules/@esbuild/netbsd-x64": {
      "version": "0.25.12",
      "resolved": "https://registry.npmjs.org/@esbuild/netbsd-x64/-/netbsd-x64-0.25.12.tgz",
      "integrity": "sha512-Ld5pTlzPy3YwGec4OuHh1aCVCRvOXdH8DgRjfDy/oumVovmuSzWfnSJg+VtakB9Cm0gxNO9BzWkj6mtO1FMXkQ==",
      "cpu": [
        "x64"
      ],
      "dev": true,
      "license": "MIT",
      "optional": true,
      "os": [
        "netbsd"
      ],
      "engines": {
        "node": ">=18"
      }
    },
    "node_modules/@esbuild/openbsd-arm64": {
      "version": "0.25.12",
      "resolved": "https://registry.npmjs.org/@esbuild/openbsd-arm64/-/openbsd-arm64-0.25.12.tgz",
      "integrity": "sha512-fF96T6KsBo/pkQI950FARU9apGNTSlZGsv1jZBAlcLL1MLjLNIWPBkj5NlSz8aAzYKg+eNqknrUJ24QBybeR5A==",
      "cpu": [
        "arm64"
      ],
      "dev": true,
      "license": "MIT",
      "optional": true,
      "os": [
        "openbsd"
      ],
      "engines": {
        "node": ">=18"
      }
    },
    "node_modules/@esbuild/openbsd-x64": {
      "version": "0.25.12",
      "resolved": "https://registry.npmjs.org/@esbuild/openbsd-x64/-/openbsd-x64-0.25.12.tgz",
      "integrity": "sha512-MZyXUkZHjQxUvzK7rN8DJ3SRmrVrke8ZyRusHlP+kuwqTcfWLyqMOE3sScPPyeIXN/mDJIfGXvcMqCgYKekoQw==",
      "cpu": [
        "x64"
      ],
      "dev": true,
      "license": "MIT",
      "optional": true,
      "os": [
        "openbsd"
      ],
      "engines": {
        "node": ">=18"
      }
    },
    "node_modules/@esbuild/openharmony-arm64": {
      "version": "0.25.12",
      "resolved": "https://registry.npmjs.org/@esbuild/openharmony-arm64/-/openharmony-arm64-0.25.12.tgz",
      "integrity": "sha512-rm0YWsqUSRrjncSXGA7Zv78Nbnw4XL6/dzr20cyrQf7ZmRcsovpcRBdhD43Nuk3y7XIoW2OxMVvwuRvk9XdASg==",
      "cpu": [
        "arm64"
      ],
      "dev": true,
      "license": "MIT",
      "optional": true,
      "os": [
        "openharmony"
      ],
      "engines": {
        "node": ">=18"
      }
    },
    "node_modules/@esbuild/sunos-x64": {
      "version": "0.25.12",
      "resolved": "https://registry.npmjs.org/@esbuild/sunos-x64/-/sunos-x64-0.25.12.tgz",
      "integrity": "sha512-3wGSCDyuTHQUzt0nV7bocDy72r2lI33QL3gkDNGkod22EsYl04sMf0qLb8luNKTOmgF/eDEDP5BFNwoBKH441w==",
      "cpu": [
        "x64"
      ],
      "dev": true,
      "license": "MIT",
      "optional": true,
      "os": [
        "sunos"
      ],
      "engines": {
        "node": ">=18"
      }
    },
    "node_modules/@esbuild/win32-arm64": {
      "version": "0.25.12",
      "resolved": "https://registry.npmjs.org/@esbuild/win32-arm64/-/win32-arm64-0.25.12.tgz",
      "integrity": "sha512-rMmLrur64A7+DKlnSuwqUdRKyd3UE7oPJZmnljqEptesKM8wx9J8gx5u0+9Pq0fQQW8vqeKebwNXdfOyP+8Bsg==",
      "cpu": [
        "arm64"
      ],
      "dev": true,
      "license": "MIT",
      "optional": true,
      "os": [
        "win32"
      ],
      "engines": {
        "node": ">=18"
      }
    },
    "node_modules/@esbuild/win32-ia32": {
      "version": "0.25.12",
      "resolved": "https://registry.npmjs.org/@esbuild/win32-ia32/-/win32-ia32-0.25.12.tgz",
      "integrity": "sha512-HkqnmmBoCbCwxUKKNPBixiWDGCpQGVsrQfJoVGYLPT41XWF8lHuE5N6WhVia2n4o5QK5M4tYr21827fNhi4byQ==",
      "cpu": [
        "ia32"
      ],
      "dev": true,
      "license": "MIT",
      "optional": true,
      "os": [
        "win32"
      ],
      "engines": {
        "node": ">=18"
      }
    },
    "node_modules/@esbuild/win32-x64": {
      "version": "0.25.12",
      "resolved": "https://registry.npmjs.org/@esbuild/win32-x64/-/win32-x64-0.25.12.tgz",
      "integrity": "sha512-alJC0uCZpTFrSL0CCDjcgleBXPnCrEAhTBILpeAp7M/OFgoqtAetfBzX0xM00MUsVVPpVjlPuMbREqnZCXaTnA==",
      "cpu": [
        "x64"
      ],
      "dev": true,
      "license": "MIT",
      "optional": true,
      "os": [
        "win32"
      ],
      "engines": {
        "node": ">=18"
      }
    },
    "node_modules/@eslint-community/eslint-utils": {
      "version": "4.9.1",
      "resolved": "https://registry.npmjs.org/@eslint-community/eslint-utils/-/eslint-utils-4.9.1.tgz",
      "integrity": "sha512-phrYmNiYppR7znFEdqgfWHXR6NCkZEK7hwWDHZUjit/2/U0r6XvkDl0SYnoM51Hq7FhCGdLDT6zxCCOY1hexsQ==",
      "dev": true,
      "license": "MIT",
      "dependencies": {
        "eslint-visitor-keys": "^3.4.3"
      },
      "engines": {
        "node": "^12.22.0 || ^14.17.0 || >=16.0.0"
      },
      "funding": {
        "url": "https://opencollective.com/eslint"
      },
      "peerDependencies": {
        "eslint": "^6.0.0 || ^7.0.0 || >=8.0.0"
      }
    },
    "node_modules/@eslint-community/eslint-utils/node_modules/eslint-visitor-keys": {
      "version": "3.4.3",
      "resolved": "https://registry.npmjs.org/eslint-visitor-keys/-/eslint-visitor-keys-3.4.3.tgz",
      "integrity": "sha512-wpc+LXeiyiisxPlEkUzU6svyS1frIO3Mgxj1fdy7Pm8Ygzguax2N3Fa/D/ag1WqbOprdI+uY6wMUl8/a2G+iag==",
      "dev": true,
      "license": "Apache-2.0",
      "engines": {
        "node": "^12.22.0 || ^14.17.0 || >=16.0.0"
      },
      "funding": {
        "url": "https://opencollective.com/eslint"
      }
    },
    "node_modules/@eslint-community/regexpp": {
      "version": "4.12.2",
      "resolved": "https://registry.npmjs.org/@eslint-community/regexpp/-/regexpp-4.12.2.tgz",
      "integrity": "sha512-EriSTlt5OC9/7SXkRSCAhfSxxoSUgBm33OH+IkwbdpgoqsSsUg7y3uh+IICI/Qg4BBWr3U2i39RpmycbxMq4ew==",
      "dev": true,
      "license": "MIT",
      "engines": {
        "node": "^12.0.0 || ^14.0.0 || >=16.0.0"
      }
    },
    "node_modules/@eslint/config-array": {
      "version": "0.21.1",
      "resolved": "https://registry.npmjs.org/@eslint/config-array/-/config-array-0.21.1.tgz",
      "integrity": "sha512-aw1gNayWpdI/jSYVgzN5pL0cfzU02GT3NBpeT/DXbx1/1x7ZKxFPd9bwrzygx/qiwIQiJ1sw/zD8qY/kRvlGHA==",
      "dev": true,
      "license": "Apache-2.0",
      "dependencies": {
        "@eslint/object-schema": "^2.1.7",
        "debug": "^4.3.1",
        "minimatch": "^3.1.2"
      },
      "engines": {
        "node": "^18.18.0 || ^20.9.0 || >=21.1.0"
      }
    },
    "node_modules/@eslint/config-helpers": {
      "version": "0.4.2",
      "resolved": "https://registry.npmjs.org/@eslint/config-helpers/-/config-helpers-0.4.2.tgz",
      "integrity": "sha512-gBrxN88gOIf3R7ja5K9slwNayVcZgK6SOUORm2uBzTeIEfeVaIhOpCtTox3P6R7o2jLFwLFTLnC7kU/RGcYEgw==",
      "dev": true,
      "license": "Apache-2.0",
      "dependencies": {
        "@eslint/core": "^0.17.0"
      },
      "engines": {
        "node": "^18.18.0 || ^20.9.0 || >=21.1.0"
      }
    },
    "node_modules/@eslint/core": {
      "version": "0.17.0",
      "resolved": "https://registry.npmjs.org/@eslint/core/-/core-0.17.0.tgz",
      "integrity": "sha512-yL/sLrpmtDaFEiUj1osRP4TI2MDz1AddJL+jZ7KSqvBuliN4xqYY54IfdN8qD8Toa6g1iloph1fxQNkjOxrrpQ==",
      "dev": true,
      "license": "Apache-2.0",
      "dependencies": {
        "@types/json-schema": "^7.0.15"
      },
      "engines": {
        "node": "^18.18.0 || ^20.9.0 || >=21.1.0"
      }
    },
    "node_modules/@eslint/eslintrc": {
      "version": "3.3.3",
      "resolved": "https://registry.npmjs.org/@eslint/eslintrc/-/eslintrc-3.3.3.tgz",
      "integrity": "sha512-Kr+LPIUVKz2qkx1HAMH8q1q6azbqBAsXJUxBl/ODDuVPX45Z9DfwB8tPjTi6nNZ8BuM3nbJxC5zCAg5elnBUTQ==",
      "dev": true,
      "license": "MIT",
      "dependencies": {
        "ajv": "^6.12.4",
        "debug": "^4.3.2",
        "espree": "^10.0.1",
        "globals": "^14.0.0",
        "ignore": "^5.2.0",
        "import-fresh": "^3.2.1",
        "js-yaml": "^4.1.1",
        "minimatch": "^3.1.2",
        "strip-json-comments": "^3.1.1"
      },
      "engines": {
        "node": "^18.18.0 || ^20.9.0 || >=21.1.0"
      },
      "funding": {
        "url": "https://opencollective.com/eslint"
      }
    },
    "node_modules/@eslint/eslintrc/node_modules/globals": {
      "version": "14.0.0",
      "resolved": "https://registry.npmjs.org/globals/-/globals-14.0.0.tgz",
      "integrity": "sha512-oahGvuMGQlPw/ivIYBjVSrWAfWLBeku5tpPE2fOPLi+WHffIWbuh2tCjhyQhTBPMf5E9jDEH4FOmTYgYwbKwtQ==",
      "dev": true,
      "license": "MIT",
      "engines": {
        "node": ">=18"
      },
      "funding": {
        "url": "https://github.com/sponsors/sindresorhus"
      }
    },
    "node_modules/@eslint/js": {
      "version": "9.39.2",
      "resolved": "https://registry.npmjs.org/@eslint/js/-/js-9.39.2.tgz",
      "integrity": "sha512-q1mjIoW1VX4IvSocvM/vbTiveKC4k9eLrajNEuSsmjymSDEbpGddtpfOoN7YGAqBK3NG+uqo8ia4PDTt8buCYA==",
      "dev": true,
      "license": "MIT",
      "engines": {
        "node": "^18.18.0 || ^20.9.0 || >=21.1.0"
      },
      "funding": {
        "url": "https://eslint.org/donate"
      }
    },
    "node_modules/@eslint/object-schema": {
      "version": "2.1.7",
      "resolved": "https://registry.npmjs.org/@eslint/object-schema/-/object-schema-2.1.7.tgz",
      "integrity": "sha512-VtAOaymWVfZcmZbp6E2mympDIHvyjXs/12LqWYjVw6qjrfF+VK+fyG33kChz3nnK+SU5/NeHOqrTEHS8sXO3OA==",
      "dev": true,
      "license": "Apache-2.0",
      "engines": {
        "node": "^18.18.0 || ^20.9.0 || >=21.1.0"
      }
    },
    "node_modules/@eslint/plugin-kit": {
      "version": "0.4.1",
      "resolved": "https://registry.npmjs.org/@eslint/plugin-kit/-/plugin-kit-0.4.1.tgz",
      "integrity": "sha512-43/qtrDUokr7LJqoF2c3+RInu/t4zfrpYdoSDfYyhg52rwLV6TnOvdG4fXm7IkSB3wErkcmJS9iEhjVtOSEjjA==",
      "dev": true,
      "license": "Apache-2.0",
      "dependencies": {
        "@eslint/core": "^0.17.0",
        "levn": "^0.4.1"
      },
      "engines": {
        "node": "^18.18.0 || ^20.9.0 || >=21.1.0"
      }
    },
    "node_modules/@floating-ui/core": {
      "version": "1.7.4",
      "resolved": "https://registry.npmjs.org/@floating-ui/core/-/core-1.7.4.tgz",
      "integrity": "sha512-C3HlIdsBxszvm5McXlB8PeOEWfBhcGBTZGkGlWc2U0KFY5IwG5OQEuQ8rq52DZmcHDlPLd+YFBK+cZcytwIFWg==",
      "license": "MIT",
      "dependencies": {
        "@floating-ui/utils": "^0.2.10"
      }
    },
    "node_modules/@floating-ui/dom": {
      "version": "1.7.5",
      "resolved": "https://registry.npmjs.org/@floating-ui/dom/-/dom-1.7.5.tgz",
      "integrity": "sha512-N0bD2kIPInNHUHehXhMke1rBGs1dwqvC9O9KYMyyjK7iXt7GAhnro7UlcuYcGdS/yYOlq0MAVgrow8IbWJwyqg==",
      "license": "MIT",
      "dependencies": {
        "@floating-ui/core": "^1.7.4",
        "@floating-ui/utils": "^0.2.10"
      }
    },
    "node_modules/@floating-ui/react-dom": {
      "version": "2.1.7",
      "resolved": "https://registry.npmjs.org/@floating-ui/react-dom/-/react-dom-2.1.7.tgz",
      "integrity": "sha512-0tLRojf/1Go2JgEVm+3Frg9A3IW8bJgKgdO0BN5RkF//ufuz2joZM63Npau2ff3J6lUVYgDSNzNkR+aH3IVfjg==",
      "license": "MIT",
      "dependencies": {
        "@floating-ui/dom": "^1.7.5"
      },
      "peerDependencies": {
        "react": ">=16.8.0",
        "react-dom": ">=16.8.0"
      }
    },
    "node_modules/@floating-ui/utils": {
      "version": "0.2.10",
      "resolved": "https://registry.npmjs.org/@floating-ui/utils/-/utils-0.2.10.tgz",
      "integrity": "sha512-aGTxbpbg8/b5JfU1HXSrbH3wXZuLPJcNEcZQFMxLs3oSzgtVu6nFPkbbGGUvBcUjKV2YyB9Wxxabo+HEH9tcRQ==",
      "license": "MIT"
    },
    "node_modules/@hello-pangea/dnd": {
      "version": "17.0.0",
      "resolved": "https://registry.npmjs.org/@hello-pangea/dnd/-/dnd-17.0.0.tgz",
      "integrity": "sha512-LDDPOix/5N0j5QZxubiW9T0M0+1PR0rTDWeZF5pu1Tz91UQnuVK4qQ/EjY83Qm2QeX0eM8qDXANfDh3VVqtR4Q==",
      "license": "Apache-2.0",
      "dependencies": {
        "@babel/runtime": "^7.25.6",
        "css-box-model": "^1.2.1",
        "memoize-one": "^6.0.0",
        "raf-schd": "^4.0.3",
        "react-redux": "^9.1.2",
        "redux": "^5.0.1",
        "use-memo-one": "^1.1.3"
      },
      "peerDependencies": {
        "react": "^18.0.0",
        "react-dom": "^18.0.0"
      }
    },
    "node_modules/@hookform/resolvers": {
      "version": "4.1.3",
      "resolved": "https://registry.npmjs.org/@hookform/resolvers/-/resolvers-4.1.3.tgz",
      "integrity": "sha512-Jsv6UOWYTrEFJ/01ZrnwVXs7KDvP8XIo115i++5PWvNkNvkrsTfGiLS6w+eJ57CYtUtDQalUWovCZDHFJ8u1VQ==",
      "license": "MIT",
      "dependencies": {
        "@standard-schema/utils": "^0.3.0"
      },
      "peerDependencies": {
        "react-hook-form": "^7.0.0"
      }
    },
    "node_modules/@humanfs/core": {
      "version": "0.19.1",
      "resolved": "https://registry.npmjs.org/@humanfs/core/-/core-0.19.1.tgz",
      "integrity": "sha512-5DyQ4+1JEUzejeK1JGICcideyfUbGixgS9jNgex5nqkW+cY7WZhxBigmieN5Qnw9ZosSNVC9KQKyb+GUaGyKUA==",
      "dev": true,
      "license": "Apache-2.0",
      "engines": {
        "node": ">=18.18.0"
      }
    },
    "node_modules/@humanfs/node": {
      "version": "0.16.7",
      "resolved": "https://registry.npmjs.org/@humanfs/node/-/node-0.16.7.tgz",
      "integrity": "sha512-/zUx+yOsIrG4Y43Eh2peDeKCxlRt/gET6aHfaKpuq267qXdYDFViVHfMaLyygZOnl0kGWxFIgsBy8QFuTLUXEQ==",
      "dev": true,
      "license": "Apache-2.0",
      "dependencies": {
        "@humanfs/core": "^0.19.1",
        "@humanwhocodes/retry": "^0.4.0"
      },
      "engines": {
        "node": ">=18.18.0"
      }
    },
    "node_modules/@humanwhocodes/module-importer": {
      "version": "1.0.1",
      "resolved": "https://registry.npmjs.org/@humanwhocodes/module-importer/-/module-importer-1.0.1.tgz",
      "integrity": "sha512-bxveV4V8v5Yb4ncFTT3rPSgZBOpCkjfK0y4oVVVJwIuDVBRMDXrPyXRL988i5ap9m9bnyEEjWfm5WkBmtffLfA==",
      "dev": true,
      "license": "Apache-2.0",
      "engines": {
        "node": ">=12.22"
      },
      "funding": {
        "type": "github",
        "url": "https://github.com/sponsors/nzakas"
      }
    },
    "node_modules/@humanwhocodes/retry": {
      "version": "0.4.3",
      "resolved": "https://registry.npmjs.org/@humanwhocodes/retry/-/retry-0.4.3.tgz",
      "integrity": "sha512-bV0Tgo9K4hfPCek+aMAn81RppFKv2ySDQeMoSZuvTASywNTnVJCArCZE2FWqpvIatKu7VMRLWlR1EazvVhDyhQ==",
      "dev": true,
      "license": "Apache-2.0",
      "engines": {
        "node": ">=18.18"
      },
      "funding": {
        "type": "github",
        "url": "https://github.com/sponsors/nzakas"
      }
    },
    "node_modules/@jridgewell/gen-mapping": {
      "version": "0.3.13",
      "resolved": "https://registry.npmjs.org/@jridgewell/gen-mapping/-/gen-mapping-0.3.13.tgz",
      "integrity": "sha512-2kkt/7niJ6MgEPxF0bYdQ6etZaA+fQvDcLKckhy1yIQOzaoKjBBjSj63/aLVjYE3qhRt5dvM+uUyfCg6UKCBbA==",
      "license": "MIT",
      "dependencies": {
        "@jridgewell/sourcemap-codec": "^1.5.0",
        "@jridgewell/trace-mapping": "^0.3.24"
      }
    },
    "node_modules/@jridgewell/remapping": {
      "version": "2.3.5",
      "resolved": "https://registry.npmjs.org/@jridgewell/remapping/-/remapping-2.3.5.tgz",
      "integrity": "sha512-LI9u/+laYG4Ds1TDKSJW2YPrIlcVYOwi2fUC6xB43lueCjgxV4lffOCZCtYFiH6TNOX+tQKXx97T4IKHbhyHEQ==",
      "dev": true,
      "license": "MIT",
      "dependencies": {
        "@jridgewell/gen-mapping": "^0.3.5",
        "@jridgewell/trace-mapping": "^0.3.24"
      }
    },
    "node_modules/@jridgewell/resolve-uri": {
      "version": "3.1.2",
      "resolved": "https://registry.npmjs.org/@jridgewell/resolve-uri/-/resolve-uri-3.1.2.tgz",
      "integrity": "sha512-bRISgCIjP20/tbWSPWMEi54QVPRZExkuD9lJL+UIxUKtwVJA8wW1Trb1jMs1RFXo1CBTNZ/5hpC9QvmKWdopKw==",
      "license": "MIT",
      "engines": {
        "node": ">=6.0.0"
      }
    },
    "node_modules/@jridgewell/sourcemap-codec": {
      "version": "1.5.5",
      "resolved": "https://registry.npmjs.org/@jridgewell/sourcemap-codec/-/sourcemap-codec-1.5.5.tgz",
      "integrity": "sha512-cYQ9310grqxueWbl+WuIUIaiUaDcj7WOq5fVhEljNVgRfOUhY9fy2zTvfoqWsnebh8Sl70VScFbICvJnLKB0Og==",
      "license": "MIT"
    },
    "node_modules/@jridgewell/trace-mapping": {
      "version": "0.3.31",
      "resolved": "https://registry.npmjs.org/@jridgewell/trace-mapping/-/trace-mapping-0.3.31.tgz",
      "integrity": "sha512-zzNR+SdQSDJzc8joaeP8QQoCQr8NuYx2dIIytl1QeBEZHJ9uW6hebsrYgbz8hJwUQao3TWCMtmfV8Nu1twOLAw==",
      "license": "MIT",
      "dependencies": {
        "@jridgewell/resolve-uri": "^3.1.0",
        "@jridgewell/sourcemap-codec": "^1.4.14"
      }
    },
    "node_modules/@nodelib/fs.scandir": {
      "version": "2.1.5",
      "resolved": "https://registry.npmjs.org/@nodelib/fs.scandir/-/fs.scandir-2.1.5.tgz",
      "integrity": "sha512-vq24Bq3ym5HEQm2NKCr3yXDwjc7vTsEThRDnkp2DK9p1uqLR+DHurm/NOTo0KG7HYHU7eppKZj3MyqYuMBf62g==",
      "license": "MIT",
      "dependencies": {
        "@nodelib/fs.stat": "2.0.5",
        "run-parallel": "^1.1.9"
      },
      "engines": {
        "node": ">= 8"
      }
    },
    "node_modules/@nodelib/fs.stat": {
      "version": "2.0.5",
      "resolved": "https://registry.npmjs.org/@nodelib/fs.stat/-/fs.stat-2.0.5.tgz",
      "integrity": "sha512-RkhPPp2zrqDAQA/2jNhnztcPAlv64XdhIp7a7454A5ovI7Bukxgt7MX7udwAu3zg1DcpPU0rz3VV1SeaqvY4+A==",
      "license": "MIT",
      "engines": {
        "node": ">= 8"
      }
    },
    "node_modules/@nodelib/fs.walk": {
      "version": "1.2.8",
      "resolved": "https://registry.npmjs.org/@nodelib/fs.walk/-/fs.walk-1.2.8.tgz",
      "integrity": "sha512-oGB+UxlgWcgQkgwo8GcEGwemoTFt3FIO9ababBmaGwXIoBKZ+GTy0pP185beGg7Llih/NSHSV2XAs1lnznocSg==",
      "license": "MIT",
      "dependencies": {
        "@nodelib/fs.scandir": "2.1.5",
        "fastq": "^1.6.0"
      },
      "engines": {
        "node": ">= 8"
      }
    },
    "node_modules/@radix-ui/number": {
      "version": "1.1.1",
      "resolved": "https://registry.npmjs.org/@radix-ui/number/-/number-1.1.1.tgz",
      "integrity": "sha512-MkKCwxlXTgz6CFoJx3pCwn07GKp36+aZyu/u2Ln2VrA5DcdyCZkASEDBTd8x5whTQQL5CiYf4prXKLcgQdv29g==",
      "license": "MIT"
    },
    "node_modules/@radix-ui/primitive": {
      "version": "1.1.3",
      "resolved": "https://registry.npmjs.org/@radix-ui/primitive/-/primitive-1.1.3.tgz",
      "integrity": "sha512-JTF99U/6XIjCBo0wqkU5sK10glYe27MRRsfwoiq5zzOEZLHU3A3KCMa5X/azekYRCJ0HlwI0crAXS/5dEHTzDg==",
      "license": "MIT"
    },
    "node_modules/@radix-ui/react-accordion": {
      "version": "1.2.12",
      "resolved": "https://registry.npmjs.org/@radix-ui/react-accordion/-/react-accordion-1.2.12.tgz",
      "integrity": "sha512-T4nygeh9YE9dLRPhAHSeOZi7HBXo+0kYIPJXayZfvWOWA0+n3dESrZbjfDPUABkUNym6Hd+f2IR113To8D2GPA==",
      "license": "MIT",
      "dependencies": {
        "@radix-ui/primitive": "1.1.3",
        "@radix-ui/react-collapsible": "1.1.12",
        "@radix-ui/react-collection": "1.1.7",
        "@radix-ui/react-compose-refs": "1.1.2",
        "@radix-ui/react-context": "1.1.2",
        "@radix-ui/react-direction": "1.1.1",
        "@radix-ui/react-id": "1.1.1",
        "@radix-ui/react-primitive": "2.1.3",
        "@radix-ui/react-use-controllable-state": "1.2.2"
      },
      "peerDependencies": {
        "@types/react": "*",
        "@types/react-dom": "*",
        "react": "^16.8 || ^17.0 || ^18.0 || ^19.0 || ^19.0.0-rc",
        "react-dom": "^16.8 || ^17.0 || ^18.0 || ^19.0 || ^19.0.0-rc"
      },
      "peerDependenciesMeta": {
        "@types/react": {
          "optional": true
        },
        "@types/react-dom": {
          "optional": true
        }
      }
    },
    "node_modules/@radix-ui/react-alert-dialog": {
      "version": "1.1.15",
      "resolved": "https://registry.npmjs.org/@radix-ui/react-alert-dialog/-/react-alert-dialog-1.1.15.tgz",
      "integrity": "sha512-oTVLkEw5GpdRe29BqJ0LSDFWI3qu0vR1M0mUkOQWDIUnY/QIkLpgDMWuKxP94c2NAC2LGcgVhG1ImF3jkZ5wXw==",
      "license": "MIT",
      "dependencies": {
        "@radix-ui/primitive": "1.1.3",
        "@radix-ui/react-compose-refs": "1.1.2",
        "@radix-ui/react-context": "1.1.2",
        "@radix-ui/react-dialog": "1.1.15",
        "@radix-ui/react-primitive": "2.1.3",
        "@radix-ui/react-slot": "1.2.3"
      },
      "peerDependencies": {
        "@types/react": "*",
        "@types/react-dom": "*",
        "react": "^16.8 || ^17.0 || ^18.0 || ^19.0 || ^19.0.0-rc",
        "react-dom": "^16.8 || ^17.0 || ^18.0 || ^19.0 || ^19.0.0-rc"
      },
      "peerDependenciesMeta": {
        "@types/react": {
          "optional": true
        },
        "@types/react-dom": {
          "optional": true
        }
      }
    },
    "node_modules/@radix-ui/react-alert-dialog/node_modules/@radix-ui/react-slot": {
      "version": "1.2.3",
      "resolved": "https://registry.npmjs.org/@radix-ui/react-slot/-/react-slot-1.2.3.tgz",
      "integrity": "sha512-aeNmHnBxbi2St0au6VBVC7JXFlhLlOnvIIlePNniyUNAClzmtAUEY8/pBiK3iHjufOlwA+c20/8jngo7xcrg8A==",
      "license": "MIT",
      "dependencies": {
        "@radix-ui/react-compose-refs": "1.1.2"
      },
      "peerDependencies": {
        "@types/react": "*",
        "react": "^16.8 || ^17.0 || ^18.0 || ^19.0 || ^19.0.0-rc"
      },
      "peerDependenciesMeta": {
        "@types/react": {
          "optional": true
        }
      }
    },
    "node_modules/@radix-ui/react-arrow": {
      "version": "1.1.7",
      "resolved": "https://registry.npmjs.org/@radix-ui/react-arrow/-/react-arrow-1.1.7.tgz",
      "integrity": "sha512-F+M1tLhO+mlQaOWspE8Wstg+z6PwxwRd8oQ8IXceWz92kfAmalTRf0EjrouQeo7QssEPfCn05B4Ihs1K9WQ/7w==",
      "license": "MIT",
      "dependencies": {
        "@radix-ui/react-primitive": "2.1.3"
      },
      "peerDependencies": {
        "@types/react": "*",
        "@types/react-dom": "*",
        "react": "^16.8 || ^17.0 || ^18.0 || ^19.0 || ^19.0.0-rc",
        "react-dom": "^16.8 || ^17.0 || ^18.0 || ^19.0 || ^19.0.0-rc"
      },
      "peerDependenciesMeta": {
        "@types/react": {
          "optional": true
        },
        "@types/react-dom": {
          "optional": true
        }
      }
    },
    "node_modules/@radix-ui/react-aspect-ratio": {
      "version": "1.1.8",
      "resolved": "https://registry.npmjs.org/@radix-ui/react-aspect-ratio/-/react-aspect-ratio-1.1.8.tgz",
      "integrity": "sha512-5nZrJTF7gH+e0nZS7/QxFz6tJV4VimhQb1avEgtsJxvvIp5JilL+c58HICsKzPxghdwaDt48hEfPM1au4zGy+w==",
      "license": "MIT",
      "dependencies": {
        "@radix-ui/react-primitive": "2.1.4"
      },
      "peerDependencies": {
        "@types/react": "*",
        "@types/react-dom": "*",
        "react": "^16.8 || ^17.0 || ^18.0 || ^19.0 || ^19.0.0-rc",
        "react-dom": "^16.8 || ^17.0 || ^18.0 || ^19.0 || ^19.0.0-rc"
      },
      "peerDependenciesMeta": {
        "@types/react": {
          "optional": true
        },
        "@types/react-dom": {
          "optional": true
        }
      }
    },
    "node_modules/@radix-ui/react-aspect-ratio/node_modules/@radix-ui/react-primitive": {
      "version": "2.1.4",
      "resolved": "https://registry.npmjs.org/@radix-ui/react-primitive/-/react-primitive-2.1.4.tgz",
      "integrity": "sha512-9hQc4+GNVtJAIEPEqlYqW5RiYdrr8ea5XQ0ZOnD6fgru+83kqT15mq2OCcbe8KnjRZl5vF3ks69AKz3kh1jrhg==",
      "license": "MIT",
      "dependencies": {
        "@radix-ui/react-slot": "1.2.4"
      },
      "peerDependencies": {
        "@types/react": "*",
        "@types/react-dom": "*",
        "react": "^16.8 || ^17.0 || ^18.0 || ^19.0 || ^19.0.0-rc",
        "react-dom": "^16.8 || ^17.0 || ^18.0 || ^19.0 || ^19.0.0-rc"
      },
      "peerDependenciesMeta": {
        "@types/react": {
          "optional": true
        },
        "@types/react-dom": {
          "optional": true
        }
      }
    },
    "node_modules/@radix-ui/react-avatar": {
      "version": "1.1.11",
      "resolved": "https://registry.npmjs.org/@radix-ui/react-avatar/-/react-avatar-1.1.11.tgz",
      "integrity": "sha512-0Qk603AHGV28BOBO34p7IgD5m+V5Sg/YovfayABkoDDBM5d3NCx0Mp4gGrjzLGes1jV5eNOE1r3itqOR33VC6Q==",
      "license": "MIT",
      "dependencies": {
        "@radix-ui/react-context": "1.1.3",
        "@radix-ui/react-primitive": "2.1.4",
        "@radix-ui/react-use-callback-ref": "1.1.1",
        "@radix-ui/react-use-is-hydrated": "0.1.0",
        "@radix-ui/react-use-layout-effect": "1.1.1"
      },
      "peerDependencies": {
        "@types/react": "*",
        "@types/react-dom": "*",
        "react": "^16.8 || ^17.0 || ^18.0 || ^19.0 || ^19.0.0-rc",
        "react-dom": "^16.8 || ^17.0 || ^18.0 || ^19.0 || ^19.0.0-rc"
      },
      "peerDependenciesMeta": {
        "@types/react": {
          "optional": true
        },
        "@types/react-dom": {
          "optional": true
        }
      }
    },
    "node_modules/@radix-ui/react-avatar/node_modules/@radix-ui/react-context": {
      "version": "1.1.3",
      "resolved": "https://registry.npmjs.org/@radix-ui/react-context/-/react-context-1.1.3.tgz",
      "integrity": "sha512-ieIFACdMpYfMEjF0rEf5KLvfVyIkOz6PDGyNnP+u+4xQ6jny3VCgA4OgXOwNx2aUkxn8zx9fiVcM8CfFYv9Lxw==",
      "license": "MIT",
      "peerDependencies": {
        "@types/react": "*",
        "react": "^16.8 || ^17.0 || ^18.0 || ^19.0 || ^19.0.0-rc"
      },
      "peerDependenciesMeta": {
        "@types/react": {
          "optional": true
        }
      }
    },
    "node_modules/@radix-ui/react-avatar/node_modules/@radix-ui/react-primitive": {
      "version": "2.1.4",
      "resolved": "https://registry.npmjs.org/@radix-ui/react-primitive/-/react-primitive-2.1.4.tgz",
      "integrity": "sha512-9hQc4+GNVtJAIEPEqlYqW5RiYdrr8ea5XQ0ZOnD6fgru+83kqT15mq2OCcbe8KnjRZl5vF3ks69AKz3kh1jrhg==",
      "license": "MIT",
      "dependencies": {
        "@radix-ui/react-slot": "1.2.4"
      },
      "peerDependencies": {
        "@types/react": "*",
        "@types/react-dom": "*",
        "react": "^16.8 || ^17.0 || ^18.0 || ^19.0 || ^19.0.0-rc",
        "react-dom": "^16.8 || ^17.0 || ^18.0 || ^19.0 || ^19.0.0-rc"
      },
      "peerDependenciesMeta": {
        "@types/react": {
          "optional": true
        },
        "@types/react-dom": {
          "optional": true
        }
      }
    },
    "node_modules/@radix-ui/react-checkbox": {
      "version": "1.3.3",
      "resolved": "https://registry.npmjs.org/@radix-ui/react-checkbox/-/react-checkbox-1.3.3.tgz",
      "integrity": "sha512-wBbpv+NQftHDdG86Qc0pIyXk5IR3tM8Vd0nWLKDcX8nNn4nXFOFwsKuqw2okA/1D/mpaAkmuyndrPJTYDNZtFw==",
      "license": "MIT",
      "dependencies": {
        "@radix-ui/primitive": "1.1.3",
        "@radix-ui/react-compose-refs": "1.1.2",
        "@radix-ui/react-context": "1.1.2",
        "@radix-ui/react-presence": "1.1.5",
        "@radix-ui/react-primitive": "2.1.3",
        "@radix-ui/react-use-controllable-state": "1.2.2",
        "@radix-ui/react-use-previous": "1.1.1",
        "@radix-ui/react-use-size": "1.1.1"
      },
      "peerDependencies": {
        "@types/react": "*",
        "@types/react-dom": "*",
        "react": "^16.8 || ^17.0 || ^18.0 || ^19.0 || ^19.0.0-rc",
        "react-dom": "^16.8 || ^17.0 || ^18.0 || ^19.0 || ^19.0.0-rc"
      },
      "peerDependenciesMeta": {
        "@types/react": {
          "optional": true
        },
        "@types/react-dom": {
          "optional": true
        }
      }
    },
    "node_modules/@radix-ui/react-collapsible": {
      "version": "1.1.12",
      "resolved": "https://registry.npmjs.org/@radix-ui/react-collapsible/-/react-collapsible-1.1.12.tgz",
      "integrity": "sha512-Uu+mSh4agx2ib1uIGPP4/CKNULyajb3p92LsVXmH2EHVMTfZWpll88XJ0j4W0z3f8NK1eYl1+Mf/szHPmcHzyA==",
      "license": "MIT",
      "dependencies": {
        "@radix-ui/primitive": "1.1.3",
        "@radix-ui/react-compose-refs": "1.1.2",
        "@radix-ui/react-context": "1.1.2",
        "@radix-ui/react-id": "1.1.1",
        "@radix-ui/react-presence": "1.1.5",
        "@radix-ui/react-primitive": "2.1.3",
        "@radix-ui/react-use-controllable-state": "1.2.2",
        "@radix-ui/react-use-layout-effect": "1.1.1"
      },
      "peerDependencies": {
        "@types/react": "*",
        "@types/react-dom": "*",
        "react": "^16.8 || ^17.0 || ^18.0 || ^19.0 || ^19.0.0-rc",
        "react-dom": "^16.8 || ^17.0 || ^18.0 || ^19.0 || ^19.0.0-rc"
      },
      "peerDependenciesMeta": {
        "@types/react": {
          "optional": true
        },
        "@types/react-dom": {
          "optional": true
        }
      }
    },
    "node_modules/@radix-ui/react-collection": {
      "version": "1.1.7",
      "resolved": "https://registry.npmjs.org/@radix-ui/react-collection/-/react-collection-1.1.7.tgz",
      "integrity": "sha512-Fh9rGN0MoI4ZFUNyfFVNU4y9LUz93u9/0K+yLgA2bwRojxM8JU1DyvvMBabnZPBgMWREAJvU2jjVzq+LrFUglw==",
      "license": "MIT",
      "dependencies": {
        "@radix-ui/react-compose-refs": "1.1.2",
        "@radix-ui/react-context": "1.1.2",
        "@radix-ui/react-primitive": "2.1.3",
        "@radix-ui/react-slot": "1.2.3"
      },
      "peerDependencies": {
        "@types/react": "*",
        "@types/react-dom": "*",
        "react": "^16.8 || ^17.0 || ^18.0 || ^19.0 || ^19.0.0-rc",
        "react-dom": "^16.8 || ^17.0 || ^18.0 || ^19.0 || ^19.0.0-rc"
      },
      "peerDependenciesMeta": {
        "@types/react": {
          "optional": true
        },
        "@types/react-dom": {
          "optional": true
        }
      }
    },
    "node_modules/@radix-ui/react-collection/node_modules/@radix-ui/react-slot": {
      "version": "1.2.3",
      "resolved": "https://registry.npmjs.org/@radix-ui/react-slot/-/react-slot-1.2.3.tgz",
      "integrity": "sha512-aeNmHnBxbi2St0au6VBVC7JXFlhLlOnvIIlePNniyUNAClzmtAUEY8/pBiK3iHjufOlwA+c20/8jngo7xcrg8A==",
      "license": "MIT",
      "dependencies": {
        "@radix-ui/react-compose-refs": "1.1.2"
      },
      "peerDependencies": {
        "@types/react": "*",
        "react": "^16.8 || ^17.0 || ^18.0 || ^19.0 || ^19.0.0-rc"
      },
      "peerDependenciesMeta": {
        "@types/react": {
          "optional": true
        }
      }
    },
    "node_modules/@radix-ui/react-compose-refs": {
      "version": "1.1.2",
      "resolved": "https://registry.npmjs.org/@radix-ui/react-compose-refs/-/react-compose-refs-1.1.2.tgz",
      "integrity": "sha512-z4eqJvfiNnFMHIIvXP3CY57y2WJs5g2v3X0zm9mEJkrkNv4rDxu+sg9Jh8EkXyeqBkB7SOcboo9dMVqhyrACIg==",
      "license": "MIT",
      "peerDependencies": {
        "@types/react": "*",
        "react": "^16.8 || ^17.0 || ^18.0 || ^19.0 || ^19.0.0-rc"
      },
      "peerDependenciesMeta": {
        "@types/react": {
          "optional": true
        }
      }
    },
    "node_modules/@radix-ui/react-context": {
      "version": "1.1.2",
      "resolved": "https://registry.npmjs.org/@radix-ui/react-context/-/react-context-1.1.2.tgz",
      "integrity": "sha512-jCi/QKUM2r1Ju5a3J64TH2A5SpKAgh0LpknyqdQ4m6DCV0xJ2HG1xARRwNGPQfi1SLdLWZ1OJz6F4OMBBNiGJA==",
      "license": "MIT",
      "peerDependencies": {
        "@types/react": "*",
        "react": "^16.8 || ^17.0 || ^18.0 || ^19.0 || ^19.0.0-rc"
      },
      "peerDependenciesMeta": {
        "@types/react": {
          "optional": true
        }
      }
    },
    "node_modules/@radix-ui/react-context-menu": {
      "version": "2.2.16",
      "resolved": "https://registry.npmjs.org/@radix-ui/react-context-menu/-/react-context-menu-2.2.16.tgz",
      "integrity": "sha512-O8morBEW+HsVG28gYDZPTrT9UUovQUlJue5YO836tiTJhuIWBm/zQHc7j388sHWtdH/xUZurK9olD2+pcqx5ww==",
      "license": "MIT",
      "dependencies": {
        "@radix-ui/primitive": "1.1.3",
        "@radix-ui/react-context": "1.1.2",
        "@radix-ui/react-menu": "2.1.16",
        "@radix-ui/react-primitive": "2.1.3",
        "@radix-ui/react-use-callback-ref": "1.1.1",
        "@radix-ui/react-use-controllable-state": "1.2.2"
      },
      "peerDependencies": {
        "@types/react": "*",
        "@types/react-dom": "*",
        "react": "^16.8 || ^17.0 || ^18.0 || ^19.0 || ^19.0.0-rc",
        "react-dom": "^16.8 || ^17.0 || ^18.0 || ^19.0 || ^19.0.0-rc"
      },
      "peerDependenciesMeta": {
        "@types/react": {
          "optional": true
        },
        "@types/react-dom": {
          "optional": true
        }
      }
    },
    "node_modules/@radix-ui/react-dialog": {
      "version": "1.1.15",
      "resolved": "https://registry.npmjs.org/@radix-ui/react-dialog/-/react-dialog-1.1.15.tgz",
      "integrity": "sha512-TCglVRtzlffRNxRMEyR36DGBLJpeusFcgMVD9PZEzAKnUs1lKCgX5u9BmC2Yg+LL9MgZDugFFs1Vl+Jp4t/PGw==",
      "license": "MIT",
      "dependencies": {
        "@radix-ui/primitive": "1.1.3",
        "@radix-ui/react-compose-refs": "1.1.2",
        "@radix-ui/react-context": "1.1.2",
        "@radix-ui/react-dismissable-layer": "1.1.11",
        "@radix-ui/react-focus-guards": "1.1.3",
        "@radix-ui/react-focus-scope": "1.1.7",
        "@radix-ui/react-id": "1.1.1",
        "@radix-ui/react-portal": "1.1.9",
        "@radix-ui/react-presence": "1.1.5",
        "@radix-ui/react-primitive": "2.1.3",
        "@radix-ui/react-slot": "1.2.3",
        "@radix-ui/react-use-controllable-state": "1.2.2",
        "aria-hidden": "^1.2.4",
        "react-remove-scroll": "^2.6.3"
      },
      "peerDependencies": {
        "@types/react": "*",
        "@types/react-dom": "*",
        "react": "^16.8 || ^17.0 || ^18.0 || ^19.0 || ^19.0.0-rc",
        "react-dom": "^16.8 || ^17.0 || ^18.0 || ^19.0 || ^19.0.0-rc"
      },
      "peerDependenciesMeta": {
        "@types/react": {
          "optional": true
        },
        "@types/react-dom": {
          "optional": true
        }
      }
    },
    "node_modules/@radix-ui/react-dialog/node_modules/@radix-ui/react-slot": {
      "version": "1.2.3",
      "resolved": "https://registry.npmjs.org/@radix-ui/react-slot/-/react-slot-1.2.3.tgz",
      "integrity": "sha512-aeNmHnBxbi2St0au6VBVC7JXFlhLlOnvIIlePNniyUNAClzmtAUEY8/pBiK3iHjufOlwA+c20/8jngo7xcrg8A==",
      "license": "MIT",
      "dependencies": {
        "@radix-ui/react-compose-refs": "1.1.2"
      },
      "peerDependencies": {
        "@types/react": "*",
        "react": "^16.8 || ^17.0 || ^18.0 || ^19.0 || ^19.0.0-rc"
      },
      "peerDependenciesMeta": {
        "@types/react": {
          "optional": true
        }
      }
    },
    "node_modules/@radix-ui/react-direction": {
      "version": "1.1.1",
      "resolved": "https://registry.npmjs.org/@radix-ui/react-direction/-/react-direction-1.1.1.tgz",
      "integrity": "sha512-1UEWRX6jnOA2y4H5WczZ44gOOjTEmlqv1uNW4GAJEO5+bauCBhv8snY65Iw5/VOS/ghKN9gr2KjnLKxrsvoMVw==",
      "license": "MIT",
      "peerDependencies": {
        "@types/react": "*",
        "react": "^16.8 || ^17.0 || ^18.0 || ^19.0 || ^19.0.0-rc"
      },
      "peerDependenciesMeta": {
        "@types/react": {
          "optional": true
        }
      }
    },
    "node_modules/@radix-ui/react-dismissable-layer": {
      "version": "1.1.11",
      "resolved": "https://registry.npmjs.org/@radix-ui/react-dismissable-layer/-/react-dismissable-layer-1.1.11.tgz",
      "integrity": "sha512-Nqcp+t5cTB8BinFkZgXiMJniQH0PsUt2k51FUhbdfeKvc4ACcG2uQniY/8+h1Yv6Kza4Q7lD7PQV0z0oicE0Mg==",
      "license": "MIT",
      "dependencies": {
        "@radix-ui/primitive": "1.1.3",
        "@radix-ui/react-compose-refs": "1.1.2",
        "@radix-ui/react-primitive": "2.1.3",
        "@radix-ui/react-use-callback-ref": "1.1.1",
        "@radix-ui/react-use-escape-keydown": "1.1.1"
      },
      "peerDependencies": {
        "@types/react": "*",
        "@types/react-dom": "*",
        "react": "^16.8 || ^17.0 || ^18.0 || ^19.0 || ^19.0.0-rc",
        "react-dom": "^16.8 || ^17.0 || ^18.0 || ^19.0 || ^19.0.0-rc"
      },
      "peerDependenciesMeta": {
        "@types/react": {
          "optional": true
        },
        "@types/react-dom": {
          "optional": true
        }
      }
    },
    "node_modules/@radix-ui/react-dropdown-menu": {
      "version": "2.1.16",
      "resolved": "https://registry.npmjs.org/@radix-ui/react-dropdown-menu/-/react-dropdown-menu-2.1.16.tgz",
      "integrity": "sha512-1PLGQEynI/3OX/ftV54COn+3Sud/Mn8vALg2rWnBLnRaGtJDduNW/22XjlGgPdpcIbiQxjKtb7BkcjP00nqfJw==",
      "license": "MIT",
      "dependencies": {
        "@radix-ui/primitive": "1.1.3",
        "@radix-ui/react-compose-refs": "1.1.2",
        "@radix-ui/react-context": "1.1.2",
        "@radix-ui/react-id": "1.1.1",
        "@radix-ui/react-menu": "2.1.16",
        "@radix-ui/react-primitive": "2.1.3",
        "@radix-ui/react-use-controllable-state": "1.2.2"
      },
      "peerDependencies": {
        "@types/react": "*",
        "@types/react-dom": "*",
        "react": "^16.8 || ^17.0 || ^18.0 || ^19.0 || ^19.0.0-rc",
        "react-dom": "^16.8 || ^17.0 || ^18.0 || ^19.0 || ^19.0.0-rc"
      },
      "peerDependenciesMeta": {
        "@types/react": {
          "optional": true
        },
        "@types/react-dom": {
          "optional": true
        }
      }
    },
    "node_modules/@radix-ui/react-focus-guards": {
      "version": "1.1.3",
      "resolved": "https://registry.npmjs.org/@radix-ui/react-focus-guards/-/react-focus-guards-1.1.3.tgz",
      "integrity": "sha512-0rFg/Rj2Q62NCm62jZw0QX7a3sz6QCQU0LpZdNrJX8byRGaGVTqbrW9jAoIAHyMQqsNpeZ81YgSizOt5WXq0Pw==",
      "license": "MIT",
      "peerDependencies": {
        "@types/react": "*",
        "react": "^16.8 || ^17.0 || ^18.0 || ^19.0 || ^19.0.0-rc"
      },
      "peerDependenciesMeta": {
        "@types/react": {
          "optional": true
        }
      }
    },
    "node_modules/@radix-ui/react-focus-scope": {
      "version": "1.1.7",
      "resolved": "https://registry.npmjs.org/@radix-ui/react-focus-scope/-/react-focus-scope-1.1.7.tgz",
      "integrity": "sha512-t2ODlkXBQyn7jkl6TNaw/MtVEVvIGelJDCG41Okq/KwUsJBwQ4XVZsHAVUkK4mBv3ewiAS3PGuUWuY2BoK4ZUw==",
      "license": "MIT",
      "dependencies": {
        "@radix-ui/react-compose-refs": "1.1.2",
        "@radix-ui/react-primitive": "2.1.3",
        "@radix-ui/react-use-callback-ref": "1.1.1"
      },
      "peerDependencies": {
        "@types/react": "*",
        "@types/react-dom": "*",
        "react": "^16.8 || ^17.0 || ^18.0 || ^19.0 || ^19.0.0-rc",
        "react-dom": "^16.8 || ^17.0 || ^18.0 || ^19.0 || ^19.0.0-rc"
      },
      "peerDependenciesMeta": {
        "@types/react": {
          "optional": true
        },
        "@types/react-dom": {
          "optional": true
        }
      }
    },
    "node_modules/@radix-ui/react-hover-card": {
      "version": "1.1.15",
      "resolved": "https://registry.npmjs.org/@radix-ui/react-hover-card/-/react-hover-card-1.1.15.tgz",
      "integrity": "sha512-qgTkjNT1CfKMoP0rcasmlH2r1DAiYicWsDsufxl940sT2wHNEWWv6FMWIQXWhVdmC1d/HYfbhQx60KYyAtKxjg==",
      "license": "MIT",
      "dependencies": {
        "@radix-ui/primitive": "1.1.3",
        "@radix-ui/react-compose-refs": "1.1.2",
        "@radix-ui/react-context": "1.1.2",
        "@radix-ui/react-dismissable-layer": "1.1.11",
        "@radix-ui/react-popper": "1.2.8",
        "@radix-ui/react-portal": "1.1.9",
        "@radix-ui/react-presence": "1.1.5",
        "@radix-ui/react-primitive": "2.1.3",
        "@radix-ui/react-use-controllable-state": "1.2.2"
      },
      "peerDependencies": {
        "@types/react": "*",
        "@types/react-dom": "*",
        "react": "^16.8 || ^17.0 || ^18.0 || ^19.0 || ^19.0.0-rc",
        "react-dom": "^16.8 || ^17.0 || ^18.0 || ^19.0 || ^19.0.0-rc"
      },
      "peerDependenciesMeta": {
        "@types/react": {
          "optional": true
        },
        "@types/react-dom": {
          "optional": true
        }
      }
    },
    "node_modules/@radix-ui/react-id": {
      "version": "1.1.1",
      "resolved": "https://registry.npmjs.org/@radix-ui/react-id/-/react-id-1.1.1.tgz",
      "integrity": "sha512-kGkGegYIdQsOb4XjsfM97rXsiHaBwco+hFI66oO4s9LU+PLAC5oJ7khdOVFxkhsmlbpUqDAvXw11CluXP+jkHg==",
      "license": "MIT",
      "dependencies": {
        "@radix-ui/react-use-layout-effect": "1.1.1"
      },
      "peerDependencies": {
        "@types/react": "*",
        "react": "^16.8 || ^17.0 || ^18.0 || ^19.0 || ^19.0.0-rc"
      },
      "peerDependenciesMeta": {
        "@types/react": {
          "optional": true
        }
      }
    },
    "node_modules/@radix-ui/react-label": {
      "version": "2.1.8",
      "resolved": "https://registry.npmjs.org/@radix-ui/react-label/-/react-label-2.1.8.tgz",
      "integrity": "sha512-FmXs37I6hSBVDlO4y764TNz1rLgKwjJMQ0EGte6F3Cb3f4bIuHB/iLa/8I9VKkmOy+gNHq8rql3j686ACVV21A==",
      "license": "MIT",
      "dependencies": {
        "@radix-ui/react-primitive": "2.1.4"
      },
      "peerDependencies": {
        "@types/react": "*",
        "@types/react-dom": "*",
        "react": "^16.8 || ^17.0 || ^18.0 || ^19.0 || ^19.0.0-rc",
        "react-dom": "^16.8 || ^17.0 || ^18.0 || ^19.0 || ^19.0.0-rc"
      },
      "peerDependenciesMeta": {
        "@types/react": {
          "optional": true
        },
        "@types/react-dom": {
          "optional": true
        }
      }
    },
    "node_modules/@radix-ui/react-label/node_modules/@radix-ui/react-primitive": {
      "version": "2.1.4",
      "resolved": "https://registry.npmjs.org/@radix-ui/react-primitive/-/react-primitive-2.1.4.tgz",
      "integrity": "sha512-9hQc4+GNVtJAIEPEqlYqW5RiYdrr8ea5XQ0ZOnD6fgru+83kqT15mq2OCcbe8KnjRZl5vF3ks69AKz3kh1jrhg==",
      "license": "MIT",
      "dependencies": {
        "@radix-ui/react-slot": "1.2.4"
      },
      "peerDependencies": {
        "@types/react": "*",
        "@types/react-dom": "*",
        "react": "^16.8 || ^17.0 || ^18.0 || ^19.0 || ^19.0.0-rc",
        "react-dom": "^16.8 || ^17.0 || ^18.0 || ^19.0 || ^19.0.0-rc"
      },
      "peerDependenciesMeta": {
        "@types/react": {
          "optional": true
        },
        "@types/react-dom": {
          "optional": true
        }
      }
    },
    "node_modules/@radix-ui/react-menu": {
      "version": "2.1.16",
      "resolved": "https://registry.npmjs.org/@radix-ui/react-menu/-/react-menu-2.1.16.tgz",
      "integrity": "sha512-72F2T+PLlphrqLcAotYPp0uJMr5SjP5SL01wfEspJbru5Zs5vQaSHb4VB3ZMJPimgHHCHG7gMOeOB9H3Hdmtxg==",
      "license": "MIT",
      "dependencies": {
        "@radix-ui/primitive": "1.1.3",
        "@radix-ui/react-collection": "1.1.7",
        "@radix-ui/react-compose-refs": "1.1.2",
        "@radix-ui/react-context": "1.1.2",
        "@radix-ui/react-direction": "1.1.1",
        "@radix-ui/react-dismissable-layer": "1.1.11",
        "@radix-ui/react-focus-guards": "1.1.3",
        "@radix-ui/react-focus-scope": "1.1.7",
        "@radix-ui/react-id": "1.1.1",
        "@radix-ui/react-popper": "1.2.8",
        "@radix-ui/react-portal": "1.1.9",
        "@radix-ui/react-presence": "1.1.5",
        "@radix-ui/react-primitive": "2.1.3",
        "@radix-ui/react-roving-focus": "1.1.11",
        "@radix-ui/react-slot": "1.2.3",
        "@radix-ui/react-use-callback-ref": "1.1.1",
        "aria-hidden": "^1.2.4",
        "react-remove-scroll": "^2.6.3"
      },
      "peerDependencies": {
        "@types/react": "*",
        "@types/react-dom": "*",
        "react": "^16.8 || ^17.0 || ^18.0 || ^19.0 || ^19.0.0-rc",
        "react-dom": "^16.8 || ^17.0 || ^18.0 || ^19.0 || ^19.0.0-rc"
      },
      "peerDependenciesMeta": {
        "@types/react": {
          "optional": true
        },
        "@types/react-dom": {
          "optional": true
        }
      }
    },
    "node_modules/@radix-ui/react-menu/node_modules/@radix-ui/react-slot": {
      "version": "1.2.3",
      "resolved": "https://registry.npmjs.org/@radix-ui/react-slot/-/react-slot-1.2.3.tgz",
      "integrity": "sha512-aeNmHnBxbi2St0au6VBVC7JXFlhLlOnvIIlePNniyUNAClzmtAUEY8/pBiK3iHjufOlwA+c20/8jngo7xcrg8A==",
      "license": "MIT",
      "dependencies": {
        "@radix-ui/react-compose-refs": "1.1.2"
      },
      "peerDependencies": {
        "@types/react": "*",
        "react": "^16.8 || ^17.0 || ^18.0 || ^19.0 || ^19.0.0-rc"
      },
      "peerDependenciesMeta": {
        "@types/react": {
          "optional": true
        }
      }
    },
    "node_modules/@radix-ui/react-menubar": {
      "version": "1.1.16",
      "resolved": "https://registry.npmjs.org/@radix-ui/react-menubar/-/react-menubar-1.1.16.tgz",
      "integrity": "sha512-EB1FktTz5xRRi2Er974AUQZWg2yVBb1yjip38/lgwtCVRd3a+maUoGHN/xs9Yv8SY8QwbSEb+YrxGadVWbEutA==",
      "license": "MIT",
      "dependencies": {
        "@radix-ui/primitive": "1.1.3",
        "@radix-ui/react-collection": "1.1.7",
        "@radix-ui/react-compose-refs": "1.1.2",
        "@radix-ui/react-context": "1.1.2",
        "@radix-ui/react-direction": "1.1.1",
        "@radix-ui/react-id": "1.1.1",
        "@radix-ui/react-menu": "2.1.16",
        "@radix-ui/react-primitive": "2.1.3",
        "@radix-ui/react-roving-focus": "1.1.11",
        "@radix-ui/react-use-controllable-state": "1.2.2"
      },
      "peerDependencies": {
        "@types/react": "*",
        "@types/react-dom": "*",
        "react": "^16.8 || ^17.0 || ^18.0 || ^19.0 || ^19.0.0-rc",
        "react-dom": "^16.8 || ^17.0 || ^18.0 || ^19.0 || ^19.0.0-rc"
      },
      "peerDependenciesMeta": {
        "@types/react": {
          "optional": true
        },
        "@types/react-dom": {
          "optional": true
        }
      }
    },
    "node_modules/@radix-ui/react-navigation-menu": {
      "version": "1.2.14",
      "resolved": "https://registry.npmjs.org/@radix-ui/react-navigation-menu/-/react-navigation-menu-1.2.14.tgz",
      "integrity": "sha512-YB9mTFQvCOAQMHU+C/jVl96WmuWeltyUEpRJJky51huhds5W2FQr1J8D/16sQlf0ozxkPK8uF3niQMdUwZPv5w==",
      "license": "MIT",
      "dependencies": {
        "@radix-ui/primitive": "1.1.3",
        "@radix-ui/react-collection": "1.1.7",
        "@radix-ui/react-compose-refs": "1.1.2",
        "@radix-ui/react-context": "1.1.2",
        "@radix-ui/react-direction": "1.1.1",
        "@radix-ui/react-dismissable-layer": "1.1.11",
        "@radix-ui/react-id": "1.1.1",
        "@radix-ui/react-presence": "1.1.5",
        "@radix-ui/react-primitive": "2.1.3",
        "@radix-ui/react-use-callback-ref": "1.1.1",
        "@radix-ui/react-use-controllable-state": "1.2.2",
        "@radix-ui/react-use-layout-effect": "1.1.1",
        "@radix-ui/react-use-previous": "1.1.1",
        "@radix-ui/react-visually-hidden": "1.2.3"
      },
      "peerDependencies": {
        "@types/react": "*",
        "@types/react-dom": "*",
        "react": "^16.8 || ^17.0 || ^18.0 || ^19.0 || ^19.0.0-rc",
        "react-dom": "^16.8 || ^17.0 || ^18.0 || ^19.0 || ^19.0.0-rc"
      },
      "peerDependenciesMeta": {
        "@types/react": {
          "optional": true
        },
        "@types/react-dom": {
          "optional": true
        }
      }
    },
    "node_modules/@radix-ui/react-popover": {
      "version": "1.1.15",
      "resolved": "https://registry.npmjs.org/@radix-ui/react-popover/-/react-popover-1.1.15.tgz",
      "integrity": "sha512-kr0X2+6Yy/vJzLYJUPCZEc8SfQcf+1COFoAqauJm74umQhta9M7lNJHP7QQS3vkvcGLQUbWpMzwrXYwrYztHKA==",
      "license": "MIT",
      "dependencies": {
        "@radix-ui/primitive": "1.1.3",
        "@radix-ui/react-compose-refs": "1.1.2",
        "@radix-ui/react-context": "1.1.2",
        "@radix-ui/react-dismissable-layer": "1.1.11",
        "@radix-ui/react-focus-guards": "1.1.3",
        "@radix-ui/react-focus-scope": "1.1.7",
        "@radix-ui/react-id": "1.1.1",
        "@radix-ui/react-popper": "1.2.8",
        "@radix-ui/react-portal": "1.1.9",
        "@radix-ui/react-presence": "1.1.5",
        "@radix-ui/react-primitive": "2.1.3",
        "@radix-ui/react-slot": "1.2.3",
        "@radix-ui/react-use-controllable-state": "1.2.2",
        "aria-hidden": "^1.2.4",
        "react-remove-scroll": "^2.6.3"
      },
      "peerDependencies": {
        "@types/react": "*",
        "@types/react-dom": "*",
        "react": "^16.8 || ^17.0 || ^18.0 || ^19.0 || ^19.0.0-rc",
        "react-dom": "^16.8 || ^17.0 || ^18.0 || ^19.0 || ^19.0.0-rc"
      },
      "peerDependenciesMeta": {
        "@types/react": {
          "optional": true
        },
        "@types/react-dom": {
          "optional": true
        }
      }
    },
    "node_modules/@radix-ui/react-popover/node_modules/@radix-ui/react-slot": {
      "version": "1.2.3",
      "resolved": "https://registry.npmjs.org/@radix-ui/react-slot/-/react-slot-1.2.3.tgz",
      "integrity": "sha512-aeNmHnBxbi2St0au6VBVC7JXFlhLlOnvIIlePNniyUNAClzmtAUEY8/pBiK3iHjufOlwA+c20/8jngo7xcrg8A==",
      "license": "MIT",
      "dependencies": {
        "@radix-ui/react-compose-refs": "1.1.2"
      },
      "peerDependencies": {
        "@types/react": "*",
        "react": "^16.8 || ^17.0 || ^18.0 || ^19.0 || ^19.0.0-rc"
      },
      "peerDependenciesMeta": {
        "@types/react": {
          "optional": true
        }
      }
    },
    "node_modules/@radix-ui/react-popper": {
      "version": "1.2.8",
      "resolved": "https://registry.npmjs.org/@radix-ui/react-popper/-/react-popper-1.2.8.tgz",
      "integrity": "sha512-0NJQ4LFFUuWkE7Oxf0htBKS6zLkkjBH+hM1uk7Ng705ReR8m/uelduy1DBo0PyBXPKVnBA6YBlU94MBGXrSBCw==",
      "license": "MIT",
      "dependencies": {
        "@floating-ui/react-dom": "^2.0.0",
        "@radix-ui/react-arrow": "1.1.7",
        "@radix-ui/react-compose-refs": "1.1.2",
        "@radix-ui/react-context": "1.1.2",
        "@radix-ui/react-primitive": "2.1.3",
        "@radix-ui/react-use-callback-ref": "1.1.1",
        "@radix-ui/react-use-layout-effect": "1.1.1",
        "@radix-ui/react-use-rect": "1.1.1",
        "@radix-ui/react-use-size": "1.1.1",
        "@radix-ui/rect": "1.1.1"
      },
      "peerDependencies": {
        "@types/react": "*",
        "@types/react-dom": "*",
        "react": "^16.8 || ^17.0 || ^18.0 || ^19.0 || ^19.0.0-rc",
        "react-dom": "^16.8 || ^17.0 || ^18.0 || ^19.0 || ^19.0.0-rc"
      },
      "peerDependenciesMeta": {
        "@types/react": {
          "optional": true
        },
        "@types/react-dom": {
          "optional": true
        }
      }
    },
    "node_modules/@radix-ui/react-portal": {
      "version": "1.1.9",
      "resolved": "https://registry.npmjs.org/@radix-ui/react-portal/-/react-portal-1.1.9.tgz",
      "integrity": "sha512-bpIxvq03if6UNwXZ+HTK71JLh4APvnXntDc6XOX8UVq4XQOVl7lwok0AvIl+b8zgCw3fSaVTZMpAPPagXbKmHQ==",
      "license": "MIT",
      "dependencies": {
        "@radix-ui/react-primitive": "2.1.3",
        "@radix-ui/react-use-layout-effect": "1.1.1"
      },
      "peerDependencies": {
        "@types/react": "*",
        "@types/react-dom": "*",
        "react": "^16.8 || ^17.0 || ^18.0 || ^19.0 || ^19.0.0-rc",
        "react-dom": "^16.8 || ^17.0 || ^18.0 || ^19.0 || ^19.0.0-rc"
      },
      "peerDependenciesMeta": {
        "@types/react": {
          "optional": true
        },
        "@types/react-dom": {
          "optional": true
        }
      }
    },
    "node_modules/@radix-ui/react-presence": {
      "version": "1.1.5",
      "resolved": "https://registry.npmjs.org/@radix-ui/react-presence/-/react-presence-1.1.5.tgz",
      "integrity": "sha512-/jfEwNDdQVBCNvjkGit4h6pMOzq8bHkopq458dPt2lMjx+eBQUohZNG9A7DtO/O5ukSbxuaNGXMjHicgwy6rQQ==",
      "license": "MIT",
      "dependencies": {
        "@radix-ui/react-compose-refs": "1.1.2",
        "@radix-ui/react-use-layout-effect": "1.1.1"
      },
      "peerDependencies": {
        "@types/react": "*",
        "@types/react-dom": "*",
        "react": "^16.8 || ^17.0 || ^18.0 || ^19.0 || ^19.0.0-rc",
        "react-dom": "^16.8 || ^17.0 || ^18.0 || ^19.0 || ^19.0.0-rc"
      },
      "peerDependenciesMeta": {
        "@types/react": {
          "optional": true
        },
        "@types/react-dom": {
          "optional": true
        }
      }
    },
    "node_modules/@radix-ui/react-primitive": {
      "version": "2.1.3",
      "resolved": "https://registry.npmjs.org/@radix-ui/react-primitive/-/react-primitive-2.1.3.tgz",
      "integrity": "sha512-m9gTwRkhy2lvCPe6QJp4d3G1TYEUHn/FzJUtq9MjH46an1wJU+GdoGC5VLof8RX8Ft/DlpshApkhswDLZzHIcQ==",
      "license": "MIT",
      "dependencies": {
        "@radix-ui/react-slot": "1.2.3"
      },
      "peerDependencies": {
        "@types/react": "*",
        "@types/react-dom": "*",
        "react": "^16.8 || ^17.0 || ^18.0 || ^19.0 || ^19.0.0-rc",
        "react-dom": "^16.8 || ^17.0 || ^18.0 || ^19.0 || ^19.0.0-rc"
      },
      "peerDependenciesMeta": {
        "@types/react": {
          "optional": true
        },
        "@types/react-dom": {
          "optional": true
        }
      }
    },
    "node_modules/@radix-ui/react-primitive/node_modules/@radix-ui/react-slot": {
      "version": "1.2.3",
      "resolved": "https://registry.npmjs.org/@radix-ui/react-slot/-/react-slot-1.2.3.tgz",
      "integrity": "sha512-aeNmHnBxbi2St0au6VBVC7JXFlhLlOnvIIlePNniyUNAClzmtAUEY8/pBiK3iHjufOlwA+c20/8jngo7xcrg8A==",
      "license": "MIT",
      "dependencies": {
        "@radix-ui/react-compose-refs": "1.1.2"
      },
      "peerDependencies": {
        "@types/react": "*",
        "react": "^16.8 || ^17.0 || ^18.0 || ^19.0 || ^19.0.0-rc"
      },
      "peerDependenciesMeta": {
        "@types/react": {
          "optional": true
        }
      }
    },
    "node_modules/@radix-ui/react-progress": {
      "version": "1.1.8",
      "resolved": "https://registry.npmjs.org/@radix-ui/react-progress/-/react-progress-1.1.8.tgz",
      "integrity": "sha512-+gISHcSPUJ7ktBy9RnTqbdKW78bcGke3t6taawyZ71pio1JewwGSJizycs7rLhGTvMJYCQB1DBK4KQsxs7U8dA==",
      "license": "MIT",
      "dependencies": {
        "@radix-ui/react-context": "1.1.3",
        "@radix-ui/react-primitive": "2.1.4"
      },
      "peerDependencies": {
        "@types/react": "*",
        "@types/react-dom": "*",
        "react": "^16.8 || ^17.0 || ^18.0 || ^19.0 || ^19.0.0-rc",
        "react-dom": "^16.8 || ^17.0 || ^18.0 || ^19.0 || ^19.0.0-rc"
      },
      "peerDependenciesMeta": {
        "@types/react": {
          "optional": true
        },
        "@types/react-dom": {
          "optional": true
        }
      }
    },
    "node_modules/@radix-ui/react-progress/node_modules/@radix-ui/react-context": {
      "version": "1.1.3",
      "resolved": "https://registry.npmjs.org/@radix-ui/react-context/-/react-context-1.1.3.tgz",
      "integrity": "sha512-ieIFACdMpYfMEjF0rEf5KLvfVyIkOz6PDGyNnP+u+4xQ6jny3VCgA4OgXOwNx2aUkxn8zx9fiVcM8CfFYv9Lxw==",
      "license": "MIT",
      "peerDependencies": {
        "@types/react": "*",
        "react": "^16.8 || ^17.0 || ^18.0 || ^19.0 || ^19.0.0-rc"
      },
      "peerDependenciesMeta": {
        "@types/react": {
          "optional": true
        }
      }
    },
    "node_modules/@radix-ui/react-progress/node_modules/@radix-ui/react-primitive": {
      "version": "2.1.4",
      "resolved": "https://registry.npmjs.org/@radix-ui/react-primitive/-/react-primitive-2.1.4.tgz",
      "integrity": "sha512-9hQc4+GNVtJAIEPEqlYqW5RiYdrr8ea5XQ0ZOnD6fgru+83kqT15mq2OCcbe8KnjRZl5vF3ks69AKz3kh1jrhg==",
      "license": "MIT",
      "dependencies": {
        "@radix-ui/react-slot": "1.2.4"
      },
      "peerDependencies": {
        "@types/react": "*",
        "@types/react-dom": "*",
        "react": "^16.8 || ^17.0 || ^18.0 || ^19.0 || ^19.0.0-rc",
        "react-dom": "^16.8 || ^17.0 || ^18.0 || ^19.0 || ^19.0.0-rc"
      },
      "peerDependenciesMeta": {
        "@types/react": {
          "optional": true
        },
        "@types/react-dom": {
          "optional": true
        }
      }
    },
    "node_modules/@radix-ui/react-radio-group": {
      "version": "1.3.8",
      "resolved": "https://registry.npmjs.org/@radix-ui/react-radio-group/-/react-radio-group-1.3.8.tgz",
      "integrity": "sha512-VBKYIYImA5zsxACdisNQ3BjCBfmbGH3kQlnFVqlWU4tXwjy7cGX8ta80BcrO+WJXIn5iBylEH3K6ZTlee//lgQ==",
      "license": "MIT",
      "dependencies": {
        "@radix-ui/primitive": "1.1.3",
        "@radix-ui/react-compose-refs": "1.1.2",
        "@radix-ui/react-context": "1.1.2",
        "@radix-ui/react-direction": "1.1.1",
        "@radix-ui/react-presence": "1.1.5",
        "@radix-ui/react-primitive": "2.1.3",
        "@radix-ui/react-roving-focus": "1.1.11",
        "@radix-ui/react-use-controllable-state": "1.2.2",
        "@radix-ui/react-use-previous": "1.1.1",
        "@radix-ui/react-use-size": "1.1.1"
      },
      "peerDependencies": {
        "@types/react": "*",
        "@types/react-dom": "*",
        "react": "^16.8 || ^17.0 || ^18.0 || ^19.0 || ^19.0.0-rc",
        "react-dom": "^16.8 || ^17.0 || ^18.0 || ^19.0 || ^19.0.0-rc"
      },
      "peerDependenciesMeta": {
        "@types/react": {
          "optional": true
        },
        "@types/react-dom": {
          "optional": true
        }
      }
    },
    "node_modules/@radix-ui/react-roving-focus": {
      "version": "1.1.11",
      "resolved": "https://registry.npmjs.org/@radix-ui/react-roving-focus/-/react-roving-focus-1.1.11.tgz",
      "integrity": "sha512-7A6S9jSgm/S+7MdtNDSb+IU859vQqJ/QAtcYQcfFC6W8RS4IxIZDldLR0xqCFZ6DCyrQLjLPsxtTNch5jVA4lA==",
      "license": "MIT",
      "dependencies": {
        "@radix-ui/primitive": "1.1.3",
        "@radix-ui/react-collection": "1.1.7",
        "@radix-ui/react-compose-refs": "1.1.2",
        "@radix-ui/react-context": "1.1.2",
        "@radix-ui/react-direction": "1.1.1",
        "@radix-ui/react-id": "1.1.1",
        "@radix-ui/react-primitive": "2.1.3",
        "@radix-ui/react-use-callback-ref": "1.1.1",
        "@radix-ui/react-use-controllable-state": "1.2.2"
      },
      "peerDependencies": {
        "@types/react": "*",
        "@types/react-dom": "*",
        "react": "^16.8 || ^17.0 || ^18.0 || ^19.0 || ^19.0.0-rc",
        "react-dom": "^16.8 || ^17.0 || ^18.0 || ^19.0 || ^19.0.0-rc"
      },
      "peerDependenciesMeta": {
        "@types/react": {
          "optional": true
        },
        "@types/react-dom": {
          "optional": true
        }
      }
    },
    "node_modules/@radix-ui/react-scroll-area": {
      "version": "1.2.10",
      "resolved": "https://registry.npmjs.org/@radix-ui/react-scroll-area/-/react-scroll-area-1.2.10.tgz",
      "integrity": "sha512-tAXIa1g3sM5CGpVT0uIbUx/U3Gs5N8T52IICuCtObaos1S8fzsrPXG5WObkQN3S6NVl6wKgPhAIiBGbWnvc97A==",
      "license": "MIT",
      "dependencies": {
        "@radix-ui/number": "1.1.1",
        "@radix-ui/primitive": "1.1.3",
        "@radix-ui/react-compose-refs": "1.1.2",
        "@radix-ui/react-context": "1.1.2",
        "@radix-ui/react-direction": "1.1.1",
        "@radix-ui/react-presence": "1.1.5",
        "@radix-ui/react-primitive": "2.1.3",
        "@radix-ui/react-use-callback-ref": "1.1.1",
        "@radix-ui/react-use-layout-effect": "1.1.1"
      },
      "peerDependencies": {
        "@types/react": "*",
        "@types/react-dom": "*",
        "react": "^16.8 || ^17.0 || ^18.0 || ^19.0 || ^19.0.0-rc",
        "react-dom": "^16.8 || ^17.0 || ^18.0 || ^19.0 || ^19.0.0-rc"
      },
      "peerDependenciesMeta": {
        "@types/react": {
          "optional": true
        },
        "@types/react-dom": {
          "optional": true
        }
      }
    },
    "node_modules/@radix-ui/react-select": {
      "version": "2.2.6",
      "resolved": "https://registry.npmjs.org/@radix-ui/react-select/-/react-select-2.2.6.tgz",
      "integrity": "sha512-I30RydO+bnn2PQztvo25tswPH+wFBjehVGtmagkU78yMdwTwVf12wnAOF+AeP8S2N8xD+5UPbGhkUfPyvT+mwQ==",
      "license": "MIT",
      "dependencies": {
        "@radix-ui/number": "1.1.1",
        "@radix-ui/primitive": "1.1.3",
        "@radix-ui/react-collection": "1.1.7",
        "@radix-ui/react-compose-refs": "1.1.2",
        "@radix-ui/react-context": "1.1.2",
        "@radix-ui/react-direction": "1.1.1",
        "@radix-ui/react-dismissable-layer": "1.1.11",
        "@radix-ui/react-focus-guards": "1.1.3",
        "@radix-ui/react-focus-scope": "1.1.7",
        "@radix-ui/react-id": "1.1.1",
        "@radix-ui/react-popper": "1.2.8",
        "@radix-ui/react-portal": "1.1.9",
        "@radix-ui/react-primitive": "2.1.3",
        "@radix-ui/react-slot": "1.2.3",
        "@radix-ui/react-use-callback-ref": "1.1.1",
        "@radix-ui/react-use-controllable-state": "1.2.2",
        "@radix-ui/react-use-layout-effect": "1.1.1",
        "@radix-ui/react-use-previous": "1.1.1",
        "@radix-ui/react-visually-hidden": "1.2.3",
        "aria-hidden": "^1.2.4",
        "react-remove-scroll": "^2.6.3"
      },
      "peerDependencies": {
        "@types/react": "*",
        "@types/react-dom": "*",
        "react": "^16.8 || ^17.0 || ^18.0 || ^19.0 || ^19.0.0-rc",
        "react-dom": "^16.8 || ^17.0 || ^18.0 || ^19.0 || ^19.0.0-rc"
      },
      "peerDependenciesMeta": {
        "@types/react": {
          "optional": true
        },
        "@types/react-dom": {
          "optional": true
        }
      }
    },
    "node_modules/@radix-ui/react-select/node_modules/@radix-ui/react-slot": {
      "version": "1.2.3",
      "resolved": "https://registry.npmjs.org/@radix-ui/react-slot/-/react-slot-1.2.3.tgz",
      "integrity": "sha512-aeNmHnBxbi2St0au6VBVC7JXFlhLlOnvIIlePNniyUNAClzmtAUEY8/pBiK3iHjufOlwA+c20/8jngo7xcrg8A==",
      "license": "MIT",
      "dependencies": {
        "@radix-ui/react-compose-refs": "1.1.2"
      },
      "peerDependencies": {
        "@types/react": "*",
        "react": "^16.8 || ^17.0 || ^18.0 || ^19.0 || ^19.0.0-rc"
      },
      "peerDependenciesMeta": {
        "@types/react": {
          "optional": true
        }
      }
    },
    "node_modules/@radix-ui/react-separator": {
      "version": "1.1.8",
      "resolved": "https://registry.npmjs.org/@radix-ui/react-separator/-/react-separator-1.1.8.tgz",
      "integrity": "sha512-sDvqVY4itsKwwSMEe0jtKgfTh+72Sy3gPmQpjqcQneqQ4PFmr/1I0YA+2/puilhggCe2gJcx5EBAYFkWkdpa5g==",
      "license": "MIT",
      "dependencies": {
        "@radix-ui/react-primitive": "2.1.4"
      },
      "peerDependencies": {
        "@types/react": "*",
        "@types/react-dom": "*",
        "react": "^16.8 || ^17.0 || ^18.0 || ^19.0 || ^19.0.0-rc",
        "react-dom": "^16.8 || ^17.0 || ^18.0 || ^19.0 || ^19.0.0-rc"
      },
      "peerDependenciesMeta": {
        "@types/react": {
          "optional": true
        },
        "@types/react-dom": {
          "optional": true
        }
      }
    },
    "node_modules/@radix-ui/react-separator/node_modules/@radix-ui/react-primitive": {
      "version": "2.1.4",
      "resolved": "https://registry.npmjs.org/@radix-ui/react-primitive/-/react-primitive-2.1.4.tgz",
      "integrity": "sha512-9hQc4+GNVtJAIEPEqlYqW5RiYdrr8ea5XQ0ZOnD6fgru+83kqT15mq2OCcbe8KnjRZl5vF3ks69AKz3kh1jrhg==",
      "license": "MIT",
      "dependencies": {
        "@radix-ui/react-slot": "1.2.4"
      },
      "peerDependencies": {
        "@types/react": "*",
        "@types/react-dom": "*",
        "react": "^16.8 || ^17.0 || ^18.0 || ^19.0 || ^19.0.0-rc",
        "react-dom": "^16.8 || ^17.0 || ^18.0 || ^19.0 || ^19.0.0-rc"
      },
      "peerDependenciesMeta": {
        "@types/react": {
          "optional": true
        },
        "@types/react-dom": {
          "optional": true
        }
      }
    },
    "node_modules/@radix-ui/react-slider": {
      "version": "1.3.6",
      "resolved": "https://registry.npmjs.org/@radix-ui/react-slider/-/react-slider-1.3.6.tgz",
      "integrity": "sha512-JPYb1GuM1bxfjMRlNLE+BcmBC8onfCi60Blk7OBqi2MLTFdS+8401U4uFjnwkOr49BLmXxLC6JHkvAsx5OJvHw==",
      "license": "MIT",
      "dependencies": {
        "@radix-ui/number": "1.1.1",
        "@radix-ui/primitive": "1.1.3",
        "@radix-ui/react-collection": "1.1.7",
        "@radix-ui/react-compose-refs": "1.1.2",
        "@radix-ui/react-context": "1.1.2",
        "@radix-ui/react-direction": "1.1.1",
        "@radix-ui/react-primitive": "2.1.3",
        "@radix-ui/react-use-controllable-state": "1.2.2",
        "@radix-ui/react-use-layout-effect": "1.1.1",
        "@radix-ui/react-use-previous": "1.1.1",
        "@radix-ui/react-use-size": "1.1.1"
      },
      "peerDependencies": {
        "@types/react": "*",
        "@types/react-dom": "*",
        "react": "^16.8 || ^17.0 || ^18.0 || ^19.0 || ^19.0.0-rc",
        "react-dom": "^16.8 || ^17.0 || ^18.0 || ^19.0 || ^19.0.0-rc"
      },
      "peerDependenciesMeta": {
        "@types/react": {
          "optional": true
        },
        "@types/react-dom": {
          "optional": true
        }
      }
    },
    "node_modules/@radix-ui/react-slot": {
      "version": "1.2.4",
      "resolved": "https://registry.npmjs.org/@radix-ui/react-slot/-/react-slot-1.2.4.tgz",
      "integrity": "sha512-Jl+bCv8HxKnlTLVrcDE8zTMJ09R9/ukw4qBs/oZClOfoQk/cOTbDn+NceXfV7j09YPVQUryJPHurafcSg6EVKA==",
      "license": "MIT",
      "dependencies": {
        "@radix-ui/react-compose-refs": "1.1.2"
      },
      "peerDependencies": {
        "@types/react": "*",
        "react": "^16.8 || ^17.0 || ^18.0 || ^19.0 || ^19.0.0-rc"
      },
      "peerDependenciesMeta": {
        "@types/react": {
          "optional": true
        }
      }
    },
    "node_modules/@radix-ui/react-switch": {
      "version": "1.2.6",
      "resolved": "https://registry.npmjs.org/@radix-ui/react-switch/-/react-switch-1.2.6.tgz",
      "integrity": "sha512-bByzr1+ep1zk4VubeEVViV592vu2lHE2BZY5OnzehZqOOgogN80+mNtCqPkhn2gklJqOpxWgPoYTSnhBCqpOXQ==",
      "license": "MIT",
      "dependencies": {
        "@radix-ui/primitive": "1.1.3",
        "@radix-ui/react-compose-refs": "1.1.2",
        "@radix-ui/react-context": "1.1.2",
        "@radix-ui/react-primitive": "2.1.3",
        "@radix-ui/react-use-controllable-state": "1.2.2",
        "@radix-ui/react-use-previous": "1.1.1",
        "@radix-ui/react-use-size": "1.1.1"
      },
      "peerDependencies": {
        "@types/react": "*",
        "@types/react-dom": "*",
        "react": "^16.8 || ^17.0 || ^18.0 || ^19.0 || ^19.0.0-rc",
        "react-dom": "^16.8 || ^17.0 || ^18.0 || ^19.0 || ^19.0.0-rc"
      },
      "peerDependenciesMeta": {
        "@types/react": {
          "optional": true
        },
        "@types/react-dom": {
          "optional": true
        }
      }
    },
    "node_modules/@radix-ui/react-tabs": {
      "version": "1.1.13",
      "resolved": "https://registry.npmjs.org/@radix-ui/react-tabs/-/react-tabs-1.1.13.tgz",
      "integrity": "sha512-7xdcatg7/U+7+Udyoj2zodtI9H/IIopqo+YOIcZOq1nJwXWBZ9p8xiu5llXlekDbZkca79a/fozEYQXIA4sW6A==",
      "license": "MIT",
      "dependencies": {
        "@radix-ui/primitive": "1.1.3",
        "@radix-ui/react-context": "1.1.2",
        "@radix-ui/react-direction": "1.1.1",
        "@radix-ui/react-id": "1.1.1",
        "@radix-ui/react-presence": "1.1.5",
        "@radix-ui/react-primitive": "2.1.3",
        "@radix-ui/react-roving-focus": "1.1.11",
        "@radix-ui/react-use-controllable-state": "1.2.2"
      },
      "peerDependencies": {
        "@types/react": "*",
        "@types/react-dom": "*",
        "react": "^16.8 || ^17.0 || ^18.0 || ^19.0 || ^19.0.0-rc",
        "react-dom": "^16.8 || ^17.0 || ^18.0 || ^19.0 || ^19.0.0-rc"
      },
      "peerDependenciesMeta": {
        "@types/react": {
          "optional": true
        },
        "@types/react-dom": {
          "optional": true
        }
      }
    },
    "node_modules/@radix-ui/react-toast": {
      "version": "1.2.15",
      "resolved": "https://registry.npmjs.org/@radix-ui/react-toast/-/react-toast-1.2.15.tgz",
      "integrity": "sha512-3OSz3TacUWy4WtOXV38DggwxoqJK4+eDkNMl5Z/MJZaoUPaP4/9lf81xXMe1I2ReTAptverZUpbPY4wWwWyL5g==",
      "license": "MIT",
      "dependencies": {
        "@radix-ui/primitive": "1.1.3",
        "@radix-ui/react-collection": "1.1.7",
        "@radix-ui/react-compose-refs": "1.1.2",
        "@radix-ui/react-context": "1.1.2",
        "@radix-ui/react-dismissable-layer": "1.1.11",
        "@radix-ui/react-portal": "1.1.9",
        "@radix-ui/react-presence": "1.1.5",
        "@radix-ui/react-primitive": "2.1.3",
        "@radix-ui/react-use-callback-ref": "1.1.1",
        "@radix-ui/react-use-controllable-state": "1.2.2",
        "@radix-ui/react-use-layout-effect": "1.1.1",
        "@radix-ui/react-visually-hidden": "1.2.3"
      },
      "peerDependencies": {
        "@types/react": "*",
        "@types/react-dom": "*",
        "react": "^16.8 || ^17.0 || ^18.0 || ^19.0 || ^19.0.0-rc",
        "react-dom": "^16.8 || ^17.0 || ^18.0 || ^19.0 || ^19.0.0-rc"
      },
      "peerDependenciesMeta": {
        "@types/react": {
          "optional": true
        },
        "@types/react-dom": {
          "optional": true
        }
      }
    },
    "node_modules/@radix-ui/react-toggle": {
      "version": "1.1.10",
      "resolved": "https://registry.npmjs.org/@radix-ui/react-toggle/-/react-toggle-1.1.10.tgz",
      "integrity": "sha512-lS1odchhFTeZv3xwHH31YPObmJn8gOg7Lq12inrr0+BH/l3Tsq32VfjqH1oh80ARM3mlkfMic15n0kg4sD1poQ==",
      "license": "MIT",
      "dependencies": {
        "@radix-ui/primitive": "1.1.3",
        "@radix-ui/react-primitive": "2.1.3",
        "@radix-ui/react-use-controllable-state": "1.2.2"
      },
      "peerDependencies": {
        "@types/react": "*",
        "@types/react-dom": "*",
        "react": "^16.8 || ^17.0 || ^18.0 || ^19.0 || ^19.0.0-rc",
        "react-dom": "^16.8 || ^17.0 || ^18.0 || ^19.0 || ^19.0.0-rc"
      },
      "peerDependenciesMeta": {
        "@types/react": {
          "optional": true
        },
        "@types/react-dom": {
          "optional": true
        }
      }
    },
    "node_modules/@radix-ui/react-toggle-group": {
      "version": "1.1.11",
      "resolved": "https://registry.npmjs.org/@radix-ui/react-toggle-group/-/react-toggle-group-1.1.11.tgz",
      "integrity": "sha512-5umnS0T8JQzQT6HbPyO7Hh9dgd82NmS36DQr+X/YJ9ctFNCiiQd6IJAYYZ33LUwm8M+taCz5t2ui29fHZc4Y6Q==",
      "license": "MIT",
      "dependencies": {
        "@radix-ui/primitive": "1.1.3",
        "@radix-ui/react-context": "1.1.2",
        "@radix-ui/react-direction": "1.1.1",
        "@radix-ui/react-primitive": "2.1.3",
        "@radix-ui/react-roving-focus": "1.1.11",
        "@radix-ui/react-toggle": "1.1.10",
        "@radix-ui/react-use-controllable-state": "1.2.2"
      },
      "peerDependencies": {
        "@types/react": "*",
        "@types/react-dom": "*",
        "react": "^16.8 || ^17.0 || ^18.0 || ^19.0 || ^19.0.0-rc",
        "react-dom": "^16.8 || ^17.0 || ^18.0 || ^19.0 || ^19.0.0-rc"
      },
      "peerDependenciesMeta": {
        "@types/react": {
          "optional": true
        },
        "@types/react-dom": {
          "optional": true
        }
      }
    },
    "node_modules/@radix-ui/react-tooltip": {
      "version": "1.2.8",
      "resolved": "https://registry.npmjs.org/@radix-ui/react-tooltip/-/react-tooltip-1.2.8.tgz",
      "integrity": "sha512-tY7sVt1yL9ozIxvmbtN5qtmH2krXcBCfjEiCgKGLqunJHvgvZG2Pcl2oQ3kbcZARb1BGEHdkLzcYGO8ynVlieg==",
      "license": "MIT",
      "dependencies": {
        "@radix-ui/primitive": "1.1.3",
        "@radix-ui/react-compose-refs": "1.1.2",
        "@radix-ui/react-context": "1.1.2",
        "@radix-ui/react-dismissable-layer": "1.1.11",
        "@radix-ui/react-id": "1.1.1",
        "@radix-ui/react-popper": "1.2.8",
        "@radix-ui/react-portal": "1.1.9",
        "@radix-ui/react-presence": "1.1.5",
        "@radix-ui/react-primitive": "2.1.3",
        "@radix-ui/react-slot": "1.2.3",
        "@radix-ui/react-use-controllable-state": "1.2.2",
        "@radix-ui/react-visually-hidden": "1.2.3"
      },
      "peerDependencies": {
        "@types/react": "*",
        "@types/react-dom": "*",
        "react": "^16.8 || ^17.0 || ^18.0 || ^19.0 || ^19.0.0-rc",
        "react-dom": "^16.8 || ^17.0 || ^18.0 || ^19.0 || ^19.0.0-rc"
      },
      "peerDependenciesMeta": {
        "@types/react": {
          "optional": true
        },
        "@types/react-dom": {
          "optional": true
        }
      }
    },
    "node_modules/@radix-ui/react-tooltip/node_modules/@radix-ui/react-slot": {
      "version": "1.2.3",
      "resolved": "https://registry.npmjs.org/@radix-ui/react-slot/-/react-slot-1.2.3.tgz",
      "integrity": "sha512-aeNmHnBxbi2St0au6VBVC7JXFlhLlOnvIIlePNniyUNAClzmtAUEY8/pBiK3iHjufOlwA+c20/8jngo7xcrg8A==",
      "license": "MIT",
      "dependencies": {
        "@radix-ui/react-compose-refs": "1.1.2"
      },
      "peerDependencies": {
        "@types/react": "*",
        "react": "^16.8 || ^17.0 || ^18.0 || ^19.0 || ^19.0.0-rc"
      },
      "peerDependenciesMeta": {
        "@types/react": {
          "optional": true
        }
      }
    },
    "node_modules/@radix-ui/react-use-callback-ref": {
      "version": "1.1.1",
      "resolved": "https://registry.npmjs.org/@radix-ui/react-use-callback-ref/-/react-use-callback-ref-1.1.1.tgz",
      "integrity": "sha512-FkBMwD+qbGQeMu1cOHnuGB6x4yzPjho8ap5WtbEJ26umhgqVXbhekKUQO+hZEL1vU92a3wHwdp0HAcqAUF5iDg==",
      "license": "MIT",
      "peerDependencies": {
        "@types/react": "*",
        "react": "^16.8 || ^17.0 || ^18.0 || ^19.0 || ^19.0.0-rc"
      },
      "peerDependenciesMeta": {
        "@types/react": {
          "optional": true
        }
      }
    },
    "node_modules/@radix-ui/react-use-controllable-state": {
      "version": "1.2.2",
      "resolved": "https://registry.npmjs.org/@radix-ui/react-use-controllable-state/-/react-use-controllable-state-1.2.2.tgz",
      "integrity": "sha512-BjasUjixPFdS+NKkypcyyN5Pmg83Olst0+c6vGov0diwTEo6mgdqVR6hxcEgFuh4QrAs7Rc+9KuGJ9TVCj0Zzg==",
      "license": "MIT",
      "dependencies": {
        "@radix-ui/react-use-effect-event": "0.0.2",
        "@radix-ui/react-use-layout-effect": "1.1.1"
      },
      "peerDependencies": {
        "@types/react": "*",
        "react": "^16.8 || ^17.0 || ^18.0 || ^19.0 || ^19.0.0-rc"
      },
      "peerDependenciesMeta": {
        "@types/react": {
          "optional": true
        }
      }
    },
    "node_modules/@radix-ui/react-use-effect-event": {
      "version": "0.0.2",
      "resolved": "https://registry.npmjs.org/@radix-ui/react-use-effect-event/-/react-use-effect-event-0.0.2.tgz",
      "integrity": "sha512-Qp8WbZOBe+blgpuUT+lw2xheLP8q0oatc9UpmiemEICxGvFLYmHm9QowVZGHtJlGbS6A6yJ3iViad/2cVjnOiA==",
      "license": "MIT",
      "dependencies": {
        "@radix-ui/react-use-layout-effect": "1.1.1"
      },
      "peerDependencies": {
        "@types/react": "*",
        "react": "^16.8 || ^17.0 || ^18.0 || ^19.0 || ^19.0.0-rc"
      },
      "peerDependenciesMeta": {
        "@types/react": {
          "optional": true
        }
      }
    },
    "node_modules/@radix-ui/react-use-escape-keydown": {
      "version": "1.1.1",
      "resolved": "https://registry.npmjs.org/@radix-ui/react-use-escape-keydown/-/react-use-escape-keydown-1.1.1.tgz",
      "integrity": "sha512-Il0+boE7w/XebUHyBjroE+DbByORGR9KKmITzbR7MyQ4akpORYP/ZmbhAr0DG7RmmBqoOnZdy2QlvajJ2QA59g==",
      "license": "MIT",
      "dependencies": {
        "@radix-ui/react-use-callback-ref": "1.1.1"
      },
      "peerDependencies": {
        "@types/react": "*",
        "react": "^16.8 || ^17.0 || ^18.0 || ^19.0 || ^19.0.0-rc"
      },
      "peerDependenciesMeta": {
        "@types/react": {
          "optional": true
        }
      }
    },
    "node_modules/@radix-ui/react-use-is-hydrated": {
      "version": "0.1.0",
      "resolved": "https://registry.npmjs.org/@radix-ui/react-use-is-hydrated/-/react-use-is-hydrated-0.1.0.tgz",
      "integrity": "sha512-U+UORVEq+cTnRIaostJv9AGdV3G6Y+zbVd+12e18jQ5A3c0xL03IhnHuiU4UV69wolOQp5GfR58NW/EgdQhwOA==",
      "license": "MIT",
      "dependencies": {
        "use-sync-external-store": "^1.5.0"
      },
      "peerDependencies": {
        "@types/react": "*",
        "react": "^16.8 || ^17.0 || ^18.0 || ^19.0 || ^19.0.0-rc"
      },
      "peerDependenciesMeta": {
        "@types/react": {
          "optional": true
        }
      }
    },
    "node_modules/@radix-ui/react-use-layout-effect": {
      "version": "1.1.1",
      "resolved": "https://registry.npmjs.org/@radix-ui/react-use-layout-effect/-/react-use-layout-effect-1.1.1.tgz",
      "integrity": "sha512-RbJRS4UWQFkzHTTwVymMTUv8EqYhOp8dOOviLj2ugtTiXRaRQS7GLGxZTLL1jWhMeoSCf5zmcZkqTl9IiYfXcQ==",
      "license": "MIT",
      "peerDependencies": {
        "@types/react": "*",
        "react": "^16.8 || ^17.0 || ^18.0 || ^19.0 || ^19.0.0-rc"
      },
      "peerDependenciesMeta": {
        "@types/react": {
          "optional": true
        }
      }
    },
    "node_modules/@radix-ui/react-use-previous": {
      "version": "1.1.1",
      "resolved": "https://registry.npmjs.org/@radix-ui/react-use-previous/-/react-use-previous-1.1.1.tgz",
      "integrity": "sha512-2dHfToCj/pzca2Ck724OZ5L0EVrr3eHRNsG/b3xQJLA2hZpVCS99bLAX+hm1IHXDEnzU6by5z/5MIY794/a8NQ==",
      "license": "MIT",
      "peerDependencies": {
        "@types/react": "*",
        "react": "^16.8 || ^17.0 || ^18.0 || ^19.0 || ^19.0.0-rc"
      },
      "peerDependenciesMeta": {
        "@types/react": {
          "optional": true
        }
      }
    },
    "node_modules/@radix-ui/react-use-rect": {
      "version": "1.1.1",
      "resolved": "https://registry.npmjs.org/@radix-ui/react-use-rect/-/react-use-rect-1.1.1.tgz",
      "integrity": "sha512-QTYuDesS0VtuHNNvMh+CjlKJ4LJickCMUAqjlE3+j8w+RlRpwyX3apEQKGFzbZGdo7XNG1tXa+bQqIE7HIXT2w==",
      "license": "MIT",
      "dependencies": {
        "@radix-ui/rect": "1.1.1"
      },
      "peerDependencies": {
        "@types/react": "*",
        "react": "^16.8 || ^17.0 || ^18.0 || ^19.0 || ^19.0.0-rc"
      },
      "peerDependenciesMeta": {
        "@types/react": {
          "optional": true
        }
      }
    },
    "node_modules/@radix-ui/react-use-size": {
      "version": "1.1.1",
      "resolved": "https://registry.npmjs.org/@radix-ui/react-use-size/-/react-use-size-1.1.1.tgz",
      "integrity": "sha512-ewrXRDTAqAXlkl6t/fkXWNAhFX9I+CkKlw6zjEwk86RSPKwZr3xpBRso655aqYafwtnbpHLj6toFzmd6xdVptQ==",
      "license": "MIT",
      "dependencies": {
        "@radix-ui/react-use-layout-effect": "1.1.1"
      },
      "peerDependencies": {
        "@types/react": "*",
        "react": "^16.8 || ^17.0 || ^18.0 || ^19.0 || ^19.0.0-rc"
      },
      "peerDependenciesMeta": {
        "@types/react": {
          "optional": true
        }
      }
    },
    "node_modules/@radix-ui/react-visually-hidden": {
      "version": "1.2.3",
      "resolved": "https://registry.npmjs.org/@radix-ui/react-visually-hidden/-/react-visually-hidden-1.2.3.tgz",
      "integrity": "sha512-pzJq12tEaaIhqjbzpCuv/OypJY/BPavOofm+dbab+MHLajy277+1lLm6JFcGgF5eskJ6mquGirhXY2GD/8u8Ug==",
      "license": "MIT",
      "dependencies": {
        "@radix-ui/react-primitive": "2.1.3"
      },
      "peerDependencies": {
        "@types/react": "*",
        "@types/react-dom": "*",
        "react": "^16.8 || ^17.0 || ^18.0 || ^19.0 || ^19.0.0-rc",
        "react-dom": "^16.8 || ^17.0 || ^18.0 || ^19.0 || ^19.0.0-rc"
      },
      "peerDependenciesMeta": {
        "@types/react": {
          "optional": true
        },
        "@types/react-dom": {
          "optional": true
        }
      }
    },
    "node_modules/@radix-ui/rect": {
      "version": "1.1.1",
      "resolved": "https://registry.npmjs.org/@radix-ui/rect/-/rect-1.1.1.tgz",
      "integrity": "sha512-HPwpGIzkl28mWyZqG52jiqDJ12waP11Pa1lGoiyUkIEuMLBP0oeK/C89esbXrxsky5we7dfd8U58nm0SgAWpVw==",
      "license": "MIT"
    },
    "node_modules/@react-leaflet/core": {
      "version": "2.1.0",
      "resolved": "https://registry.npmjs.org/@react-leaflet/core/-/core-2.1.0.tgz",
      "integrity": "sha512-Qk7Pfu8BSarKGqILj4x7bCSZ1pjuAPZ+qmRwH5S7mDS91VSbVVsJSrW4qA+GPrro8t69gFYVMWb1Zc4yFmPiVg==",
      "license": "Hippocratic-2.1",
      "peerDependencies": {
        "leaflet": "^1.9.0",
        "react": "^18.0.0",
        "react-dom": "^18.0.0"
      }
    },
    "node_modules/@remix-run/router": {
      "version": "1.23.3",
      "resolved": "https://registry.npmjs.org/@remix-run/router/-/router-1.23.3.tgz",
      "integrity": "sha512-4An71tdz9X8+3sI4Qqqd2LWd9vS39J7sqd9EU4Scw7TJE/qB10Flv/UuqbPVgfQV9XoK8Np6jNquZitnZq5i+Q==",
      "license": "MIT",
      "engines": {
        "node": ">=14.0.0"
      }
    },
    "node_modules/@rolldown/pluginutils": {
      "version": "1.0.0-beta.27",
      "resolved": "https://registry.npmjs.org/@rolldown/pluginutils/-/pluginutils-1.0.0-beta.27.tgz",
      "integrity": "sha512-+d0F4MKMCbeVUJwG96uQ4SgAznZNSq93I3V+9NHA4OpvqG8mRCpGdKmK8l/dl02h2CCDHwW2FqilnTyDcAnqjA==",
      "dev": true,
      "license": "MIT"
    },
    "node_modules/@rollup/rollup-android-arm-eabi": {
      "version": "4.62.2",
      "resolved": "https://registry.npmjs.org/@rollup/rollup-android-arm-eabi/-/rollup-android-arm-eabi-4.62.2.tgz",
      "integrity": "sha512-6o7ZLZK+BeenkZCFNDXqpbjw9bD6nuWonvS/lwQJp7NoVVxm6p3qE7qQ5jGuBjiFsgvqjD8mZAU5oWxTmbOeOg==",
      "cpu": [
        "arm"
      ],
      "dev": true,
      "license": "MIT",
      "optional": true,
      "os": [
        "android"
      ]
    },
    "node_modules/@rollup/rollup-android-arm64": {
      "version": "4.62.2",
      "resolved": "https://registry.npmjs.org/@rollup/rollup-android-arm64/-/rollup-android-arm64-4.62.2.tgz",
      "integrity": "sha512-BaH7BllCACHoH1LguOU56UItGfUWjujlO65kS9LAodViaN4bwIKd7oeW/ZHJ/4ljr/7MIiENnNy3HJ0zXv8Zkw==",
      "cpu": [
        "arm64"
      ],
      "dev": true,
      "license": "MIT",
      "optional": true,
      "os": [
        "android"
      ]
    },
    "node_modules/@rollup/rollup-darwin-arm64": {
      "version": "4.62.2",
      "resolved": "https://registry.npmjs.org/@rollup/rollup-darwin-arm64/-/rollup-darwin-arm64-4.62.2.tgz",
      "integrity": "sha512-v39RCCvj4He82I9sFmk+M1VZ0PLM9sfsLVikjfx2hYBNALhrrOR2D3JjQA6AhlaSOgcR+RzrKY7e1+bT6SUO/A==",
      "cpu": [
        "arm64"
      ],
      "dev": true,
      "license": "MIT",
      "optional": true,
      "os": [
        "darwin"
      ]
    },
    "node_modules/@rollup/rollup-darwin-x64": {
      "version": "4.62.2",
      "resolved": "https://registry.npmjs.org/@rollup/rollup-darwin-x64/-/rollup-darwin-x64-4.62.2.tgz",
      "integrity": "sha512-yl0y2vq3S3lHeuXhEdss6TWfKW8vkujImO12tn4ZkG/4oghr09LvdYm2RElVjokTQiUvDUGXLGsYeLqUMCKpGA==",
      "cpu": [
        "x64"
      ],
      "dev": true,
      "license": "MIT",
      "optional": true,
      "os": [
        "darwin"
      ]
    },
    "node_modules/@rollup/rollup-freebsd-arm64": {
      "version": "4.62.2",
      "resolved": "https://registry.npmjs.org/@rollup/rollup-freebsd-arm64/-/rollup-freebsd-arm64-4.62.2.tgz",
      "integrity": "sha512-tT4pvt4qXD+vEoezupCWi+a1F0vvDiksiHc+PxRlYTOH1I6/X4id9jPxTP+Fg+545euaFT1jJVs4CEdHZAU1vw==",
      "cpu": [
        "arm64"
      ],
      "dev": true,
      "license": "MIT",
      "optional": true,
      "os": [
        "freebsd"
      ]
    },
    "node_modules/@rollup/rollup-freebsd-x64": {
      "version": "4.62.2",
      "resolved": "https://registry.npmjs.org/@rollup/rollup-freebsd-x64/-/rollup-freebsd-x64-4.62.2.tgz",
      "integrity": "sha512-6nU5F2wCW+qvCBhTn1pdIU3bzsIoF7EUwsCDRxilWGprQR6yd508YnH9+OKFCwpfS8pjZqDUmnCAr7exax0XCg==",
      "cpu": [
        "x64"
      ],
      "dev": true,
      "license": "MIT",
      "optional": true,
      "os": [
        "freebsd"
      ]
    },
    "node_modules/@rollup/rollup-linux-arm-gnueabihf": {
      "version": "4.62.2",
      "resolved": "https://registry.npmjs.org/@rollup/rollup-linux-arm-gnueabihf/-/rollup-linux-arm-gnueabihf-4.62.2.tgz",
      "integrity": "sha512-n1GJHPOvpIfhi3TmrCeh6S6URt9BFCt0KQE3qvexyGCTAKpR4Lg+eWvNZEqu7epxwus/8ElT3hacYEucm49SZg==",
      "cpu": [
        "arm"
      ],
      "dev": true,
      "license": "MIT",
      "optional": true,
      "os": [
        "linux"
      ]
    },
    "node_modules/@rollup/rollup-linux-arm-musleabihf": {
      "version": "4.62.2",
      "resolved": "https://registry.npmjs.org/@rollup/rollup-linux-arm-musleabihf/-/rollup-linux-arm-musleabihf-4.62.2.tgz",
      "integrity": "sha512-JqgflS8wEB+UXV/vS1RpRbifGBeN4D5lz8D8oOFbFZw4vedvdOgCFAjfBmIMdW3yL10XpQQ0Ambepw6MXrhOnA==",
      "cpu": [
        "arm"
      ],
      "dev": true,
      "license": "MIT",
      "optional": true,
      "os": [
        "linux"
      ]
    },
    "node_modules/@rollup/rollup-linux-arm64-gnu": {
      "version": "4.62.2",
      "resolved": "https://registry.npmjs.org/@rollup/rollup-linux-arm64-gnu/-/rollup-linux-arm64-gnu-4.62.2.tgz",
      "integrity": "sha512-wnFJkogWvN4jm/hQRF2UBaeUmk20j5+DmHvoyWii2b8HJDyvz1MF2OU/6ynXt2KR63rbZLWkFpoytpdc/yBuSA==",
      "cpu": [
        "arm64"
      ],
      "dev": true,
      "license": "MIT",
      "optional": true,
      "os": [
        "linux"
      ]
    },
    "node_modules/@rollup/rollup-linux-arm64-musl": {
      "version": "4.62.2",
      "resolved": "https://registry.npmjs.org/@rollup/rollup-linux-arm64-musl/-/rollup-linux-arm64-musl-4.62.2.tgz",
      "integrity": "sha512-HVu2bp0zhvJ8xHEV9+UUs7S90VadmBSY3LcIMvozbPo4AuMGDWlz3ymHLHZPX4hR67TKTt8Qp5PJ5RBg/i+RMQ==",
      "cpu": [
        "arm64"
      ],
      "dev": true,
      "license": "MIT",
      "optional": true,
      "os": [
        "linux"
      ]
    },
    "node_modules/@rollup/rollup-linux-loong64-gnu": {
      "version": "4.62.2",
      "resolved": "https://registry.npmjs.org/@rollup/rollup-linux-loong64-gnu/-/rollup-linux-loong64-gnu-4.62.2.tgz",
      "integrity": "sha512-mQqqAV8QaoSgr9I2fKDLY2BAVvmKjWoGiu/cSYQonsLvtqwEn1E4QYfnCOcp5zoEqNhsDYin1s6jx/VJmrxlZg==",
      "cpu": [
        "loong64"
      ],
      "dev": true,
      "license": "MIT",
      "optional": true,
      "os": [
        "linux"
      ]
    },
    "node_modules/@rollup/rollup-linux-loong64-musl": {
      "version": "4.62.2",
      "resolved": "https://registry.npmjs.org/@rollup/rollup-linux-loong64-musl/-/rollup-linux-loong64-musl-4.62.2.tgz",
      "integrity": "sha512-IxKLoxCQ2IWi6bT2akyDUBGsOImDKB+sPp4EsTmwFQ/fMwpCKm8uLSSgP/Kx/QYUgKis6SEZ5/Nlhup0DIA0PQ==",
      "cpu": [
        "loong64"
      ],
      "dev": true,
      "license": "MIT",
      "optional": true,
      "os": [
        "linux"
      ]
    },
    "node_modules/@rollup/rollup-linux-ppc64-gnu": {
      "version": "4.62.2",
      "resolved": "https://registry.npmjs.org/@rollup/rollup-linux-ppc64-gnu/-/rollup-linux-ppc64-gnu-4.62.2.tgz",
      "integrity": "sha512-Mk5ha2RQSgyFfmYYLkBpPnUk8D8FriBxesO1u9O75X0mHgXL1UQcH5Itl2lurWL2tj0RxV9b9tJgipac0hRY9A==",
      "cpu": [
        "ppc64"
      ],
      "dev": true,
      "license": "MIT",
      "optional": true,
      "os": [
        "linux"
      ]
    },
    "node_modules/@rollup/rollup-linux-ppc64-musl": {
      "version": "4.62.2",
      "resolved": "https://registry.npmjs.org/@rollup/rollup-linux-ppc64-musl/-/rollup-linux-ppc64-musl-4.62.2.tgz",
      "integrity": "sha512-CjvEnqJL/0/TQ3TXX3OPIJ/kmBellrWd4heXUmHeJlTnmwjKpSJzoehLaL6Xk0ZnMHBu9dZuFADNOrtjF4v+2w==",
      "cpu": [
        "ppc64"
      ],
      "dev": true,
      "license": "MIT",
      "optional": true,
      "os": [
        "linux"
      ]
    },
    "node_modules/@rollup/rollup-linux-riscv64-gnu": {
      "version": "4.62.2",
      "resolved": "https://registry.npmjs.org/@rollup/rollup-linux-riscv64-gnu/-/rollup-linux-riscv64-gnu-4.62.2.tgz",
      "integrity": "sha512-1SiZbzwdkaDURsew/tSOrooKiYy7EQGT6m8ufavAi9NEyQb/6VuIxFXAL1fqa4iZe3g4NbNk4P7J32z2tw5Mgg==",
      "cpu": [
        "riscv64"
      ],
      "dev": true,
      "license": "MIT",
      "optional": true,
      "os": [
        "linux"
      ]
    },
    "node_modules/@rollup/rollup-linux-riscv64-musl": {
      "version": "4.62.2",
      "resolved": "https://registry.npmjs.org/@rollup/rollup-linux-riscv64-musl/-/rollup-linux-riscv64-musl-4.62.2.tgz",
      "integrity": "sha512-nQts12zJ3NQRoE6uYljOH89v7szzLDvG2JD/vsX+vGXU8w/At1GowTZ5/7qeFQ8m7L55rpR8Okugnuo5bgjy2Q==",
      "cpu": [
        "riscv64"
      ],
      "dev": true,
      "license": "MIT",
      "optional": true,
      "os": [
        "linux"
      ]
    },
    "node_modules/@rollup/rollup-linux-s390x-gnu": {
      "version": "4.62.2",
      "resolved": "https://registry.npmjs.org/@rollup/rollup-linux-s390x-gnu/-/rollup-linux-s390x-gnu-4.62.2.tgz",
      "integrity": "sha512-E9/ll019jhPIJgpzfZoIkBGhcz+kKNgVWYRY0zr9srBdPPFVpvOKW8VaJKUbeK+eZXyQF9ltME+Kk6affeaPgg==",
      "cpu": [
        "s390x"
      ],
      "dev": true,
      "license": "MIT",
      "optional": true,
      "os": [
        "linux"
      ]
    },
    "node_modules/@rollup/rollup-linux-x64-gnu": {
      "version": "4.62.2",
      "resolved": "https://registry.npmjs.org/@rollup/rollup-linux-x64-gnu/-/rollup-linux-x64-gnu-4.62.2.tgz",
      "integrity": "sha512-5BqxR/pshjey51iliyzTD5Xi3EN0aLmQ2lZ3lvefVV9c82BvrLo2/6OT55iifpWBufs6kdwWbuOKS841DrmK9A==",
      "cpu": [
        "x64"
      ],
      "dev": true,
      "license": "MIT",
      "optional": true,
      "os": [
        "linux"
      ]
    },
    "node_modules/@rollup/rollup-linux-x64-musl": {
      "version": "4.62.2",
      "resolved": "https://registry.npmjs.org/@rollup/rollup-linux-x64-musl/-/rollup-linux-x64-musl-4.62.2.tgz",
      "integrity": "sha512-uNN83XxQrRAh/w0/pmAfibcwyb6YWt4gP+dpnQKPVJshAloQ785ii8CT8ZCIxkGg9opVsvAlGhFitSm6D1Jjpg==",
      "cpu": [
        "x64"
      ],
      "dev": true,
      "license": "MIT",
      "optional": true,
      "os": [
        "linux"
      ]
    },
    "node_modules/@rollup/rollup-openbsd-x64": {
      "version": "4.62.2",
      "resolved": "https://registry.npmjs.org/@rollup/rollup-openbsd-x64/-/rollup-openbsd-x64-4.62.2.tgz",
      "integrity": "sha512-srjEIxSH3LRnJN6THczDHWQplqEMFiAJrTab0msUryh9kwNpkICf3Ea6q6MN/2cZwRFUNx5w+h6Hpi4QuHS6Zg==",
      "cpu": [
        "x64"
      ],
      "dev": true,
      "license": "MIT",
      "optional": true,
      "os": [
        "openbsd"
      ]
    },
    "node_modules/@rollup/rollup-openharmony-arm64": {
      "version": "4.62.2",
      "resolved": "https://registry.npmjs.org/@rollup/rollup-openharmony-arm64/-/rollup-openharmony-arm64-4.62.2.tgz",
      "integrity": "sha512-8hOJnxgbyObnCm5AlRA3A931xX19xq80RjVTKgJOvEKWqJruP/Uf12IbAOaDjjEXYRewwHLfmF0YRIdK3OwKWA==",
      "cpu": [
        "arm64"
      ],
      "dev": true,
      "license": "MIT",
      "optional": true,
      "os": [
        "openharmony"
      ]
    },
    "node_modules/@rollup/rollup-win32-arm64-msvc": {
      "version": "4.62.2",
      "resolved": "https://registry.npmjs.org/@rollup/rollup-win32-arm64-msvc/-/rollup-win32-arm64-msvc-4.62.2.tgz",
      "integrity": "sha512-mmF4AY1i0hG/bLWUctUq59gtmgaSIRa3cu/A3JFRp/sCNEme2bgDEiDS22P9FbnJB8NJNF4jPJiSP5RHQpUTDg==",
      "cpu": [
        "arm64"
      ],
      "dev": true,
      "license": "MIT",
      "optional": true,
      "os": [
        "win32"
      ]
    },
    "node_modules/@rollup/rollup-win32-ia32-msvc": {
      "version": "4.62.2",
      "resolved": "https://registry.npmjs.org/@rollup/rollup-win32-ia32-msvc/-/rollup-win32-ia32-msvc-4.62.2.tgz",
      "integrity": "sha512-DZgkknc6jhHrk46V25vbAM0zZkyP0nSDkJB8/dRkLTxv470dOmWDqGoEJl/9A0dFfS7yE3REOwNDxpHwSLSt0Q==",
      "cpu": [
        "ia32"
      ],
      "dev": true,
      "license": "MIT",
      "optional": true,
      "os": [
        "win32"
      ]
    },
    "node_modules/@rollup/rollup-win32-x64-gnu": {
      "version": "4.62.2",
      "resolved": "https://registry.npmjs.org/@rollup/rollup-win32-x64-gnu/-/rollup-win32-x64-gnu-4.62.2.tgz",
      "integrity": "sha512-T6xr6ucWSFto+VGajA8YH26LdpHRuP4YLHEKAtCWvJDOlnmWcDZVCI2Jmjr+IFHDlt2zRaTAKE4tfjTaWLgJBg==",
      "cpu": [
        "x64"
      ],
      "dev": true,
      "license": "MIT",
      "optional": true,
      "os": [
        "win32"
      ]
    },
    "node_modules/@rollup/rollup-win32-x64-msvc": {
      "version": "4.62.2",
      "resolved": "https://registry.npmjs.org/@rollup/rollup-win32-x64-msvc/-/rollup-win32-x64-msvc-4.62.2.tgz",
      "integrity": "sha512-BfzEnDJOt9T8M989/lA37EcJgat01wLRnoi5dQf3QzOH7jzpqTAzdDbVfRljVr5r+jzKqpbHeyOfAaXxAd0PAA==",
      "cpu": [
        "x64"
      ],
      "dev": true,
      "license": "MIT",
      "optional": true,
      "os": [
        "win32"
      ]
    },
    "node_modules/@socket.io/component-emitter": {
      "version": "3.1.2",
      "resolved": "https://registry.npmjs.org/@socket.io/component-emitter/-/component-emitter-3.1.2.tgz",
      "integrity": "sha512-9BCxFwvbGg/RsZK9tjXd8s4UcwR0MWeFQ1XEKIQVVvAGJyINdrqKMcTRyLoK8Rse1GjzLV9cwjWV1olXRWEXVA==",
      "license": "MIT"
    },
    "node_modules/@standard-schema/utils": {
      "version": "0.3.0",
      "resolved": "https://registry.npmjs.org/@standard-schema/utils/-/utils-0.3.0.tgz",
      "integrity": "sha512-e7Mew686owMaPJVNNLs55PUvgz371nKgwsc4vxE49zsODpJEnxgxRo2y/OKrqueavXgZNMDVj3DdHFlaSAeU8g==",
      "license": "MIT"
    },
    "node_modules/@stripe/react-stripe-js": {
      "version": "3.10.0",
      "resolved": "https://registry.npmjs.org/@stripe/react-stripe-js/-/react-stripe-js-3.10.0.tgz",
      "integrity": "sha512-UPqHZwMwDzGSax0ZI7XlxR3tZSpgIiZdk3CiwjbTK978phwR/fFXeAXQcN/h8wTAjR4ZIAzdlI9DbOqJhuJdeg==",
      "license": "MIT",
      "dependencies": {
        "prop-types": "^15.7.2"
      },
      "peerDependencies": {
        "@stripe/stripe-js": ">=1.44.1 <8.0.0",
        "react": ">=16.8.0 <20.0.0",
        "react-dom": ">=16.8.0 <20.0.0"
      }
    },
    "node_modules/@stripe/stripe-js": {
      "version": "5.10.0",
      "resolved": "https://registry.npmjs.org/@stripe/stripe-js/-/stripe-js-5.10.0.tgz",
      "integrity": "sha512-PTigkxMdMUP6B5ISS7jMqJAKhgrhZwjprDqR1eATtFfh0OpKVNp110xiH+goeVdrJ29/4LeZJR4FaHHWstsu0A==",
      "license": "MIT",
      "engines": {
        "node": ">=12.16"
      }
    },
    "node_modules/@tanstack/query-core": {
      "version": "5.90.20",
      "resolved": "https://registry.npmjs.org/@tanstack/query-core/-/query-core-5.90.20.tgz",
      "integrity": "sha512-OMD2HLpNouXEfZJWcKeVKUgQ5n+n3A2JFmBaScpNDUqSrQSjiveC7dKMe53uJUg1nDG16ttFPz2xfilz6i2uVg==",
      "license": "MIT",
      "funding": {
        "type": "github",
        "url": "https://github.com/sponsors/tannerlinsley"
      }
    },
    "node_modules/@tanstack/react-query": {
      "version": "5.90.21",
      "resolved": "https://registry.npmjs.org/@tanstack/react-query/-/react-query-5.90.21.tgz",
      "integrity": "sha512-0Lu6y5t+tvlTJMTO7oh5NSpJfpg/5D41LlThfepTixPYkJ0sE2Jj0m0f6yYqujBwIXlId87e234+MxG3D3g7kg==",
      "license": "MIT",
      "dependencies": {
        "@tanstack/query-core": "5.90.20"
      },
      "funding": {
        "type": "github",
        "url": "https://github.com/sponsors/tannerlinsley"
      },
      "peerDependencies": {
        "react": "^18 || ^19"
      }
    },
    "node_modules/@types/babel__core": {
      "version": "7.20.5",
      "resolved": "https://registry.npmjs.org/@types/babel__core/-/babel__core-7.20.5.tgz",
      "integrity": "sha512-qoQprZvz5wQFJwMDqeseRXWv3rqMvhgpbXFfVyWhbx9X47POIA6i/+dXefEmZKoAgOaTdaIgNSMqMIU61yRyzA==",
      "dev": true,
      "license": "MIT",
      "dependencies": {
        "@babel/parser": "^7.20.7",
        "@babel/types": "^7.20.7",
        "@types/babel__generator": "*",
        "@types/babel__template": "*",
        "@types/babel__traverse": "*"
      }
    },
    "node_modules/@types/babel__generator": {
      "version": "7.27.0",
      "resolved": "https://registry.npmjs.org/@types/babel__generator/-/babel__generator-7.27.0.tgz",
      "integrity": "sha512-ufFd2Xi92OAVPYsy+P4n7/U7e68fex0+Ee8gSG9KX7eo084CWiQ4sdxktvdl0bOPupXtVJPY19zk6EwWqUQ8lg==",
      "dev": true,
      "license": "MIT",
      "dependencies": {
        "@babel/types": "^7.0.0"
      }
    },
    "node_modules/@types/babel__template": {
      "version": "7.4.4",
      "resolved": "https://registry.npmjs.org/@types/babel__template/-/babel__template-7.4.4.tgz",
      "integrity": "sha512-h/NUaSyG5EyxBIp8YRxo4RMe2/qQgvyowRwVMzhYhBCONbW8PUsg4lkFMrhgZhUe5z3L3MiLDuvyJ/CaPa2A8A==",
      "dev": true,
      "license": "MIT",
      "dependencies": {
        "@babel/parser": "^7.1.0",
        "@babel/types": "^7.0.0"
      }
    },
    "node_modules/@types/babel__traverse": {
      "version": "7.28.0",
      "resolved": "https://registry.npmjs.org/@types/babel__traverse/-/babel__traverse-7.28.0.tgz",
      "integrity": "sha512-8PvcXf70gTDZBgt9ptxJ8elBeBjcLOAcOtoO/mPJjtji1+CdGbHgm77om1GrsPxsiE+uXIpNSK64UYaIwQXd4Q==",
      "dev": true,
      "license": "MIT",
      "dependencies": {
        "@babel/types": "^7.28.2"
      }
    },
    "node_modules/@types/d3-array": {
      "version": "3.2.2",
      "resolved": "https://registry.npmjs.org/@types/d3-array/-/d3-array-3.2.2.tgz",
      "integrity": "sha512-hOLWVbm7uRza0BYXpIIW5pxfrKe0W+D5lrFiAEYR+pb6w3N2SwSMaJbXdUfSEv+dT4MfHBLtn5js0LAWaO6otw==",
      "license": "MIT"
    },
    "node_modules/@types/d3-color": {
      "version": "3.1.3",
      "resolved": "https://registry.npmjs.org/@types/d3-color/-/d3-color-3.1.3.tgz",
      "integrity": "sha512-iO90scth9WAbmgv7ogoq57O9YpKmFBbmoEoCHDB2xMBY0+/KVrqAaCDyCE16dUspeOvIxFFRI+0sEtqDqy2b4A==",
      "license": "MIT"
    },
    "node_modules/@types/d3-ease": {
      "version": "3.0.2",
      "resolved": "https://registry.npmjs.org/@types/d3-ease/-/d3-ease-3.0.2.tgz",
      "integrity": "sha512-NcV1JjO5oDzoK26oMzbILE6HW7uVXOHLQvHshBUW4UMdZGfiY6v5BeQwh9a9tCzv+CeefZQHJt5SRgK154RtiA==",
      "license": "MIT"
    },
    "node_modules/@types/d3-interpolate": {
      "version": "3.0.4",
      "resolved": "https://registry.npmjs.org/@types/d3-interpolate/-/d3-interpolate-3.0.4.tgz",
      "integrity": "sha512-mgLPETlrpVV1YRJIglr4Ez47g7Yxjl1lj7YKsiMCb27VJH9W8NVM6Bb9d8kkpG/uAQS5AmbA48q2IAolKKo1MA==",
      "license": "MIT",
      "dependencies": {
        "@types/d3-color": "*"
      }
    },
    "node_modules/@types/d3-path": {
      "version": "3.1.1",
      "resolved": "https://registry.npmjs.org/@types/d3-path/-/d3-path-3.1.1.tgz",
      "integrity": "sha512-VMZBYyQvbGmWyWVea0EHs/BwLgxc+MKi1zLDCONksozI4YJMcTt8ZEuIR4Sb1MMTE8MMW49v0IwI5+b7RmfWlg==",
      "license": "MIT"
    },
    "node_modules/@types/d3-scale": {
      "version": "4.0.9",
      "resolved": "https://registry.npmjs.org/@types/d3-scale/-/d3-scale-4.0.9.tgz",
      "integrity": "sha512-dLmtwB8zkAeO/juAMfnV+sItKjlsw2lKdZVVy6LRr0cBmegxSABiLEpGVmSJJ8O08i4+sGR6qQtb6WtuwJdvVw==",
      "license": "MIT",
      "dependencies": {
        "@types/d3-time": "*"
      }
    },
    "node_modules/@types/d3-shape": {
      "version": "3.1.8",
      "resolved": "https://registry.npmjs.org/@types/d3-shape/-/d3-shape-3.1.8.tgz",
      "integrity": "sha512-lae0iWfcDeR7qt7rA88BNiqdvPS5pFVPpo5OfjElwNaT2yyekbM0C9vK+yqBqEmHr6lDkRnYNoTBYlAgJa7a4w==",
      "license": "MIT",
      "dependencies": {
        "@types/d3-path": "*"
      }
    },
    "node_modules/@types/d3-time": {
      "version": "3.0.4",
      "resolved": "https://registry.npmjs.org/@types/d3-time/-/d3-time-3.0.4.tgz",
      "integrity": "sha512-yuzZug1nkAAaBlBBikKZTgzCeA+k1uy4ZFwWANOfKw5z5LRhV0gNA7gNkKm7HoK+HRN0wX3EkxGk0fpbWhmB7g==",
      "license": "MIT"
    },
    "node_modules/@types/d3-timer": {
      "version": "3.0.2",
      "resolved": "https://registry.npmjs.org/@types/d3-timer/-/d3-timer-3.0.2.tgz",
      "integrity": "sha512-Ps3T8E8dZDam6fUyNiMkekK3XUsaUEik+idO9/YjPtfj2qruF8tFBXS7XhtE4iIXBLxhmLjP3SXpLhVf21I9Lw==",
      "license": "MIT"
    },
    "node_modules/@types/debug": {
      "version": "4.1.12",
      "resolved": "https://registry.npmjs.org/@types/debug/-/debug-4.1.12.tgz",
      "integrity": "sha512-vIChWdVG3LG1SMxEvI/AK+FWJthlrqlTu7fbrlywTkkaONwk/UAGaULXRlf8vkzFBLVm0zkMdCquhL5aOjhXPQ==",
      "license": "MIT",
      "dependencies": {
        "@types/ms": "*"
      }
    },
    "node_modules/@types/estree": {
      "version": "1.0.9",
      "resolved": "https://registry.npmjs.org/@types/estree/-/estree-1.0.9.tgz",
      "integrity": "sha512-GhdPgy1el4/ImP05X05Uw4cw2/M93BCUmnEvWZNStlCzEKME4Fkk+YpoA5OiHNQmoS7Cafb8Xa3Pya8m1Qrzeg==",
      "license": "MIT"
    },
    "node_modules/@types/estree-jsx": {
      "version": "1.0.5",
      "resolved": "https://registry.npmjs.org/@types/estree-jsx/-/estree-jsx-1.0.5.tgz",
      "integrity": "sha512-52CcUVNFyfb1A2ALocQw/Dd1BQFNmSdkuC3BkZ6iqhdMfQz7JWOFRuJFloOzjk+6WijU56m9oKXFAXc7o3Towg==",
      "license": "MIT",
      "dependencies": {
        "@types/estree": "*"
      }
    },
    "node_modules/@types/hast": {
      "version": "3.0.4",
      "resolved": "https://registry.npmjs.org/@types/hast/-/hast-3.0.4.tgz",
      "integrity": "sha512-WPs+bbQw5aCj+x6laNGWLH3wviHtoCv/P3+otBhbOhJgG8qtpdAMlTCxLtsTWA7LH1Oh/bFCHsBn0TPS5m30EQ==",
      "license": "MIT",
      "dependencies": {
        "@types/unist": "*"
      }
    },
    "node_modules/@types/json-schema": {
      "version": "7.0.15",
      "resolved": "https://registry.npmjs.org/@types/json-schema/-/json-schema-7.0.15.tgz",
      "integrity": "sha512-5+fP8P8MFNC+AyZCDxrB2pkZFPGzqQWUzpSeuuVLvm8VMcorNYavBqoFcxK8bQz4Qsbn4oUEEem4wDLfcysGHA==",
      "dev": true,
      "license": "MIT"
    },
    "node_modules/@types/mdast": {
      "version": "4.0.4",
      "resolved": "https://registry.npmjs.org/@types/mdast/-/mdast-4.0.4.tgz",
      "integrity": "sha512-kGaNbPh1k7AFzgpud/gMdvIm5xuECykRR+JnWKQno9TAXVa6WIVCGTPvYGekIDL4uwCZQSYbUxNBSb1aUo79oA==",
      "license": "MIT",
      "dependencies": {
        "@types/unist": "*"
      }
    },
    "node_modules/@types/ms": {
      "version": "2.1.0",
      "resolved": "https://registry.npmjs.org/@types/ms/-/ms-2.1.0.tgz",
      "integrity": "sha512-GsCCIZDE/p3i96vtEqx+7dBUGXrc7zeSK3wwPHIaRThS+9OhWIXRqzs4d6k1SVU8g91DrNRWxWUGhp5KXQb2VA==",
      "license": "MIT"
    },
    "node_modules/@types/node": {
      "version": "22.19.11",
      "resolved": "https://registry.npmjs.org/@types/node/-/node-22.19.11.tgz",
      "integrity": "sha512-BH7YwL6rA93ReqeQS1c4bsPpcfOmJasG+Fkr6Y59q83f9M1WcBRHR2vM+P9eOisYRcN3ujQoiZY8uk5W+1WL8w==",
      "dev": true,
      "license": "MIT",
      "dependencies": {
        "undici-types": "~6.21.0"
      }
    },
    "node_modules/@types/pako": {
      "version": "2.0.4",
      "resolved": "https://registry.npmjs.org/@types/pako/-/pako-2.0.4.tgz",
      "integrity": "sha512-VWDCbrLeVXJM9fihYodcLiIv0ku+AlOa/TQ1SvYOaBuyrSKgEcro95LJyIsJ4vSo6BXIxOKxiJAat04CmST9Fw==",
      "license": "MIT"
    },
    "node_modules/@types/prop-types": {
      "version": "15.7.15",
      "resolved": "https://registry.npmjs.org/@types/prop-types/-/prop-types-15.7.15.tgz",
      "integrity": "sha512-F6bEyamV9jKGAFBEmlQnesRPGOQqS2+Uwi0Em15xenOxHaf2hv6L8YCVn3rPdPJOiJfPiCnLIRyvwVaqMY3MIw==",
      "license": "MIT"
    },
    "node_modules/@types/quill": {
      "version": "1.3.10",
      "resolved": "https://registry.npmjs.org/@types/quill/-/quill-1.3.10.tgz",
      "integrity": "sha512-IhW3fPW+bkt9MLNlycw8u8fWb7oO7W5URC9MfZYHBlA24rex9rs23D5DETChu1zvgVdc5ka64ICjJOgQMr6Shw==",
      "license": "MIT",
      "dependencies": {
        "parchment": "^1.1.2"
      }
    },
    "node_modules/@types/raf": {
      "version": "3.4.3",
      "resolved": "https://registry.npmjs.org/@types/raf/-/raf-3.4.3.tgz",
      "integrity": "sha512-c4YAvMedbPZ5tEyxzQdMoOhhJ4RD3rngZIdwC2/qDN3d7JpEhB6fiBRKVY1lg5B7Wk+uPBjn5f39j1/2MY1oOw==",
      "license": "MIT",
      "optional": true
    },
    "node_modules/@types/react": {
      "version": "18.3.28",
      "resolved": "https://registry.npmjs.org/@types/react/-/react-18.3.28.tgz",
      "integrity": "sha512-z9VXpC7MWrhfWipitjNdgCauoMLRdIILQsAEV+ZesIzBq/oUlxk0m3ApZuMFCXdnS4U7KrI+l3WRUEGQ8K1QKw==",
      "license": "MIT",
      "dependencies": {
        "@types/prop-types": "*",
        "csstype": "^3.2.2"
      }
    },
    "node_modules/@types/react-dom": {
      "version": "18.3.7",
      "resolved": "https://registry.npmjs.org/@types/react-dom/-/react-dom-18.3.7.tgz",
      "integrity": "sha512-MEe3UeoENYVFXzoXEWsvcpg6ZvlrFNlOQ7EOsvhI3CfAXwzPfO8Qwuxd40nepsYKqyyVQnTdEfv68q91yLcKrQ==",
      "devOptional": true,
      "license": "MIT",
      "peerDependencies": {
        "@types/react": "^18.0.0"
      }
    },
    "node_modules/@types/trusted-types": {
      "version": "2.0.7",
      "resolved": "https://registry.npmjs.org/@types/trusted-types/-/trusted-types-2.0.7.tgz",
      "integrity": "sha512-ScaPdn1dQczgbl0QFTeTOmVHFULt394XJgOQNoyVhZ6r2vLnMLJfBPd53SB52T/3G36VI1/g2MZaX0cwDuXsfw==",
      "license": "MIT",
      "optional": true
    },
    "node_modules/@types/unist": {
      "version": "3.0.3",
      "resolved": "https://registry.npmjs.org/@types/unist/-/unist-3.0.3.tgz",
      "integrity": "sha512-ko/gIFJRv177XgZsZcBwnqJN5x/Gien8qNOn0D5bQU/zAzVf9Zt3BlcUiLqhV9y4ARk0GbT3tnUiPNgnTXzc/Q==",
      "license": "MIT"
    },
    "node_modules/@types/use-sync-external-store": {
      "version": "0.0.6",
      "resolved": "https://registry.npmjs.org/@types/use-sync-external-store/-/use-sync-external-store-0.0.6.tgz",
      "integrity": "sha512-zFDAD+tlpf2r4asuHEj0XH6pY6i0g5NeAHPn+15wk3BV6JA69eERFXC1gyGThDkVa1zCyKr5jox1+2LbV/AMLg==",
      "license": "MIT"
    },
    "node_modules/@ungap/structured-clone": {
      "version": "1.3.0",
      "resolved": "https://registry.npmjs.org/@ungap/structured-clone/-/structured-clone-1.3.0.tgz",
      "integrity": "sha512-WmoN8qaIAo7WTYWbAZuG8PYEhn5fkz7dZrqTBZ7dtt//lL2Gwms1IcnQ5yHqjDfX8Ft5j4YzDM23f87zBfDe9g==",
      "license": "ISC"
    },
    "node_modules/@vitejs/plugin-react": {
      "version": "4.7.0",
      "resolved": "https://registry.npmjs.org/@vitejs/plugin-react/-/plugin-react-4.7.0.tgz",
      "integrity": "sha512-gUu9hwfWvvEDBBmgtAowQCojwZmJ5mcLn3aufeCsitijs3+f2NsrPtlAWIR6OPiqljl96GVCUbLe0HyqIpVaoA==",
      "dev": true,
      "license": "MIT",
      "dependencies": {
        "@babel/core": "^7.28.0",
        "@babel/plugin-transform-react-jsx-self": "^7.27.1",
        "@babel/plugin-transform-react-jsx-source": "^7.27.1",
        "@rolldown/pluginutils": "1.0.0-beta.27",
        "@types/babel__core": "^7.20.5",
        "react-refresh": "^0.17.0"
      },
      "engines": {
        "node": "^14.18.0 || >=16.0.0"
      },
      "peerDependencies": {
        "vite": "^4.2.0 || ^5.0.0 || ^6.0.0 || ^7.0.0"
      }
    },
    "node_modules/acorn": {
      "version": "8.15.0",
      "resolved": "https://registry.npmjs.org/acorn/-/acorn-8.15.0.tgz",
      "integrity": "sha512-NZyJarBfL7nWwIq+FDL6Zp/yHEhePMNnnJ0y3qfieCrmNvYct8uvtiV41UvlSe6apAfk0fY1FbWx+NwfmpvtTg==",
      "dev": true,
      "license": "MIT",
      "bin": {
        "acorn": "bin/acorn"
      },
      "engines": {
        "node": ">=0.4.0"
      }
    },
    "node_modules/acorn-jsx": {
      "version": "5.3.2",
      "resolved": "https://registry.npmjs.org/acorn-jsx/-/acorn-jsx-5.3.2.tgz",
      "integrity": "sha512-rq9s+JNhf0IChjtDXxllJ7g41oZk5SlXtp0LHwyA5cejwn7vKmKp4pPri6YEePv2PU65sAsegbXtIinmDFDXgQ==",
      "dev": true,
      "license": "MIT",
      "peerDependencies": {
        "acorn": "^6.0.0 || ^7.0.0 || ^8.0.0"
      }
    },
    "node_modules/agent-base": {
      "version": "6.0.2",
      "resolved": "https://registry.npmjs.org/agent-base/-/agent-base-6.0.2.tgz",
      "integrity": "sha512-RZNwNclF7+MS/8bDg70amg32dyeZGZxiDuQmZxKLAlQjr3jGyLx+4Kkk58UO7D2QdgFIQCovuSuZESne6RG6XQ==",
      "license": "MIT",
      "dependencies": {
        "debug": "4"
      },
      "engines": {
        "node": ">= 6.0.0"
      }
    },
    "node_modules/ajv": {
      "version": "6.15.0",
      "resolved": "https://registry.npmjs.org/ajv/-/ajv-6.15.0.tgz",
      "integrity": "sha512-fgFx7Hfoq60ytK2c7DhnF8jIvzYgOMxfugjLOSMHjLIPgenqa7S7oaagATUq99mV6IYvN2tRmC0wnTYX6iPbMw==",
      "dev": true,
      "license": "MIT",
      "dependencies": {
        "fast-deep-equal": "^3.1.1",
        "fast-json-stable-stringify": "^2.0.0",
        "json-schema-traverse": "^0.4.1",
        "uri-js": "^4.2.2"
      },
      "funding": {
        "type": "github",
        "url": "https://github.com/sponsors/epoberezkin"
      }
    },
    "node_modules/ansi-styles": {
      "version": "4.3.0",
      "resolved": "https://registry.npmjs.org/ansi-styles/-/ansi-styles-4.3.0.tgz",
      "integrity": "sha512-zbB9rCJAT1rbjiVDb2hqKFHNYLxgtk8NURxZ3IZwD3F6NtxbXZQCnnSi1Lkx+IDohdPlFp222wVALIheZJQSEg==",
      "dev": true,
      "license": "MIT",
      "dependencies": {
        "color-convert": "^2.0.1"
      },
      "engines": {
        "node": ">=8"
      },
      "funding": {
        "url": "https://github.com/chalk/ansi-styles?sponsor=1"
      }
    },
    "node_modules/any-promise": {
      "version": "1.3.0",
      "resolved": "https://registry.npmjs.org/any-promise/-/any-promise-1.3.0.tgz",
      "integrity": "sha512-7UvmKalWRt1wgjL1RrGxoSJW/0QZFIegpeGvZG9kjp8vrRu55XTHbwnqq2GpXm9uLbcuhxm3IqX9OB4MZR1b2A==",
      "license": "MIT"
    },
    "node_modules/anymatch": {
      "version": "3.1.3",
      "resolved": "https://registry.npmjs.org/anymatch/-/anymatch-3.1.3.tgz",
      "integrity": "sha512-KMReFUr0B4t+D+OBkjR3KYqvocp2XaSzO55UcB6mgQMd3KbcE+mWTyvVV7D/zsdEbNnV6acZUutkiHQXvTr1Rw==",
      "license": "ISC",
      "dependencies": {
        "normalize-path": "^3.0.0",
        "picomatch": "^2.0.4"
      },
      "engines": {
        "node": ">= 8"
      }
    },
    "node_modules/arg": {
      "version": "5.0.2",
      "resolved": "https://registry.npmjs.org/arg/-/arg-5.0.2.tgz",
      "integrity": "sha512-PYjyFOLKQ9y57JvQ6QLo8dAgNqswh8M1RMJYdQduT6xbWSgK36P/Z/v+p888pM69jMMfS8Xd8F6I1kQ/I9HUGg==",
      "license": "MIT"
    },
    "node_modules/argparse": {
      "version": "2.0.1",
      "resolved": "https://registry.npmjs.org/argparse/-/argparse-2.0.1.tgz",
      "integrity": "sha512-8+9WqebbFzpX9OR+Wa6O29asIogeRMzcGtAINdpMHHyAg10f05aSFVBbcEqGf/PXw1EjAZ+q2/bEBg3DvurK3Q==",
      "dev": true,
      "license": "Python-2.0"
    },
    "node_modules/aria-hidden": {
      "version": "1.2.6",
      "resolved": "https://registry.npmjs.org/aria-hidden/-/aria-hidden-1.2.6.tgz",
      "integrity": "sha512-ik3ZgC9dY/lYVVM++OISsaYDeg1tb0VtP5uL3ouh1koGOaUMDPpbFIei4JkFimWUFPn90sbMNMXQAIVOlnYKJA==",
      "license": "MIT",
      "dependencies": {
        "tslib": "^2.0.0"
      },
      "engines": {
        "node": ">=10"
      }
    },
    "node_modules/array-buffer-byte-length": {
      "version": "1.0.2",
      "resolved": "https://registry.npmjs.org/array-buffer-byte-length/-/array-buffer-byte-length-1.0.2.tgz",
      "integrity": "sha512-LHE+8BuR7RYGDKvnrmcuSq3tDcKv9OFEXQt/HpbZhY7V6h0zlUXutnAD82GiFx9rdieCMjkvtcsPqBwgUl1Iiw==",
      "dev": true,
      "license": "MIT",
      "dependencies": {
        "call-bound": "^1.0.3",
        "is-array-buffer": "^3.0.5"
      },
      "engines": {
        "node": ">= 0.4"
      },
      "funding": {
        "url": "https://github.com/sponsors/ljharb"
      }
    },
    "node_modules/array-includes": {
      "version": "3.1.9",
      "resolved": "https://registry.npmjs.org/array-includes/-/array-includes-3.1.9.tgz",
      "integrity": "sha512-FmeCCAenzH0KH381SPT5FZmiA/TmpndpcaShhfgEN9eCVjnFBqq3l1xrI42y8+PPLI6hypzou4GXw00WHmPBLQ==",
      "dev": true,
      "license": "MIT",
      "dependencies": {
        "call-bind": "^1.0.8",
        "call-bound": "^1.0.4",
        "define-properties": "^1.2.1",
        "es-abstract": "^1.24.0",
        "es-object-atoms": "^1.1.1",
        "get-intrinsic": "^1.3.0",
        "is-string": "^1.1.1",
        "math-intrinsics": "^1.1.0"
      },
      "engines": {
        "node": ">= 0.4"
      },
      "funding": {
        "url": "https://github.com/sponsors/ljharb"
      }
    },
    "node_modules/array.prototype.findlast": {
      "version": "1.2.5",
      "resolved": "https://registry.npmjs.org/array.prototype.findlast/-/array.prototype.findlast-1.2.5.tgz",
      "integrity": "sha512-CVvd6FHg1Z3POpBLxO6E6zr+rSKEQ9L6rZHAaY7lLfhKsWYUBBOuMs0e9o24oopj6H+geRCX0YJ+TJLBK2eHyQ==",
      "dev": true,
      "license": "MIT",
      "dependencies": {
        "call-bind": "^1.0.7",
        "define-properties": "^1.2.1",
        "es-abstract": "^1.23.2",
        "es-errors": "^1.3.0",
        "es-object-atoms": "^1.0.0",
        "es-shim-unscopables": "^1.0.2"
      },
      "engines": {
        "node": ">= 0.4"
      },
      "funding": {
        "url": "https://github.com/sponsors/ljharb"
      }
    },
    "node_modules/array.prototype.flat": {
      "version": "1.3.3",
      "resolved": "https://registry.npmjs.org/array.prototype.flat/-/array.prototype.flat-1.3.3.tgz",
      "integrity": "sha512-rwG/ja1neyLqCuGZ5YYrznA62D4mZXg0i1cIskIUKSiqF3Cje9/wXAls9B9s1Wa2fomMsIv8czB8jZcPmxCXFg==",
      "dev": true,
      "license": "MIT",
      "dependencies": {
        "call-bind": "^1.0.8",
        "define-properties": "^1.2.1",
        "es-abstract": "^1.23.5",
        "es-shim-unscopables": "^1.0.2"
      },
      "engines": {
        "node": ">= 0.4"
      },
      "funding": {
        "url": "https://github.com/sponsors/ljharb"
      }
    },
    "node_modules/array.prototype.flatmap": {
      "version": "1.3.3",
      "resolved": "https://registry.npmjs.org/array.prototype.flatmap/-/array.prototype.flatmap-1.3.3.tgz",
      "integrity": "sha512-Y7Wt51eKJSyi80hFrJCePGGNo5ktJCslFuboqJsbf57CCPcm5zztluPlc4/aD8sWsKvlwatezpV4U1efk8kpjg==",
      "dev": true,
      "license": "MIT",
      "dependencies": {
        "call-bind": "^1.0.8",
        "define-properties": "^1.2.1",
        "es-abstract": "^1.23.5",
        "es-shim-unscopables": "^1.0.2"
      },
      "engines": {
        "node": ">= 0.4"
      },
      "funding": {
        "url": "https://github.com/sponsors/ljharb"
      }
    },
    "node_modules/array.prototype.tosorted": {
      "version": "1.1.4",
      "resolved": "https://registry.npmjs.org/array.prototype.tosorted/-/array.prototype.tosorted-1.1.4.tgz",
      "integrity": "sha512-p6Fx8B7b7ZhL/gmUsAy0D15WhvDccw3mnGNbZpi3pmeJdxtWsj2jEaI4Y6oo3XiHfzuSgPwKc04MYt6KgvC/wA==",
      "dev": true,
      "license": "MIT",
      "dependencies": {
        "call-bind": "^1.0.7",
        "define-properties": "^1.2.1",
        "es-abstract": "^1.23.3",
        "es-errors": "^1.3.0",
        "es-shim-unscopables": "^1.0.2"
      },
      "engines": {
        "node": ">= 0.4"
      }
    },
    "node_modules/arraybuffer.prototype.slice": {
      "version": "1.0.4",
      "resolved": "https://registry.npmjs.org/arraybuffer.prototype.slice/-/arraybuffer.prototype.slice-1.0.4.tgz",
      "integrity": "sha512-BNoCY6SXXPQ7gF2opIP4GBE+Xw7U+pHMYKuzjgCN3GwiaIR09UUeKfheyIry77QtrCBlC0KK0q5/TER/tYh3PQ==",
      "dev": true,
      "license": "MIT",
      "dependencies": {
        "array-buffer-byte-length": "^1.0.1",
        "call-bind": "^1.0.8",
        "define-properties": "^1.2.1",
        "es-abstract": "^1.23.5",
        "es-errors": "^1.3.0",
        "get-intrinsic": "^1.2.6",
        "is-array-buffer": "^3.0.4"
      },
      "engines": {
        "node": ">= 0.4"
      },
      "funding": {
        "url": "https://github.com/sponsors/ljharb"
      }
    },
    "node_modules/async-function": {
      "version": "1.0.0",
      "resolved": "https://registry.npmjs.org/async-function/-/async-function-1.0.0.tgz",
      "integrity": "sha512-hsU18Ae8CDTR6Kgu9DYf0EbCr/a5iGL0rytQDobUcdpYOKokk8LEjVphnXkDkgpi0wYVsqrXuP0bZxJaTqdgoA==",
      "dev": true,
      "license": "MIT",
      "engines": {
        "node": ">= 0.4"
      }
    },
    "node_modules/asynckit": {
      "version": "0.4.0",
      "resolved": "https://registry.npmjs.org/asynckit/-/asynckit-0.4.0.tgz",
      "integrity": "sha512-Oei9OH4tRh0YqU3GxhX79dM/mwVgvbZJaSNaRk+bshkj0S5cfHcgYakreBjrHwatXKbz+IoIdYLxrKim2MjW0Q==",
      "license": "MIT"
    },
    "node_modules/autoprefixer": {
      "version": "10.4.24",
      "resolved": "https://registry.npmjs.org/autoprefixer/-/autoprefixer-10.4.24.tgz",
      "integrity": "sha512-uHZg7N9ULTVbutaIsDRoUkoS8/h3bdsmVJYZ5l3wv8Cp/6UIIoRDm90hZ+BwxUj/hGBEzLxdHNSKuFpn8WOyZw==",
      "dev": true,
      "funding": [
        {
          "type": "opencollective",
          "url": "https://opencollective.com/postcss/"
        },
        {
          "type": "tidelift",
          "url": "https://tidelift.com/funding/github/npm/autoprefixer"
        },
        {
          "type": "github",
          "url": "https://github.com/sponsors/ai"
        }
      ],
      "license": "MIT",
      "dependencies": {
        "browserslist": "^4.28.1",
        "caniuse-lite": "^1.0.30001766",
        "fraction.js": "^5.3.4",
        "picocolors": "^1.1.1",
        "postcss-value-parser": "^4.2.0"
      },
      "bin": {
        "autoprefixer": "bin/autoprefixer"
      },
      "engines": {
        "node": "^10 || ^12 || >=14"
      },
      "peerDependencies": {
        "postcss": "^8.1.0"
      }
    },
    "node_modules/available-typed-arrays": {
      "version": "1.0.7",
      "resolved": "https://registry.npmjs.org/available-typed-arrays/-/available-typed-arrays-1.0.7.tgz",
      "integrity": "sha512-wvUjBtSGN7+7SjNpq/9M2Tg350UZD3q62IFZLbRAR1bSMlCo1ZaeW+BJ+D090e4hIIZLBcTDWe4Mh4jvUDajzQ==",
      "dev": true,
      "license": "MIT",
      "dependencies": {
        "possible-typed-array-names": "^1.0.0"
      },
      "engines": {
        "node": ">= 0.4"
      },
      "funding": {
        "url": "https://github.com/sponsors/ljharb"
      }
    },
    "node_modules/axios": {
      "version": "1.18.1",
      "resolved": "https://registry.npmjs.org/axios/-/axios-1.18.1.tgz",
      "integrity": "sha512-3nTvFlvpn9Zu/RkHUqtc7/+al4UpRW5az71ap5zccp6e8RAYEzhMTecX8Dz1wWDYrPpUoB1HAQEGEAEvUr7S9g==",
      "license": "MIT",
      "dependencies": {
        "follow-redirects": "^1.16.0",
        "form-data": "^4.0.5",
        "https-proxy-agent": "^5.0.1",
        "proxy-from-env": "^2.1.0"
      }
    },
    "node_modules/bail": {
      "version": "2.0.2",
      "resolved": "https://registry.npmjs.org/bail/-/bail-2.0.2.tgz",
      "integrity": "sha512-0xO6mYd7JB2YesxDKplafRpsiOzPt9V02ddPCLbY1xYGPOX24NTyN50qnUxgCPcSoYMhKpAuBTjQoRZCAkUDRw==",
      "license": "MIT",
      "funding": {
        "type": "github",
        "url": "https://github.com/sponsors/wooorm"
      }
    },
    "node_modules/balanced-match": {
      "version": "1.0.2",
      "resolved": "https://registry.npmjs.org/balanced-match/-/balanced-match-1.0.2.tgz",
      "integrity": "sha512-3oSeUO0TMV67hN1AmbXsK4yaqU7tjiHlbxRDZOpH0KW9+CeX4bRAaX0Anxt0tx2MrpRpWwQaPwIlISEJhYU5Pw==",
      "dev": true,
      "license": "MIT"
    },
    "node_modules/base64-arraybuffer": {
      "version": "1.0.2",
      "resolved": "https://registry.npmjs.org/base64-arraybuffer/-/base64-arraybuffer-1.0.2.tgz",
      "integrity": "sha512-I3yl4r9QB5ZRY3XuJVEPfc2XhZO6YweFPI+UovAzn+8/hb3oJ6lnysaFcjVpkCPfVWFUDvoZ8kmVDP7WyRtYtQ==",
      "license": "MIT",
      "engines": {
        "node": ">= 0.6.0"
      }
    },
    "node_modules/baseline-browser-mapping": {
      "version": "2.9.19",
      "resolved": "https://registry.npmjs.org/baseline-browser-mapping/-/baseline-browser-mapping-2.9.19.tgz",
      "integrity": "sha512-ipDqC8FrAl/76p2SSWKSI+H9tFwm7vYqXQrItCuiVPt26Km0jS+NzSsBWAaBusvSbQcfJG+JitdMm+wZAgTYqg==",
      "dev": true,
      "license": "Apache-2.0",
      "bin": {
        "baseline-browser-mapping": "dist/cli.js"
      }
    },
    "node_modules/binary-extensions": {
      "version": "2.3.0",
      "resolved": "https://registry.npmjs.org/binary-extensions/-/binary-extensions-2.3.0.tgz",
      "integrity": "sha512-Ceh+7ox5qe7LJuLHoY0feh3pHuUDHAcRUeyL2VYghZwfpkNIy/+8Ocg0a3UuSoYzavmylwuLWQOf3hl0jjMMIw==",
      "license": "MIT",
      "engines": {
        "node": ">=8"
      },
      "funding": {
        "url": "https://github.com/sponsors/sindresorhus"
      }
    },
    "node_modules/brace-expansion": {
      "version": "1.1.15",
      "resolved": "https://registry.npmjs.org/brace-expansion/-/brace-expansion-1.1.15.tgz",
      "integrity": "sha512-EwOCDEex4quD37XhqM3omwtMoJjr//isUZz1JopUNWms+4Z2ViyM/k1YIRePpoVNnQhENnxtFjLaxNHrT7xIUg==",
      "dev": true,
      "license": "MIT",
      "dependencies": {
        "balanced-match": "^1.0.0",
        "concat-map": "0.0.1"
      }
    },
    "node_modules/braces": {
      "version": "3.0.3",
      "resolved": "https://registry.npmjs.org/braces/-/braces-3.0.3.tgz",
      "integrity": "sha512-yQbXgO/OSZVD2IsiLlro+7Hf6Q18EJrKSEsdoMzKePKXct3gvD8oLcOQdIzGupr5Fj+EDe8gO/lxc1BzfMpxvA==",
      "license": "MIT",
      "dependencies": {
        "fill-range": "^7.1.1"
      },
      "engines": {
        "node": ">=8"
      }
    },
    "node_modules/browserslist": {
      "version": "4.28.1",
      "resolved": "https://registry.npmjs.org/browserslist/-/browserslist-4.28.1.tgz",
      "integrity": "sha512-ZC5Bd0LgJXgwGqUknZY/vkUQ04r8NXnJZ3yYi4vDmSiZmC/pdSN0NbNRPxZpbtO4uAfDUAFffO8IZoM3Gj8IkA==",
      "dev": true,
      "funding": [
        {
          "type": "opencollective",
          "url": "https://opencollective.com/browserslist"
        },
        {
          "type": "tidelift",
          "url": "https://tidelift.com/funding/github/npm/browserslist"
        },
        {
          "type": "github",
          "url": "https://github.com/sponsors/ai"
        }
      ],
      "license": "MIT",
      "dependencies": {
        "baseline-browser-mapping": "^2.9.0",
        "caniuse-lite": "^1.0.30001759",
        "electron-to-chromium": "^1.5.263",
        "node-releases": "^2.0.27",
        "update-browserslist-db": "^1.2.0"
      },
      "bin": {
        "browserslist": "cli.js"
      },
      "engines": {
        "node": "^6 || ^7 || ^8 || ^9 || ^10 || ^11 || ^12 || >=13.7"
      }
    },
    "node_modules/call-bind": {
      "version": "1.0.8",
      "resolved": "https://registry.npmjs.org/call-bind/-/call-bind-1.0.8.tgz",
      "integrity": "sha512-oKlSFMcMwpUg2ednkhQ454wfWiU/ul3CkJe/PEHcTKuiX6RpbehUiFMXu13HalGZxfUwCQzZG747YXBn1im9ww==",
      "license": "MIT",
      "dependencies": {
        "call-bind-apply-helpers": "^1.0.0",
        "es-define-property": "^1.0.0",
        "get-intrinsic": "^1.2.4",
        "set-function-length": "^1.2.2"
      },
      "engines": {
        "node": ">= 0.4"
      },
      "funding": {
        "url": "https://github.com/sponsors/ljharb"
      }
    },
    "node_modules/call-bind-apply-helpers": {
      "version": "1.0.2",
      "resolved": "https://registry.npmjs.org/call-bind-apply-helpers/-/call-bind-apply-helpers-1.0.2.tgz",
      "integrity": "sha512-Sp1ablJ0ivDkSzjcaJdxEunN5/XvksFJ2sMBFfq6x0ryhQV/2b/KwFe21cMpmHtPOSij8K99/wSfoEuTObmuMQ==",
      "license": "MIT",
      "dependencies": {
        "es-errors": "^1.3.0",
        "function-bind": "^1.1.2"
      },
      "engines": {
        "node": ">= 0.4"
      }
    },
    "node_modules/call-bound": {
      "version": "1.0.4",
      "resolved": "https://registry.npmjs.org/call-bound/-/call-bound-1.0.4.tgz",
      "integrity": "sha512-+ys997U96po4Kx/ABpBCqhA9EuxJaQWDQg7295H4hBphv3IZg0boBKuwYpt4YXp6MZ5AmZQnU/tyMTlRpaSejg==",
      "license": "MIT",
      "dependencies": {
        "call-bind-apply-helpers": "^1.0.2",
        "get-intrinsic": "^1.3.0"
      },
      "engines": {
        "node": ">= 0.4"
      },
      "funding": {
        "url": "https://github.com/sponsors/ljharb"
      }
    },
    "node_modules/callsites": {
      "version": "3.1.0",
      "resolved": "https://registry.npmjs.org/callsites/-/callsites-3.1.0.tgz",
      "integrity": "sha512-P8BjAsXvZS+VIDUI11hHCQEv74YT67YUi5JJFNWIqL235sBmjX4+qx9Muvls5ivyNENctx46xQLQ3aTuE7ssaQ==",
      "dev": true,
      "license": "MIT",
      "engines": {
        "node": ">=6"
      }
    },
    "node_modules/camelcase-css": {
      "version": "2.0.1",
      "resolved": "https://registry.npmjs.org/camelcase-css/-/camelcase-css-2.0.1.tgz",
      "integrity": "sha512-QOSvevhslijgYwRx6Rv7zKdMF8lbRmx+uQGx2+vDc+KI/eBnsy9kit5aj23AgGu3pa4t9AgwbnXWqS+iOY+2aA==",
      "license": "MIT",
      "engines": {
        "node": ">= 6"
      }
    },
    "node_modules/caniuse-lite": {
      "version": "1.0.30001770",
      "resolved": "https://registry.npmjs.org/caniuse-lite/-/caniuse-lite-1.0.30001770.tgz",
      "integrity": "sha512-x/2CLQ1jHENRbHg5PSId2sXq1CIO1CISvwWAj027ltMVG2UNgW+w9oH2+HzgEIRFembL8bUlXtfbBHR1fCg2xw==",
      "dev": true,
      "funding": [
        {
          "type": "opencollective",
          "url": "https://opencollective.com/browserslist"
        },
        {
          "type": "tidelift",
          "url": "https://tidelift.com/funding/github/npm/caniuse-lite"
        },
        {
          "type": "github",
          "url": "https://github.com/sponsors/ai"
        }
      ],
      "license": "CC-BY-4.0"
    },
    "node_modules/canvas-confetti": {
      "version": "1.9.4",
      "resolved": "https://registry.npmjs.org/canvas-confetti/-/canvas-confetti-1.9.4.tgz",
      "integrity": "sha512-yxQbJkAVrFXWNbTUjPqjF7G+g6pDotOUHGbkZq2NELZUMDpiJ85rIEazVb8GTaAptNW2miJAXbs1BtioA251Pw==",
      "license": "ISC",
      "funding": {
        "type": "donate",
        "url": "https://www.paypal.me/kirilvatev"
      }
    },
    "node_modules/canvg": {
      "version": "3.0.11",
      "resolved": "https://registry.npmjs.org/canvg/-/canvg-3.0.11.tgz",
      "integrity": "sha512-5ON+q7jCTgMp9cjpu4Jo6XbvfYwSB2Ow3kzHKfIyJfaCAOHLbdKPQqGKgfED/R5B+3TFFfe8pegYA+b423SRyA==",
      "license": "MIT",
      "optional": true,
      "dependencies": {
        "@babel/runtime": "^7.12.5",
        "@types/raf": "^3.4.0",
        "core-js": "^3.8.3",
        "raf": "^3.4.1",
        "regenerator-runtime": "^0.13.7",
        "rgbcolor": "^1.0.1",
        "stackblur-canvas": "^2.0.0",
        "svg-pathdata": "^6.0.3"
      },
      "engines": {
        "node": ">=10.0.0"
      }
    },
    "node_modules/ccount": {
      "version": "2.0.1",
      "resolved": "https://registry.npmjs.org/ccount/-/ccount-2.0.1.tgz",
      "integrity": "sha512-eyrF0jiFpY+3drT6383f1qhkbGsLSifNAjA61IUjZjmLCWjItY6LB9ft9YhoDgwfmclB2zhu51Lc7+95b8NRAg==",
      "license": "MIT",
      "funding": {
        "type": "github",
        "url": "https://github.com/sponsors/wooorm"
      }
    },
    "node_modules/chalk": {
      "version": "4.1.2",
      "resolved": "https://registry.npmjs.org/chalk/-/chalk-4.1.2.tgz",
      "integrity": "sha512-oKnbhFyRIXpUuez8iBMmyEa4nbj4IOQyuhc/wy9kY7/WVPcwIO9VA668Pu8RkO7+0G76SLROeyw9CpQ061i4mA==",
      "dev": true,
      "license": "MIT",
      "dependencies": {
        "ansi-styles": "^4.1.0",
        "supports-color": "^7.1.0"
      },
      "engines": {
        "node": ">=10"
      },
      "funding": {
        "url": "https://github.com/chalk/chalk?sponsor=1"
      }
    },
    "node_modules/character-entities": {
      "version": "2.0.2",
      "resolved": "https://registry.npmjs.org/character-entities/-/character-entities-2.0.2.tgz",
      "integrity": "sha512-shx7oQ0Awen/BRIdkjkvz54PnEEI/EjwXDSIZp86/KKdbafHh1Df/RYGBhn4hbe2+uKC9FnT5UCEdyPz3ai9hQ==",
      "license": "MIT",
      "funding": {
        "type": "github",
        "url": "https://github.com/sponsors/wooorm"
      }
    },
    "node_modules/character-entities-html4": {
      "version": "2.1.0",
      "resolved": "https://registry.npmjs.org/character-entities-html4/-/character-entities-html4-2.1.0.tgz",
      "integrity": "sha512-1v7fgQRj6hnSwFpq1Eu0ynr/CDEw0rXo2B61qXrLNdHZmPKgb7fqS1a2JwF0rISo9q77jDI8VMEHoApn8qDoZA==",
      "license": "MIT",
      "funding": {
        "type": "github",
        "url": "https://github.com/sponsors/wooorm"
      }
    },
    "node_modules/character-entities-legacy": {
      "version": "3.0.0",
      "resolved": "https://registry.npmjs.org/character-entities-legacy/-/character-entities-legacy-3.0.0.tgz",
      "integrity": "sha512-RpPp0asT/6ufRm//AJVwpViZbGM/MkjQFxJccQRHmISF/22NBtsHqAWmL+/pmkPWoIUJdWyeVleTl1wydHATVQ==",
      "license": "MIT",
      "funding": {
        "type": "github",
        "url": "https://github.com/sponsors/wooorm"
      }
    },
    "node_modules/character-reference-invalid": {
      "version": "2.0.1",
      "resolved": "https://registry.npmjs.org/character-reference-invalid/-/character-reference-invalid-2.0.1.tgz",
      "integrity": "sha512-iBZ4F4wRbyORVsu0jPV7gXkOsGYjGHPmAyv+HiHG8gi5PtC9KI2j1+v8/tlibRvjoWX027ypmG/n0HtO5t7unw==",
      "license": "MIT",
      "funding": {
        "type": "github",
        "url": "https://github.com/sponsors/wooorm"
      }
    },
    "node_modules/chokidar": {
      "version": "3.6.0",
      "resolved": "https://registry.npmjs.org/chokidar/-/chokidar-3.6.0.tgz",
      "integrity": "sha512-7VT13fmjotKpGipCW9JEQAusEPE+Ei8nl6/g4FBAmIm0GOOLMua9NDDo/DWp0ZAxCr3cPq5ZpBqmPAQgDda2Pw==",
      "license": "MIT",
      "dependencies": {
        "anymatch": "~3.1.2",
        "braces": "~3.0.2",
        "glob-parent": "~5.1.2",
        "is-binary-path": "~2.1.0",
        "is-glob": "~4.0.1",
        "normalize-path": "~3.0.0",
        "readdirp": "~3.6.0"
      },
      "engines": {
        "node": ">= 8.10.0"
      },
      "funding": {
        "url": "https://paulmillr.com/funding/"
      },
      "optionalDependencies": {
        "fsevents": "~2.3.2"
      }
    },
    "node_modules/chokidar/node_modules/glob-parent": {
      "version": "5.1.2",
      "resolved": "https://registry.npmjs.org/glob-parent/-/glob-parent-5.1.2.tgz",
      "integrity": "sha512-AOIgSQCepiJYwP3ARnGx+5VnTu2HBYdzbGP45eLw1vr3zB3vZLeyed1sC9hnbcOc9/SrMyM5RPQrkGz4aS9Zow==",
      "license": "ISC",
      "dependencies": {
        "is-glob": "^4.0.1"
      },
      "engines": {
        "node": ">= 6"
      }
    },
    "node_modules/class-variance-authority": {
      "version": "0.7.1",
      "resolved": "https://registry.npmjs.org/class-variance-authority/-/class-variance-authority-0.7.1.tgz",
      "integrity": "sha512-Ka+9Trutv7G8M6WT6SeiRWz792K5qEqIGEGzXKhAE6xOWAY6pPH8U+9IY3oCMv6kqTmLsv7Xh/2w2RigkePMsg==",
      "license": "Apache-2.0",
      "dependencies": {
        "clsx": "^2.1.1"
      },
      "funding": {
        "url": "https://polar.sh/cva"
      }
    },
    "node_modules/clone": {
      "version": "2.1.2",
      "resolved": "https://registry.npmjs.org/clone/-/clone-2.1.2.tgz",
      "integrity": "sha512-3Pe/CF1Nn94hyhIYpjtiLhdCoEoz0DqQ+988E9gmeEdQZlojxnOb74wctFyuwWQHzqyf9X7C7MG8juUpqBJT8w==",
      "license": "MIT",
      "engines": {
        "node": ">=0.8"
      }
    },
    "node_modules/clsx": {
      "version": "2.1.1",
      "resolved": "https://registry.npmjs.org/clsx/-/clsx-2.1.1.tgz",
      "integrity": "sha512-eYm0QWBtUrBWZWG0d386OGAw16Z995PiOVo2B7bjWSbHedGl5e0ZWaq65kOGgUSNesEIDkB9ISbTg/JK9dhCZA==",
      "license": "MIT",
      "engines": {
        "node": ">=6"
      }
    },
    "node_modules/cmdk": {
      "version": "1.1.1",
      "resolved": "https://registry.npmjs.org/cmdk/-/cmdk-1.1.1.tgz",
      "integrity": "sha512-Vsv7kFaXm+ptHDMZ7izaRsP70GgrW9NBNGswt9OZaVBLlE0SNpDq8eu/VGXyF9r7M0azK3Wy7OlYXsuyYLFzHg==",
      "license": "MIT",
      "dependencies": {
        "@radix-ui/react-compose-refs": "^1.1.1",
        "@radix-ui/react-dialog": "^1.1.6",
        "@radix-ui/react-id": "^1.1.0",
        "@radix-ui/react-primitive": "^2.0.2"
      },
      "peerDependencies": {
        "react": "^18 || ^19 || ^19.0.0-rc",
        "react-dom": "^18 || ^19 || ^19.0.0-rc"
      }
    },
    "node_modules/color-convert": {
      "version": "2.0.1",
      "resolved": "https://registry.npmjs.org/color-convert/-/color-convert-2.0.1.tgz",
      "integrity": "sha512-RRECPsj7iu/xb5oKYcsFHSppFNnsj/52OVTRKb4zP5onXwVF3zVmmToNcOfGC+CRDpfK/U584fMg38ZHCaElKQ==",
      "dev": true,
      "license": "MIT",
      "dependencies": {
        "color-name": "~1.1.4"
      },
      "engines": {
        "node": ">=7.0.0"
      }
    },
    "node_modules/color-name": {
      "version": "1.1.4",
      "resolved": "https://registry.npmjs.org/color-name/-/color-name-1.1.4.tgz",
      "integrity": "sha512-dOy+3AuW3a2wNbZHIuMZpTcgjGuLU/uBL/ubcZF9OXbDo8ff4O8yVp5Bf0efS8uEoYo5q4Fx7dY9OgQGXgAsQA==",
      "dev": true,
      "license": "MIT"
    },
    "node_modules/combined-stream": {
      "version": "1.0.8",
      "resolved": "https://registry.npmjs.org/combined-stream/-/combined-stream-1.0.8.tgz",
      "integrity": "sha512-FQN4MRfuJeHf7cBbBMJFXhKSDq+2kAArBlmRBvcvFE5BB1HZKXtSFASDhdlz9zOYwxh8lDdnvmMOe/+5cdoEdg==",
      "license": "MIT",
      "dependencies": {
        "delayed-stream": "~1.0.0"
      },
      "engines": {
        "node": ">= 0.8"
      }
    },
    "node_modules/comma-separated-tokens": {
      "version": "2.0.3",
      "resolved": "https://registry.npmjs.org/comma-separated-tokens/-/comma-separated-tokens-2.0.3.tgz",
      "integrity": "sha512-Fu4hJdvzeylCfQPp9SGWidpzrMs7tTrlu6Vb8XGaRGck8QSNZJJp538Wrb60Lax4fPwR64ViY468OIUTbRlGZg==",
      "license": "MIT",
      "funding": {
        "type": "github",
        "url": "https://github.com/sponsors/wooorm"
      }
    },
    "node_modules/commander": {
      "version": "4.1.1",
      "resolved": "https://registry.npmjs.org/commander/-/commander-4.1.1.tgz",
      "integrity": "sha512-NOKm8xhkzAjzFx8B2v5OAHT+u5pRQc2UCa2Vq9jYL/31o2wi9mxBA7LIFs3sV5VSC49z6pEhfbMULvShKj26WA==",
      "license": "MIT",
      "engines": {
        "node": ">= 6"
      }
    },
    "node_modules/concat-map": {
      "version": "0.0.1",
      "resolved": "https://registry.npmjs.org/concat-map/-/concat-map-0.0.1.tgz",
      "integrity": "sha512-/Srv4dswyQNBfohGpz9o6Yb3Gz3SrUDqBH5rTuhGR7ahtlbYKnVxw2bCFMRljaA7EXHaXZ8wsHdodFvbkhKmqg==",
      "dev": true,
      "license": "MIT"
    },
    "node_modules/convert-source-map": {
      "version": "2.0.0",
      "resolved": "https://registry.npmjs.org/convert-source-map/-/convert-source-map-2.0.0.tgz",
      "integrity": "sha512-Kvp459HrV2FEJ1CAsi1Ku+MY3kasH19TFykTz2xWmMeq6bk2NU3XXvfJ+Q61m0xktWwt+1HSYf3JZsTms3aRJg==",
      "dev": true,
      "license": "MIT"
    },
    "node_modules/core-js": {
      "version": "3.48.0",
      "resolved": "https://registry.npmjs.org/core-js/-/core-js-3.48.0.tgz",
      "integrity": "sha512-zpEHTy1fjTMZCKLHUZoVeylt9XrzaIN2rbPXEt0k+q7JE5CkCZdo6bNq55bn24a69CH7ErAVLKijxJja4fw+UQ==",
      "hasInstallScript": true,
      "license": "MIT",
      "optional": true,
      "funding": {
        "type": "opencollective",
        "url": "https://opencollective.com/core-js"
      }
    },
    "node_modules/cross-spawn": {
      "version": "7.0.6",
      "resolved": "https://registry.npmjs.org/cross-spawn/-/cross-spawn-7.0.6.tgz",
      "integrity": "sha512-uV2QOWP2nWzsy2aMp8aRibhi9dlzF5Hgh5SHaB9OiTGEyDTiJJyx0uy51QXdyWbtAHNua4XJzUKca3OzKUd3vA==",
      "dev": true,
      "license": "MIT",
      "dependencies": {
        "path-key": "^3.1.0",
        "shebang-command": "^2.0.0",
        "which": "^2.0.1"
      },
      "engines": {
        "node": ">= 8"
      }
    },
    "node_modules/css-box-model": {
      "version": "1.2.1",
      "resolved": "https://registry.npmjs.org/css-box-model/-/css-box-model-1.2.1.tgz",
      "integrity": "sha512-a7Vr4Q/kd/aw96bnJG332W9V9LkJO69JRcaCYDUqjp6/z0w6VcZjgAcTbgFxEPfBgdnAwlh3iwu+hLopa+flJw==",
      "license": "MIT",
      "dependencies": {
        "tiny-invariant": "^1.0.6"
      }
    },
    "node_modules/css-line-break": {
      "version": "2.1.0",
      "resolved": "https://registry.npmjs.org/css-line-break/-/css-line-break-2.1.0.tgz",
      "integrity": "sha512-FHcKFCZcAha3LwfVBhCQbW2nCNbkZXn7KVUJcsT5/P8YmfsVja0FMPJr0B903j/E69HUphKiV9iQArX8SDYA4w==",
      "license": "MIT",
      "dependencies": {
        "utrie": "^1.0.2"
      }
    },
    "node_modules/cssesc": {
      "version": "3.0.0",
      "resolved": "https://registry.npmjs.org/cssesc/-/cssesc-3.0.0.tgz",
      "integrity": "sha512-/Tb/JcjK111nNScGob5MNtsntNM1aCNUDipB/TkwZFhyDrrE47SOx/18wF2bbjgc3ZzCSKW1T5nt5EbFoAz/Vg==",
      "license": "MIT",
      "bin": {
        "cssesc": "bin/cssesc"
      },
      "engines": {
        "node": ">=4"
      }
    },
    "node_modules/csstype": {
      "version": "3.2.3",
      "resolved": "https://registry.npmjs.org/csstype/-/csstype-3.2.3.tgz",
      "integrity": "sha512-z1HGKcYy2xA8AGQfwrn0PAy+PB7X/GSj3UVJW9qKyn43xWa+gl5nXmU4qqLMRzWVLFC8KusUX8T/0kCiOYpAIQ==",
      "license": "MIT"
    },
    "node_modules/d3-array": {
      "version": "3.2.4",
      "resolved": "https://registry.npmjs.org/d3-array/-/d3-array-3.2.4.tgz",
      "integrity": "sha512-tdQAmyA18i4J7wprpYq8ClcxZy3SC31QMeByyCFyRt7BVHdREQZ5lpzoe5mFEYZUWe+oq8HBvk9JjpibyEV4Jg==",
      "license": "ISC",
      "dependencies": {
        "internmap": "1 - 2"
      },
      "engines": {
        "node": ">=12"
      }
    },
    "node_modules/d3-color": {
      "version": "3.1.0",
      "resolved": "https://registry.npmjs.org/d3-color/-/d3-color-3.1.0.tgz",
      "integrity": "sha512-zg/chbXyeBtMQ1LbD/WSoW2DpC3I0mpmPdW+ynRTj/x2DAWYrIY7qeZIHidozwV24m4iavr15lNwIwLxRmOxhA==",
      "license": "ISC",
      "engines": {
        "node": ">=12"
      }
    },
    "node_modules/d3-ease": {
      "version": "3.0.1",
      "resolved": "https://registry.npmjs.org/d3-ease/-/d3-ease-3.0.1.tgz",
      "integrity": "sha512-wR/XK3D3XcLIZwpbvQwQ5fK+8Ykds1ip7A2Txe0yxncXSdq1L9skcG7blcedkOX+ZcgxGAmLX1FrRGbADwzi0w==",
      "license": "BSD-3-Clause",
      "engines": {
        "node": ">=12"
      }
    },
    "node_modules/d3-format": {
      "version": "3.1.2",
      "resolved": "https://registry.npmjs.org/d3-format/-/d3-format-3.1.2.tgz",
      "integrity": "sha512-AJDdYOdnyRDV5b6ArilzCPPwc1ejkHcoyFarqlPqT7zRYjhavcT3uSrqcMvsgh2CgoPbK3RCwyHaVyxYcP2Arg==",
      "license": "ISC",
      "engines": {
        "node": ">=12"
      }
    },
    "node_modules/d3-interpolate": {
      "version": "3.0.1",
      "resolved": "https://registry.npmjs.org/d3-interpolate/-/d3-interpolate-3.0.1.tgz",
      "integrity": "sha512-3bYs1rOD33uo8aqJfKP3JWPAibgw8Zm2+L9vBKEHJ2Rg+viTR7o5Mmv5mZcieN+FRYaAOWX5SJATX6k1PWz72g==",
      "license": "ISC",
      "dependencies": {
        "d3-color": "1 - 3"
      },
      "engines": {
        "node": ">=12"
      }
    },
    "node_modules/d3-path": {
      "version": "3.1.0",
      "resolved": "https://registry.npmjs.org/d3-path/-/d3-path-3.1.0.tgz",
      "integrity": "sha512-p3KP5HCf/bvjBSSKuXid6Zqijx7wIfNW+J/maPs+iwR35at5JCbLUT0LzF1cnjbCHWhqzQTIN2Jpe8pRebIEFQ==",
      "license": "ISC",
      "engines": {
        "node": ">=12"
      }
    },
    "node_modules/d3-scale": {
      "version": "4.0.2",
      "resolved": "https://registry.npmjs.org/d3-scale/-/d3-scale-4.0.2.tgz",
      "integrity": "sha512-GZW464g1SH7ag3Y7hXjf8RoUuAFIqklOAq3MRl4OaWabTFJY9PN/E1YklhXLh+OQ3fM9yS2nOkCoS+WLZ6kvxQ==",
      "license": "ISC",
      "dependencies": {
        "d3-array": "2.10.0 - 3",
        "d3-format": "1 - 3",
        "d3-interpolate": "1.2.0 - 3",
        "d3-time": "2.1.1 - 3",
        "d3-time-format": "2 - 4"
      },
      "engines": {
        "node": ">=12"
      }
    },
    "node_modules/d3-shape": {
      "version": "3.2.0",
      "resolved": "https://registry.npmjs.org/d3-shape/-/d3-shape-3.2.0.tgz",
      "integrity": "sha512-SaLBuwGm3MOViRq2ABk3eLoxwZELpH6zhl3FbAoJ7Vm1gofKx6El1Ib5z23NUEhF9AsGl7y+dzLe5Cw2AArGTA==",
      "license": "ISC",
      "dependencies": {
        "d3-path": "^3.1.0"
      },
      "engines": {
        "node": ">=12"
      }
    },
    "node_modules/d3-time": {
      "version": "3.1.0",
      "resolved": "https://registry.npmjs.org/d3-time/-/d3-time-3.1.0.tgz",
      "integrity": "sha512-VqKjzBLejbSMT4IgbmVgDjpkYrNWUYJnbCGo874u7MMKIWsILRX+OpX/gTk8MqjpT1A/c6HY2dCA77ZN0lkQ2Q==",
      "license": "ISC",
      "dependencies": {
        "d3-array": "2 - 3"
      },
      "engines": {
        "node": ">=12"
      }
    },
    "node_modules/d3-time-format": {
      "version": "4.1.0",
      "resolved": "https://registry.npmjs.org/d3-time-format/-/d3-time-format-4.1.0.tgz",
      "integrity": "sha512-dJxPBlzC7NugB2PDLwo9Q8JiTR3M3e4/XANkreKSUxF8vvXKqm1Yfq4Q5dl8budlunRVlUUaDUgFt7eA8D6NLg==",
      "license": "ISC",
      "dependencies": {
        "d3-time": "1 - 3"
      },
      "engines": {
        "node": ">=12"
      }
    },
    "node_modules/d3-timer": {
      "version": "3.0.1",
      "resolved": "https://registry.npmjs.org/d3-timer/-/d3-timer-3.0.1.tgz",
      "integrity": "sha512-ndfJ/JxxMd3nw31uyKoY2naivF+r29V+Lc0svZxe1JvvIRmi8hUsrMvdOwgS1o6uBHmiz91geQ0ylPP0aj1VUA==",
      "license": "ISC",
      "engines": {
        "node": ">=12"
      }
    },
    "node_modules/data-view-buffer": {
      "version": "1.0.2",
      "resolved": "https://registry.npmjs.org/data-view-buffer/-/data-view-buffer-1.0.2.tgz",
      "integrity": "sha512-EmKO5V3OLXh1rtK2wgXRansaK1/mtVdTUEiEI0W8RkvgT05kfxaH29PliLnpLP73yYO6142Q72QNa8Wx/A5CqQ==",
      "dev": true,
      "license": "MIT",
      "dependencies": {
        "call-bound": "^1.0.3",
        "es-errors": "^1.3.0",
        "is-data-view": "^1.0.2"
      },
      "engines": {
        "node": ">= 0.4"
      },
      "funding": {
        "url": "https://github.com/sponsors/ljharb"
      }
    },
    "node_modules/data-view-byte-length": {
      "version": "1.0.2",
      "resolved": "https://registry.npmjs.org/data-view-byte-length/-/data-view-byte-length-1.0.2.tgz",
      "integrity": "sha512-tuhGbE6CfTM9+5ANGf+oQb72Ky/0+s3xKUpHvShfiz2RxMFgFPjsXuRLBVMtvMs15awe45SRb83D6wH4ew6wlQ==",
      "dev": true,
      "license": "MIT",
      "dependencies": {
        "call-bound": "^1.0.3",
        "es-errors": "^1.3.0",
        "is-data-view": "^1.0.2"
      },
      "engines": {
        "node": ">= 0.4"
      },
      "funding": {
        "url": "https://github.com/sponsors/inspect-js"
      }
    },
    "node_modules/data-view-byte-offset": {
      "version": "1.0.1",
      "resolved": "https://registry.npmjs.org/data-view-byte-offset/-/data-view-byte-offset-1.0.1.tgz",
      "integrity": "sha512-BS8PfmtDGnrgYdOonGZQdLZslWIeCGFP9tpan0hi1Co2Zr2NKADsvGYA8XxuG/4UWgJ6Cjtv+YJnB6MM69QGlQ==",
      "dev": true,
      "license": "MIT",
      "dependencies": {
        "call-bound": "^1.0.2",
        "es-errors": "^1.3.0",
        "is-data-view": "^1.0.1"
      },
      "engines": {
        "node": ">= 0.4"
      },
      "funding": {
        "url": "https://github.com/sponsors/ljharb"
      }
    },
    "node_modules/date-fns": {
      "version": "3.6.0",
      "resolved": "https://registry.npmjs.org/date-fns/-/date-fns-3.6.0.tgz",
      "integrity": "sha512-fRHTG8g/Gif+kSh50gaGEdToemgfj74aRX3swtiouboip5JDLAyDE9F11nHMIcvOaXeOC6D7SpNhi7uFyB7Uww==",
      "license": "MIT",
      "funding": {
        "type": "github",
        "url": "https://github.com/sponsors/kossnocorp"
      }
    },
    "node_modules/debug": {
      "version": "4.4.3",
      "resolved": "https://registry.npmjs.org/debug/-/debug-4.4.3.tgz",
      "integrity": "sha512-RGwwWnwQvkVfavKVt22FGLw+xYSdzARwm0ru6DhTVA3umU5hZc28V3kO4stgYryrTlLpuvgI9GiijltAjNbcqA==",
      "license": "MIT",
      "dependencies": {
        "ms": "^2.1.3"
      },
      "engines": {
        "node": ">=6.0"
      },
      "peerDependenciesMeta": {
        "supports-color": {
          "optional": true
        }
      }
    },
    "node_modules/decimal.js-light": {
      "version": "2.5.1",
      "resolved": "https://registry.npmjs.org/decimal.js-light/-/decimal.js-light-2.5.1.tgz",
      "integrity": "sha512-qIMFpTMZmny+MMIitAB6D7iVPEorVw6YQRWkvarTkT4tBeSLLiHzcwj6q0MmYSFCiVpiqPJTJEYIrpcPzVEIvg==",
      "license": "MIT"
    },
    "node_modules/decode-named-character-reference": {
      "version": "1.3.0",
      "resolved": "https://registry.npmjs.org/decode-named-character-reference/-/decode-named-character-reference-1.3.0.tgz",
      "integrity": "sha512-GtpQYB283KrPp6nRw50q3U9/VfOutZOe103qlN7BPP6Ad27xYnOIWv4lPzo8HCAL+mMZofJ9KEy30fq6MfaK6Q==",
      "license": "MIT",
      "dependencies": {
        "character-entities": "^2.0.0"
      },
      "funding": {
        "type": "github",
        "url": "https://github.com/sponsors/wooorm"
      }
    },
    "node_modules/deep-equal": {
      "version": "1.1.2",
      "resolved": "https://registry.npmjs.org/deep-equal/-/deep-equal-1.1.2.tgz",
      "integrity": "sha512-5tdhKF6DbU7iIzrIOa1AOUt39ZRm13cmL1cGEh//aqR8x9+tNfbywRf0n5FD/18OKMdo7DNEtrX2t22ZAkI+eg==",
      "license": "MIT",
      "dependencies": {
        "is-arguments": "^1.1.1",
        "is-date-object": "^1.0.5",
        "is-regex": "^1.1.4",
        "object-is": "^1.1.5",
        "object-keys": "^1.1.1",
        "regexp.prototype.flags": "^1.5.1"
      },
      "engines": {
        "node": ">= 0.4"
      },
      "funding": {
        "url": "https://github.com/sponsors/ljharb"
      }
    },
    "node_modules/deep-is": {
      "version": "0.1.4",
      "resolved": "https://registry.npmjs.org/deep-is/-/deep-is-0.1.4.tgz",
      "integrity": "sha512-oIPzksmTg4/MriiaYGO+okXDT7ztn/w3Eptv/+gSIdMdKsJo0u4CfYNFJPy+4SKMuCqGw2wxnA+URMg3t8a/bQ==",
      "dev": true,
      "license": "MIT"
    },
    "node_modules/define-data-property": {
      "version": "1.1.4",
      "resolved": "https://registry.npmjs.org/define-data-property/-/define-data-property-1.1.4.tgz",
      "integrity": "sha512-rBMvIzlpA8v6E+SJZoo++HAYqsLrkg7MSfIinMPFhmkorw7X+dOXVJQs+QT69zGkzMyfDnIMN2Wid1+NbL3T+A==",
      "license": "MIT",
      "dependencies": {
        "es-define-property": "^1.0.0",
        "es-errors": "^1.3.0",
        "gopd": "^1.0.1"
      },
      "engines": {
        "node": ">= 0.4"
      },
      "funding": {
        "url": "https://github.com/sponsors/ljharb"
      }
    },
    "node_modules/define-properties": {
      "version": "1.2.1",
      "resolved": "https://registry.npmjs.org/define-properties/-/define-properties-1.2.1.tgz",
      "integrity": "sha512-8QmQKqEASLd5nx0U1B1okLElbUuuttJ/AnYmRXbbbGDWh6uS208EjD4Xqq/I9wK7u0v6O08XhTWnt5XtEbR6Dg==",
      "license": "MIT",
      "dependencies": {
        "define-data-property": "^1.0.1",
        "has-property-descriptors": "^1.0.0",
        "object-keys": "^1.1.1"
      },
      "engines": {
        "node": ">= 0.4"
      },
      "funding": {
        "url": "https://github.com/sponsors/ljharb"
      }
    },
    "node_modules/delayed-stream": {
      "version": "1.0.0",
      "resolved": "https://registry.npmjs.org/delayed-stream/-/delayed-stream-1.0.0.tgz",
      "integrity": "sha512-ZySD7Nf91aLB0RxL4KGrKHBXl7Eds1DAmEdcoVawXnLD7SDhpNgtuII2aAkg7a7QS41jxPSZ17p4VdGnMHk3MQ==",
      "license": "MIT",
      "engines": {
        "node": ">=0.4.0"
      }
    },
    "node_modules/dequal": {
      "version": "2.0.3",
      "resolved": "https://registry.npmjs.org/dequal/-/dequal-2.0.3.tgz",
      "integrity": "sha512-0je+qPKHEMohvfRTCEo3CrPG6cAzAYgmzKyxRiYSSDkS6eGJdyVJm7WaYA5ECaAD9wLB2T4EEeymA5aFVcYXCA==",
      "license": "MIT",
      "engines": {
        "node": ">=6"
      }
    },
    "node_modules/detect-node-es": {
      "version": "1.1.0",
      "resolved": "https://registry.npmjs.org/detect-node-es/-/detect-node-es-1.1.0.tgz",
      "integrity": "sha512-ypdmJU/TbBby2Dxibuv7ZLW3Bs1QEmM7nHjEANfohJLvE0XVujisn1qPJcZxg+qDucsr+bP6fLD1rPS3AhJ7EQ==",
      "license": "MIT"
    },
    "node_modules/devlop": {
      "version": "1.1.0",
      "resolved": "https://registry.npmjs.org/devlop/-/devlop-1.1.0.tgz",
      "integrity": "sha512-RWmIqhcFf1lRYBvNmr7qTNuyCt/7/ns2jbpp1+PalgE/rDQcBT0fioSMUpJ93irlUhC5hrg4cYqe6U+0ImW0rA==",
      "license": "MIT",
      "dependencies": {
        "dequal": "^2.0.0"
      },
      "funding": {
        "type": "github",
        "url": "https://github.com/sponsors/wooorm"
      }
    },
    "node_modules/didyoumean": {
      "version": "1.2.2",
      "resolved": "https://registry.npmjs.org/didyoumean/-/didyoumean-1.2.2.tgz",
      "integrity": "sha512-gxtyfqMg7GKyhQmb056K7M3xszy/myH8w+B4RT+QXBQsvAOdc3XymqDDPHx1BgPgsdAA5SIifona89YtRATDzw==",
      "license": "Apache-2.0"
    },
    "node_modules/dlv": {
      "version": "1.1.3",
      "resolved": "https://registry.npmjs.org/dlv/-/dlv-1.1.3.tgz",
      "integrity": "sha512-+HlytyjlPKnIG8XuRG8WvmBP8xs8P71y+SKKS6ZXWoEgLuePxtDoUEiH7WkdePWrQ5JBpE6aoVqfZfJUQkjXwA==",
      "license": "MIT"
    },
    "node_modules/doctrine": {
      "version": "2.1.0",
      "resolved": "https://registry.npmjs.org/doctrine/-/doctrine-2.1.0.tgz",
      "integrity": "sha512-35mSku4ZXK0vfCuHEDAwt55dg2jNajHZ1odvF+8SSr82EsZY4QmXfuWso8oEd8zRhVObSN18aM0CjSdoBX7zIw==",
      "dev": true,
      "license": "Apache-2.0",
      "dependencies": {
        "esutils": "^2.0.2"
      },
      "engines": {
        "node": ">=0.10.0"
      }
    },
    "node_modules/dom-helpers": {
      "version": "5.2.1",
      "resolved": "https://registry.npmjs.org/dom-helpers/-/dom-helpers-5.2.1.tgz",
      "integrity": "sha512-nRCa7CK3VTrM2NmGkIy4cbK7IZlgBE/PYMn55rrXefr5xXDP0LdtfPnblFDoVdcAfslJ7or6iqAUnx0CCGIWQA==",
      "license": "MIT",
      "dependencies": {
        "@babel/runtime": "^7.8.7",
        "csstype": "^3.0.2"
      }
    },
    "node_modules/dompurify": {
      "version": "3.4.11",
      "resolved": "https://registry.npmjs.org/dompurify/-/dompurify-3.4.11.tgz",
      "integrity": "sha512-zhlUV12GsaRzMsf9q5M254YhA4+VuF0fG+QFqu6aYpoGlKtz+w8//jBcGVYBgQkR5GHjUomejY84AV+/uPbWdw==",
      "license": "(MPL-2.0 OR Apache-2.0)",
      "optional": true,
      "optionalDependencies": {
        "@types/trusted-types": "^2.0.7"
      }
    },
    "node_modules/dunder-proto": {
      "version": "1.0.1",
      "resolved": "https://registry.npmjs.org/dunder-proto/-/dunder-proto-1.0.1.tgz",
      "integrity": "sha512-KIN/nDJBQRcXw0MLVhZE9iQHmG68qAVIBg9CqmUYjmQIhgij9U5MFvrqkUL5FbtyyzZuOeOt0zdeRe4UY7ct+A==",
      "license": "MIT",
      "dependencies": {
        "call-bind-apply-helpers": "^1.0.1",
        "es-errors": "^1.3.0",
        "gopd": "^1.2.0"
      },
      "engines": {
        "node": ">= 0.4"
      }
    },
    "node_modules/electron-to-chromium": {
      "version": "1.5.286",
      "resolved": "https://registry.npmjs.org/electron-to-chromium/-/electron-to-chromium-1.5.286.tgz",
      "integrity": "sha512-9tfDXhJ4RKFNerfjdCcZfufu49vg620741MNs26a9+bhLThdB+plgMeou98CAaHu/WATj2iHOOHTp1hWtABj2A==",
      "dev": true,
      "license": "ISC"
    },
    "node_modules/embla-carousel": {
      "version": "8.6.0",
      "resolved": "https://registry.npmjs.org/embla-carousel/-/embla-carousel-8.6.0.tgz",
      "integrity": "sha512-SjWyZBHJPbqxHOzckOfo8lHisEaJWmwd23XppYFYVh10bU66/Pn5tkVkbkCMZVdbUE5eTCI2nD8OyIP4Z+uwkA==",
      "license": "MIT"
    },
    "node_modules/embla-carousel-react": {
      "version": "8.6.0",
      "resolved": "https://registry.npmjs.org/embla-carousel-react/-/embla-carousel-react-8.6.0.tgz",
      "integrity": "sha512-0/PjqU7geVmo6F734pmPqpyHqiM99olvyecY7zdweCw+6tKEXnrE90pBiBbMMU8s5tICemzpQ3hi5EpxzGW+JA==",
      "license": "MIT",
      "dependencies": {
        "embla-carousel": "8.6.0",
        "embla-carousel-reactive-utils": "8.6.0"
      },
      "peerDependencies": {
        "react": "^16.8.0 || ^17.0.1 || ^18.0.0 || ^19.0.0 || ^19.0.0-rc"
      }
    },
    "node_modules/embla-carousel-reactive-utils": {
      "version": "8.6.0",
      "resolved": "https://registry.npmjs.org/embla-carousel-reactive-utils/-/embla-carousel-reactive-utils-8.6.0.tgz",
      "integrity": "sha512-fMVUDUEx0/uIEDM0Mz3dHznDhfX+znCCDCeIophYb1QGVM7YThSWX+wz11zlYwWFOr74b4QLGg0hrGPJeG2s4A==",
      "license": "MIT",
      "peerDependencies": {
        "embla-carousel": "8.6.0"
      }
    },
    "node_modules/engine.io-client": {
      "version": "6.6.6",
      "resolved": "https://registry.npmjs.org/engine.io-client/-/engine.io-client-6.6.6.tgz",
      "integrity": "sha512-iY6QdftLQ9pyiPoX082bpf/u1UewnOaJrtJIF9T0++QB34lZrj0uP+Q/bj8AlUsAxqhnkTV2BS8SBZSxOmoV5Q==",
      "license": "MIT",
      "dependencies": {
        "@socket.io/component-emitter": "~3.1.0",
        "debug": "~4.4.1",
        "engine.io-parser": "~5.2.1",
        "ws": "~8.21.0",
        "xmlhttprequest-ssl": "~2.1.1"
      }
    },
    "node_modules/engine.io-parser": {
      "version": "5.2.3",
      "resolved": "https://registry.npmjs.org/engine.io-parser/-/engine.io-parser-5.2.3.tgz",
      "integrity": "sha512-HqD3yTBfnBxIrbnM1DoD6Pcq8NECnh8d4As1Qgh0z5Gg3jRRIqijury0CL3ghu/edArpUYiYqQiDUQBIs4np3Q==",
      "license": "MIT",
      "engines": {
        "node": ">=10.0.0"
      }
    },
    "node_modules/es-abstract": {
      "version": "1.24.1",
      "resolved": "https://registry.npmjs.org/es-abstract/-/es-abstract-1.24.1.tgz",
      "integrity": "sha512-zHXBLhP+QehSSbsS9Pt23Gg964240DPd6QCf8WpkqEXxQ7fhdZzYsocOr5u7apWonsS5EjZDmTF+/slGMyasvw==",
      "dev": true,
      "license": "MIT",
      "dependencies": {
        "array-buffer-byte-length": "^1.0.2",
        "arraybuffer.prototype.slice": "^1.0.4",
        "available-typed-arrays": "^1.0.7",
        "call-bind": "^1.0.8",
        "call-bound": "^1.0.4",
        "data-view-buffer": "^1.0.2",
        "data-view-byte-length": "^1.0.2",
        "data-view-byte-offset": "^1.0.1",
        "es-define-property": "^1.0.1",
        "es-errors": "^1.3.0",
        "es-object-atoms": "^1.1.1",
        "es-set-tostringtag": "^2.1.0",
        "es-to-primitive": "^1.3.0",
        "function.prototype.name": "^1.1.8",
        "get-intrinsic": "^1.3.0",
        "get-proto": "^1.0.1",
        "get-symbol-description": "^1.1.0",
        "globalthis": "^1.0.4",
        "gopd": "^1.2.0",
        "has-property-descriptors": "^1.0.2",
        "has-proto": "^1.2.0",
        "has-symbols": "^1.1.0",
        "hasown": "^2.0.2",
        "internal-slot": "^1.1.0",
        "is-array-buffer": "^3.0.5",
        "is-callable": "^1.2.7",
        "is-data-view": "^1.0.2",
        "is-negative-zero": "^2.0.3",
        "is-regex": "^1.2.1",
        "is-set": "^2.0.3",
        "is-shared-array-buffer": "^1.0.4",
        "is-string": "^1.1.1",
        "is-typed-array": "^1.1.15",
        "is-weakref": "^1.1.1",
        "math-intrinsics": "^1.1.0",
        "object-inspect": "^1.13.4",
        "object-keys": "^1.1.1",
        "object.assign": "^4.1.7",
        "own-keys": "^1.0.1",
        "regexp.prototype.flags": "^1.5.4",
        "safe-array-concat": "^1.1.3",
        "safe-push-apply": "^1.0.0",
        "safe-regex-test": "^1.1.0",
        "set-proto": "^1.0.0",
        "stop-iteration-iterator": "^1.1.0",
        "string.prototype.trim": "^1.2.10",
        "string.prototype.trimend": "^1.0.9",
        "string.prototype.trimstart": "^1.0.8",
        "typed-array-buffer": "^1.0.3",
        "typed-array-byte-length": "^1.0.3",
        "typed-array-byte-offset": "^1.0.4",
        "typed-array-length": "^1.0.7",
        "unbox-primitive": "^1.1.0",
        "which-typed-array": "^1.1.19"
      },
      "engines": {
        "node": ">= 0.4"
      },
      "funding": {
        "url": "https://github.com/sponsors/ljharb"
      }
    },
    "node_modules/es-define-property": {
      "version": "1.0.1",
      "resolved": "https://registry.npmjs.org/es-define-property/-/es-define-property-1.0.1.tgz",
      "integrity": "sha512-e3nRfgfUZ4rNGL232gUgX06QNyyez04KdjFrF+LTRoOXmrOgFKDg4BCdsjW8EnT69eqdYGmRpJwiPVYNrCaW3g==",
      "license": "MIT",
      "engines": {
        "node": ">= 0.4"
      }
    },
    "node_modules/es-errors": {
      "version": "1.3.0",
      "resolved": "https://registry.npmjs.org/es-errors/-/es-errors-1.3.0.tgz",
      "integrity": "sha512-Zf5H2Kxt2xjTvbJvP2ZWLEICxA6j+hAmMzIlypy4xcBg1vKVnx89Wy0GbS+kf5cwCVFFzdCFh2XSCFNULS6csw==",
      "license": "MIT",
      "engines": {
        "node": ">= 0.4"
      }
    },
    "node_modules/es-iterator-helpers": {
      "version": "1.2.2",
      "resolved": "https://registry.npmjs.org/es-iterator-helpers/-/es-iterator-helpers-1.2.2.tgz",
      "integrity": "sha512-BrUQ0cPTB/IwXj23HtwHjS9n7O4h9FX94b4xc5zlTHxeLgTAdzYUDyy6KdExAl9lbN5rtfe44xpjpmj9grxs5w==",
      "dev": true,
      "license": "MIT",
      "dependencies": {
        "call-bind": "^1.0.8",
        "call-bound": "^1.0.4",
        "define-properties": "^1.2.1",
        "es-abstract": "^1.24.1",
        "es-errors": "^1.3.0",
        "es-set-tostringtag": "^2.1.0",
        "function-bind": "^1.1.2",
        "get-intrinsic": "^1.3.0",
        "globalthis": "^1.0.4",
        "gopd": "^1.2.0",
        "has-property-descriptors": "^1.0.2",
        "has-proto": "^1.2.0",
        "has-symbols": "^1.1.0",
        "internal-slot": "^1.1.0",
        "iterator.prototype": "^1.1.5",
        "safe-array-concat": "^1.1.3"
      },
      "engines": {
        "node": ">= 0.4"
      }
    },
    "node_modules/es-object-atoms": {
      "version": "1.1.1",
      "resolved": "https://registry.npmjs.org/es-object-atoms/-/es-object-atoms-1.1.1.tgz",
      "integrity": "sha512-FGgH2h8zKNim9ljj7dankFPcICIK9Cp5bm+c2gQSYePhpaG5+esrLODihIorn+Pe6FGJzWhXQotPv73jTaldXA==",
      "license": "MIT",
      "dependencies": {
        "es-errors": "^1.3.0"
      },
      "engines": {
        "node": ">= 0.4"
      }
    },
    "node_modules/es-set-tostringtag": {
      "version": "2.1.0",
      "resolved": "https://registry.npmjs.org/es-set-tostringtag/-/es-set-tostringtag-2.1.0.tgz",
      "integrity": "sha512-j6vWzfrGVfyXxge+O0x5sh6cvxAog0a/4Rdd2K36zCMV5eJ+/+tOAngRO8cODMNWbVRdVlmGZQL2YS3yR8bIUA==",
      "license": "MIT",
      "dependencies": {
        "es-errors": "^1.3.0",
        "get-intrinsic": "^1.2.6",
        "has-tostringtag": "^1.0.2",
        "hasown": "^2.0.2"
      },
      "engines": {
        "node": ">= 0.4"
      }
    },
    "node_modules/es-shim-unscopables": {
      "version": "1.1.0",
      "resolved": "https://registry.npmjs.org/es-shim-unscopables/-/es-shim-unscopables-1.1.0.tgz",
      "integrity": "sha512-d9T8ucsEhh8Bi1woXCf+TIKDIROLG5WCkxg8geBCbvk22kzwC5G2OnXVMO6FUsvQlgUUXQ2itephWDLqDzbeCw==",
      "dev": true,
      "license": "MIT",
      "dependencies": {
        "hasown": "^2.0.2"
      },
      "engines": {
        "node": ">= 0.4"
      }
    },
    "node_modules/es-to-primitive": {
      "version": "1.3.0",
      "resolved": "https://registry.npmjs.org/es-to-primitive/-/es-to-primitive-1.3.0.tgz",
      "integrity": "sha512-w+5mJ3GuFL+NjVtJlvydShqE1eN3h3PbI7/5LAsYJP/2qtuMXjfL2LpHSRqo4b4eSF5K/DH1JXKUAHSB2UW50g==",
      "dev": true,
      "license": "MIT",
      "dependencies": {
        "is-callable": "^1.2.7",
        "is-date-object": "^1.0.5",
        "is-symbol": "^1.0.4"
      },
      "engines": {
        "node": ">= 0.4"
      },
      "funding": {
        "url": "https://github.com/sponsors/ljharb"
      }
    },
    "node_modules/esbuild": {
      "version": "0.25.12",
      "resolved": "https://registry.npmjs.org/esbuild/-/esbuild-0.25.12.tgz",
      "integrity": "sha512-bbPBYYrtZbkt6Os6FiTLCTFxvq4tt3JKall1vRwshA3fdVztsLAatFaZobhkBC8/BrPetoa0oksYoKXoG4ryJg==",
      "dev": true,
      "hasInstallScript": true,
      "license": "MIT",
      "bin": {
        "esbuild": "bin/esbuild"
      },
      "engines": {
        "node": ">=18"
      },
      "optionalDependencies": {
        "@esbuild/aix-ppc64": "0.25.12",
        "@esbuild/android-arm": "0.25.12",
        "@esbuild/android-arm64": "0.25.12",
        "@esbuild/android-x64": "0.25.12",
        "@esbuild/darwin-arm64": "0.25.12",
        "@esbuild/darwin-x64": "0.25.12",
        "@esbuild/freebsd-arm64": "0.25.12",
        "@esbuild/freebsd-x64": "0.25.12",
        "@esbuild/linux-arm": "0.25.12",
        "@esbuild/linux-arm64": "0.25.12",
        "@esbuild/linux-ia32": "0.25.12",
        "@esbuild/linux-loong64": "0.25.12",
        "@esbuild/linux-mips64el": "0.25.12",
        "@esbuild/linux-ppc64": "0.25.12",
        "@esbuild/linux-riscv64": "0.25.12",
        "@esbuild/linux-s390x": "0.25.12",
        "@esbuild/linux-x64": "0.25.12",
        "@esbuild/netbsd-arm64": "0.25.12",
        "@esbuild/netbsd-x64": "0.25.12",
        "@esbuild/openbsd-arm64": "0.25.12",
        "@esbuild/openbsd-x64": "0.25.12",
        "@esbuild/openharmony-arm64": "0.25.12",
        "@esbuild/sunos-x64": "0.25.12",
        "@esbuild/win32-arm64": "0.25.12",
        "@esbuild/win32-ia32": "0.25.12",
        "@esbuild/win32-x64": "0.25.12"
      }
    },
    "node_modules/escalade": {
      "version": "3.2.0",
      "resolved": "https://registry.npmjs.org/escalade/-/escalade-3.2.0.tgz",
      "integrity": "sha512-WUj2qlxaQtO4g6Pq5c29GTcWGDyd8itL8zTlipgECz3JesAiiOKotd8JU6otB3PACgG6xkJUyVhboMS+bje/jA==",
      "dev": true,
      "license": "MIT",
      "engines": {
        "node": ">=6"
      }
    },
    "node_modules/escape-string-regexp": {
      "version": "4.0.0",
      "resolved": "https://registry.npmjs.org/escape-string-regexp/-/escape-string-regexp-4.0.0.tgz",
      "integrity": "sha512-TtpcNJ3XAzx3Gq8sWRzJaVajRs0uVxA2YAkdb1jm2YkPz4G6egUFAyA3n5vtEIZefPk5Wa4UXbKuS5fKkJWdgA==",
      "dev": true,
      "license": "MIT",
      "engines": {
        "node": ">=10"
      },
      "funding": {
        "url": "https://github.com/sponsors/sindresorhus"
      }
    },
    "node_modules/eslint": {
      "version": "9.39.2",
      "resolved": "https://registry.npmjs.org/eslint/-/eslint-9.39.2.tgz",
      "integrity": "sha512-LEyamqS7W5HB3ujJyvi0HQK/dtVINZvd5mAAp9eT5S/ujByGjiZLCzPcHVzuXbpJDJF/cxwHlfceVUDZ2lnSTw==",
      "dev": true,
      "license": "MIT",
      "dependencies": {
        "@eslint-community/eslint-utils": "^4.8.0",
        "@eslint-community/regexpp": "^4.12.1",
        "@eslint/config-array": "^0.21.1",
        "@eslint/config-helpers": "^0.4.2",
        "@eslint/core": "^0.17.0",
        "@eslint/eslintrc": "^3.3.1",
        "@eslint/js": "9.39.2",
        "@eslint/plugin-kit": "^0.4.1",
        "@humanfs/node": "^0.16.6",
        "@humanwhocodes/module-importer": "^1.0.1",
        "@humanwhocodes/retry": "^0.4.2",
        "@types/estree": "^1.0.6",
        "ajv": "^6.12.4",
        "chalk": "^4.0.0",
        "cross-spawn": "^7.0.6",
        "debug": "^4.3.2",
        "escape-string-regexp": "^4.0.0",
        "eslint-scope": "^8.4.0",
        "eslint-visitor-keys": "^4.2.1",
        "espree": "^10.4.0",
        "esquery": "^1.5.0",
        "esutils": "^2.0.2",
        "fast-deep-equal": "^3.1.3",
        "file-entry-cache": "^8.0.0",
        "find-up": "^5.0.0",
        "glob-parent": "^6.0.2",
        "ignore": "^5.2.0",
        "imurmurhash": "^0.1.4",
        "is-glob": "^4.0.0",
        "json-stable-stringify-without-jsonify": "^1.0.1",
        "lodash.merge": "^4.6.2",
        "minimatch": "^3.1.2",
        "natural-compare": "^1.4.0",
        "optionator": "^0.9.3"
      },
      "bin": {
        "eslint": "bin/eslint.js"
      },
      "engines": {
        "node": "^18.18.0 || ^20.9.0 || >=21.1.0"
      },
      "funding": {
        "url": "https://eslint.org/donate"
      },
      "peerDependencies": {
        "jiti": "*"
      },
      "peerDependenciesMeta": {
        "jiti": {
          "optional": true
        }
      }
    },
    "node_modules/eslint-plugin-react": {
      "version": "7.37.5",
      "resolved": "https://registry.npmjs.org/eslint-plugin-react/-/eslint-plugin-react-7.37.5.tgz",
      "integrity": "sha512-Qteup0SqU15kdocexFNAJMvCJEfa2xUKNV4CC1xsVMrIIqEy3SQ/rqyxCWNzfrd3/ldy6HMlD2e0JDVpDg2qIA==",
      "dev": true,
      "license": "MIT",
      "dependencies": {
        "array-includes": "^3.1.8",
        "array.prototype.findlast": "^1.2.5",
        "array.prototype.flatmap": "^1.3.3",
        "array.prototype.tosorted": "^1.1.4",
        "doctrine": "^2.1.0",
        "es-iterator-helpers": "^1.2.1",
        "estraverse": "^5.3.0",
        "hasown": "^2.0.2",
        "jsx-ast-utils": "^2.4.1 || ^3.0.0",
        "minimatch": "^3.1.2",
        "object.entries": "^1.1.9",
        "object.fromentries": "^2.0.8",
        "object.values": "^1.2.1",
        "prop-types": "^15.8.1",
        "resolve": "^2.0.0-next.5",
        "semver": "^6.3.1",
        "string.prototype.matchall": "^4.0.12",
        "string.prototype.repeat": "^1.0.0"
      },
      "engines": {
        "node": ">=4"
      },
      "peerDependencies": {
        "eslint": "^3 || ^4 || ^5 || ^6 || ^7 || ^8 || ^9.7"
      }
    },
    "node_modules/eslint-plugin-react-hooks": {
      "version": "5.2.0",
      "resolved": "https://registry.npmjs.org/eslint-plugin-react-hooks/-/eslint-plugin-react-hooks-5.2.0.tgz",
      "integrity": "sha512-+f15FfK64YQwZdJNELETdn5ibXEUQmW1DZL6KXhNnc2heoy/sg9VJJeT7n8TlMWouzWqSWavFkIhHyIbIAEapg==",
      "dev": true,
      "license": "MIT",
      "engines": {
        "node": ">=10"
      },
      "peerDependencies": {
        "eslint": "^3.0.0 || ^4.0.0 || ^5.0.0 || ^6.0.0 || ^7.0.0 || ^8.0.0-0 || ^9.0.0"
      }
    },
    "node_modules/eslint-plugin-react-refresh": {
      "version": "0.4.26",
      "resolved": "https://registry.npmjs.org/eslint-plugin-react-refresh/-/eslint-plugin-react-refresh-0.4.26.tgz",
      "integrity": "sha512-1RETEylht2O6FM/MvgnyvT+8K21wLqDNg4qD51Zj3guhjt433XbnnkVttHMyaVyAFD03QSV4LPS5iE3VQmO7XQ==",
      "dev": true,
      "license": "MIT",
      "peerDependencies": {
        "eslint": ">=8.40"
      }
    },
    "node_modules/eslint-plugin-unused-imports": {
      "version": "4.4.1",
      "resolved": "https://registry.npmjs.org/eslint-plugin-unused-imports/-/eslint-plugin-unused-imports-4.4.1.tgz",
      "integrity": "sha512-oZGYUz1X3sRMGUB+0cZyK2VcvRX5lm/vB56PgNNcU+7ficUCKm66oZWKUubXWnOuPjQ8PvmXtCViXBMONPe7tQ==",
      "dev": true,
      "license": "MIT",
      "peerDependencies": {
        "@typescript-eslint/eslint-plugin": "^8.0.0-0 || ^7.0.0 || ^6.0.0 || ^5.0.0",
        "eslint": "^10.0.0 || ^9.0.0 || ^8.0.0"
      },
      "peerDependenciesMeta": {
        "@typescript-eslint/eslint-plugin": {
          "optional": true
        }
      }
    },
    "node_modules/eslint-scope": {
      "version": "8.4.0",
      "resolved": "https://registry.npmjs.org/eslint-scope/-/eslint-scope-8.4.0.tgz",
      "integrity": "sha512-sNXOfKCn74rt8RICKMvJS7XKV/Xk9kA7DyJr8mJik3S7Cwgy3qlkkmyS2uQB3jiJg6VNdZd/pDBJu0nvG2NlTg==",
      "dev": true,
      "license": "BSD-2-Clause",
      "dependencies": {
        "esrecurse": "^4.3.0",
        "estraverse": "^5.2.0"
      },
      "engines": {
        "node": "^18.18.0 || ^20.9.0 || >=21.1.0"
      },
      "funding": {
        "url": "https://opencollective.com/eslint"
      }
    },
    "node_modules/eslint-visitor-keys": {
      "version": "4.2.1",
      "resolved": "https://registry.npmjs.org/eslint-visitor-keys/-/eslint-visitor-keys-4.2.1.tgz",
      "integrity": "sha512-Uhdk5sfqcee/9H/rCOJikYz67o0a2Tw2hGRPOG2Y1R2dg7brRe1uG0yaNQDHu+TO/uQPF/5eCapvYSmHUjt7JQ==",
      "dev": true,
      "license": "Apache-2.0",
      "engines": {
        "node": "^18.18.0 || ^20.9.0 || >=21.1.0"
      },
      "funding": {
        "url": "https://opencollective.com/eslint"
      }
    },
    "node_modules/espree": {
      "version": "10.4.0",
      "resolved": "https://registry.npmjs.org/espree/-/espree-10.4.0.tgz",
      "integrity": "sha512-j6PAQ2uUr79PZhBjP5C5fhl8e39FmRnOjsD5lGnWrFU8i2G776tBK7+nP8KuQUTTyAZUwfQqXAgrVH5MbH9CYQ==",
      "dev": true,
      "license": "BSD-2-Clause",
      "dependencies": {
        "acorn": "^8.15.0",
        "acorn-jsx": "^5.3.2",
        "eslint-visitor-keys": "^4.2.1"
      },
      "engines": {
        "node": "^18.18.0 || ^20.9.0 || >=21.1.0"
      },
      "funding": {
        "url": "https://opencollective.com/eslint"
      }
    },
    "node_modules/esquery": {
      "version": "1.7.0",
      "resolved": "https://registry.npmjs.org/esquery/-/esquery-1.7.0.tgz",
      "integrity": "sha512-Ap6G0WQwcU/LHsvLwON1fAQX9Zp0A2Y6Y/cJBl9r/JbW90Zyg4/zbG6zzKa2OTALELarYHmKu0GhpM5EO+7T0g==",
      "dev": true,
      "license": "BSD-3-Clause",
      "dependencies": {
        "estraverse": "^5.1.0"
      },
      "engines": {
        "node": ">=0.10"
      }
    },
    "node_modules/esrecurse": {
      "version": "4.3.0",
      "resolved": "https://registry.npmjs.org/esrecurse/-/esrecurse-4.3.0.tgz",
      "integrity": "sha512-KmfKL3b6G+RXvP8N1vr3Tq1kL/oCFgn2NYXEtqP8/L3pKapUA4G8cFVaoF3SU323CD4XypR/ffioHmkti6/Tag==",
      "dev": true,
      "license": "BSD-2-Clause",
      "dependencies": {
        "estraverse": "^5.2.0"
      },
      "engines": {
        "node": ">=4.0"
      }
    },
    "node_modules/estraverse": {
      "version": "5.3.0",
      "resolved": "https://registry.npmjs.org/estraverse/-/estraverse-5.3.0.tgz",
      "integrity": "sha512-MMdARuVEQziNTeJD8DgMqmhwR11BRQ/cBP+pLtYdSTnf3MIO8fFeiINEbX36ZdNlfU/7A9f3gUw49B3oQsvwBA==",
      "dev": true,
      "license": "BSD-2-Clause",
      "engines": {
        "node": ">=4.0"
      }
    },
    "node_modules/estree-util-is-identifier-name": {
      "version": "3.0.0",
      "resolved": "https://registry.npmjs.org/estree-util-is-identifier-name/-/estree-util-is-identifier-name-3.0.0.tgz",
      "integrity": "sha512-hFtqIDZTIUZ9BXLb8y4pYGyk6+wekIivNVTcmvk8NoOh+VeRn5y6cEHzbURrWbfp1fIqdVipilzj+lfaadNZmg==",
      "license": "MIT",
      "funding": {
        "type": "opencollective",
        "url": "https://opencollective.com/unified"
      }
    },
    "node_modules/esutils": {
      "version": "2.0.3",
      "resolved": "https://registry.npmjs.org/esutils/-/esutils-2.0.3.tgz",
      "integrity": "sha512-kVscqXk4OCp68SZ0dkgEKVi6/8ij300KBWTJq32P/dYeWTSwK41WyTxalN1eRmA5Z9UU/LX9D7FWSmV9SAYx6g==",
      "dev": true,
      "license": "BSD-2-Clause",
      "engines": {
        "node": ">=0.10.0"
      }
    },
    "node_modules/eventemitter3": {
      "version": "2.0.3",
      "resolved": "https://registry.npmjs.org/eventemitter3/-/eventemitter3-2.0.3.tgz",
      "integrity": "sha512-jLN68Dx5kyFHaePoXWPsCGW5qdyZQtLYHkxkg02/Mz6g0kYpDx4FyP6XfArhQdlOC4b8Mv+EMxPo/8La7Tzghg==",
      "license": "MIT"
    },
    "node_modules/extend": {
      "version": "3.0.2",
      "resolved": "https://registry.npmjs.org/extend/-/extend-3.0.2.tgz",
      "integrity": "sha512-fjquC59cD7CyW6urNXK0FBufkZcoiGG80wTuPujX590cB5Ttln20E2UB4S/WARVqhXffZl2LNgS+gQdPIIim/g==",
      "license": "MIT"
    },
    "node_modules/fast-deep-equal": {
      "version": "3.1.3",
      "resolved": "https://registry.npmjs.org/fast-deep-equal/-/fast-deep-equal-3.1.3.tgz",
      "integrity": "sha512-f3qQ9oQy9j2AhBe/H9VC91wLmKBCCU/gDOnKNAYG5hswO7BLKj09Hc5HYNz9cGI++xlpDCIgDaitVs03ATR84Q==",
      "dev": true,
      "license": "MIT"
    },
    "node_modules/fast-diff": {
      "version": "1.1.2",
      "resolved": "https://registry.npmjs.org/fast-diff/-/fast-diff-1.1.2.tgz",
      "integrity": "sha512-KaJUt+M9t1qaIteSvjc6P3RbMdXsNhK61GRftR6SNxqmhthcd9MGIi4T+o0jD8LUSpSnSKXE20nLtJ3fOHxQig==",
      "license": "Apache-2.0"
    },
    "node_modules/fast-equals": {
      "version": "5.4.0",
      "resolved": "https://registry.npmjs.org/fast-equals/-/fast-equals-5.4.0.tgz",
      "integrity": "sha512-jt2DW/aNFNwke7AUd+Z+e6pz39KO5rzdbbFCg2sGafS4mk13MI7Z8O5z9cADNn5lhGODIgLwug6TZO2ctf7kcw==",
      "license": "MIT",
      "engines": {
        "node": ">=6.0.0"
      }
    },
    "node_modules/fast-glob": {
      "version": "3.3.3",
      "resolved": "https://registry.npmjs.org/fast-glob/-/fast-glob-3.3.3.tgz",
      "integrity": "sha512-7MptL8U0cqcFdzIzwOTHoilX9x5BrNqye7Z/LuC7kCMRio1EMSyqRK3BEAUD7sXRq4iT4AzTVuZdhgQ2TCvYLg==",
      "license": "MIT",
      "dependencies": {
        "@nodelib/fs.stat": "^2.0.2",
        "@nodelib/fs.walk": "^1.2.3",
        "glob-parent": "^5.1.2",
        "merge2": "^1.3.0",
        "micromatch": "^4.0.8"
      },
      "engines": {
        "node": ">=8.6.0"
      }
    },
    "node_modules/fast-glob/node_modules/glob-parent": {
      "version": "5.1.2",
      "resolved": "https://registry.npmjs.org/glob-parent/-/glob-parent-5.1.2.tgz",
      "integrity": "sha512-AOIgSQCepiJYwP3ARnGx+5VnTu2HBYdzbGP45eLw1vr3zB3vZLeyed1sC9hnbcOc9/SrMyM5RPQrkGz4aS9Zow==",
      "license": "ISC",
      "dependencies": {
        "is-glob": "^4.0.1"
      },
      "engines": {
        "node": ">= 6"
      }
    },
    "node_modules/fast-json-stable-stringify": {
      "version": "2.1.0",
      "resolved": "https://registry.npmjs.org/fast-json-stable-stringify/-/fast-json-stable-stringify-2.1.0.tgz",
      "integrity": "sha512-lhd/wF+Lk98HZoTCtlVraHtfh5XYijIjalXck7saUtuanSDyLMxnHhSXEDJqHxD7msR8D0uCmqlkwjCV8xvwHw==",
      "dev": true,
      "license": "MIT"
    },
    "node_modules/fast-levenshtein": {
      "version": "2.0.6",
      "resolved": "https://registry.npmjs.org/fast-levenshtein/-/fast-levenshtein-2.0.6.tgz",
      "integrity": "sha512-DCXu6Ifhqcks7TZKY3Hxp3y6qphY5SJZmrWMDrKcERSOXWQdMhU9Ig/PYrzyw/ul9jOIyh0N4M0tbC5hodg8dw==",
      "dev": true,
      "license": "MIT"
    },
    "node_modules/fast-png": {
      "version": "6.4.0",
      "resolved": "https://registry.npmjs.org/fast-png/-/fast-png-6.4.0.tgz",
      "integrity": "sha512-kAqZq1TlgBjZcLr5mcN6NP5Rv4V2f22z00c3g8vRrwkcqjerx7BEhPbOnWCPqaHUl2XWQBJQvOT/FQhdMT7X/Q==",
      "license": "MIT",
      "dependencies": {
        "@types/pako": "^2.0.3",
        "iobuffer": "^5.3.2",
        "pako": "^2.1.0"
      }
    },
    "node_modules/fastq": {
      "version": "1.20.1",
      "resolved": "https://registry.npmjs.org/fastq/-/fastq-1.20.1.tgz",
      "integrity": "sha512-GGToxJ/w1x32s/D2EKND7kTil4n8OVk/9mycTc4VDza13lOvpUZTGX3mFSCtV9ksdGBVzvsyAVLM6mHFThxXxw==",
      "license": "ISC",
      "dependencies": {
        "reusify": "^1.0.4"
      }
    },
    "node_modules/fflate": {
      "version": "0.8.2",
      "resolved": "https://registry.npmjs.org/fflate/-/fflate-0.8.2.tgz",
      "integrity": "sha512-cPJU47OaAoCbg0pBvzsgpTPhmhqI5eJjh/JIu8tPj5q+T7iLvW/JAYUqmE7KOB4R1ZyEhzBaIQpQpardBF5z8A==",
      "license": "MIT"
    },
    "node_modules/file-entry-cache": {
      "version": "8.0.0",
      "resolved": "https://registry.npmjs.org/file-entry-cache/-/file-entry-cache-8.0.0.tgz",
      "integrity": "sha512-XXTUwCvisa5oacNGRP9SfNtYBNAMi+RPwBFmblZEF7N7swHYQS6/Zfk7SRwx4D5j3CH211YNRco1DEMNVfZCnQ==",
      "dev": true,
      "license": "MIT",
      "dependencies": {
        "flat-cache": "^4.0.0"
      },
      "engines": {
        "node": ">=16.0.0"
      }
    },
    "node_modules/fill-range": {
      "version": "7.1.1",
      "resolved": "https://registry.npmjs.org/fill-range/-/fill-range-7.1.1.tgz",
      "integrity": "sha512-YsGpe3WHLK8ZYi4tWDg2Jy3ebRz2rXowDxnld4bkQB00cc/1Zw9AWnC0i9ztDJitivtQvaI9KaLyKrc+hBW0yg==",
      "license": "MIT",
      "dependencies": {
        "to-regex-range": "^5.0.1"
      },
      "engines": {
        "node": ">=8"
      }
    },
    "node_modules/find-up": {
      "version": "5.0.0",
      "resolved": "https://registry.npmjs.org/find-up/-/find-up-5.0.0.tgz",
      "integrity": "sha512-78/PXT1wlLLDgTzDs7sjq9hzz0vXD+zn+7wypEe4fXQxCmdmqfGsEPQxmiCSQI3ajFV91bVSsvNtrJRiW6nGng==",
      "dev": true,
      "license": "MIT",
      "dependencies": {
        "locate-path": "^6.0.0",
        "path-exists": "^4.0.0"
      },
      "engines": {
        "node": ">=10"
      },
      "funding": {
        "url": "https://github.com/sponsors/sindresorhus"
      }
    },
    "node_modules/flat-cache": {
      "version": "4.0.1",
      "resolved": "https://registry.npmjs.org/flat-cache/-/flat-cache-4.0.1.tgz",
      "integrity": "sha512-f7ccFPK3SXFHpx15UIGyRJ/FJQctuKZ0zVuN3frBo4HnK3cay9VEW0R6yPYFHC0AgqhukPzKjq22t5DmAyqGyw==",
      "dev": true,
      "license": "MIT",
      "dependencies": {
        "flatted": "^3.2.9",
        "keyv": "^4.5.4"
      },
      "engines": {
        "node": ">=16"
      }
    },
    "node_modules/flatted": {
      "version": "3.4.2",
      "resolved": "https://registry.npmjs.org/flatted/-/flatted-3.4.2.tgz",
      "integrity": "sha512-PjDse7RzhcPkIJwy5t7KPWQSZ9cAbzQXcafsetQoD7sOJRQlGikNbx7yZp2OotDnJyrDcbyRq3Ttb18iYOqkxA==",
      "dev": true,
      "license": "ISC"
    },
    "node_modules/follow-redirects": {
      "version": "1.16.0",
      "resolved": "https://registry.npmjs.org/follow-redirects/-/follow-redirects-1.16.0.tgz",
      "integrity": "sha512-y5rN/uOsadFT/JfYwhxRS5R7Qce+g3zG97+JrtFZlC9klX/W5hD7iiLzScI4nZqUS7DNUdhPgw4xI8W2LuXlUw==",
      "funding": [
        {
          "type": "individual",
          "url": "https://github.com/sponsors/RubenVerborgh"
        }
      ],
      "license": "MIT",
      "engines": {
        "node": ">=4.0"
      },
      "peerDependenciesMeta": {
        "debug": {
          "optional": true
        }
      }
    },
    "node_modules/for-each": {
      "version": "0.3.5",
      "resolved": "https://registry.npmjs.org/for-each/-/for-each-0.3.5.tgz",
      "integrity": "sha512-dKx12eRCVIzqCxFGplyFKJMPvLEWgmNtUrpTiJIR5u97zEhRG8ySrtboPHZXx7daLxQVrl643cTzbab2tkQjxg==",
      "dev": true,
      "license": "MIT",
      "dependencies": {
        "is-callable": "^1.2.7"
      },
      "engines": {
        "node": ">= 0.4"
      },
      "funding": {
        "url": "https://github.com/sponsors/ljharb"
      }
    },
    "node_modules/form-data": {
      "version": "4.0.6",
      "resolved": "https://registry.npmjs.org/form-data/-/form-data-4.0.6.tgz",
      "integrity": "sha512-vKatAh4SlVfgbv+YtmhiRjhEMJsYpsG1Y2rMQtR+SVSbytsSD1YGzDIcrAJmdFec88u/+VoGmxnl+80gL1tRCQ==",
      "license": "MIT",
      "dependencies": {
        "asynckit": "^0.4.0",
        "combined-stream": "^1.0.8",
        "es-set-tostringtag": "^2.1.0",
        "hasown": "^2.0.4",
        "mime-types": "^2.1.35"
      },
      "engines": {
        "node": ">= 6"
      }
    },
    "node_modules/fraction.js": {
      "version": "5.3.4",
      "resolved": "https://registry.npmjs.org/fraction.js/-/fraction.js-5.3.4.tgz",
      "integrity": "sha512-1X1NTtiJphryn/uLQz3whtY6jK3fTqoE3ohKs0tT+Ujr1W59oopxmoEh7Lu5p6vBaPbgoM0bzveAW4Qi5RyWDQ==",
      "dev": true,
      "license": "MIT",
      "engines": {
        "node": "*"
      },
      "funding": {
        "type": "github",
        "url": "https://github.com/sponsors/rawify"
      }
    },
    "node_modules/framer-motion": {
      "version": "11.18.2",
      "resolved": "https://registry.npmjs.org/framer-motion/-/framer-motion-11.18.2.tgz",
      "integrity": "sha512-5F5Och7wrvtLVElIpclDT0CBzMVg3dL22B64aZwHtsIY8RB4mXICLrkajK4G9R+ieSAGcgrLeae2SeUTg2pr6w==",
      "license": "MIT",
      "dependencies": {
        "motion-dom": "^11.18.1",
        "motion-utils": "^11.18.1",
        "tslib": "^2.4.0"
      },
      "peerDependencies": {
        "@emotion/is-prop-valid": "*",
        "react": "^18.0.0 || ^19.0.0",
        "react-dom": "^18.0.0 || ^19.0.0"
      },
      "peerDependenciesMeta": {
        "@emotion/is-prop-valid": {
          "optional": true
        },
        "react": {
          "optional": true
        },
        "react-dom": {
          "optional": true
        }
      }
    },
    "node_modules/fsevents": {
      "version": "2.3.3",
      "resolved": "https://registry.npmjs.org/fsevents/-/fsevents-2.3.3.tgz",
      "integrity": "sha512-5xoDfX+fL7faATnagmWPpbFtwh/R77WmMMqqHGS65C3vvB0YHrgF+B1YmZ3441tMj5n63k0212XNoJwzlhffQw==",
      "hasInstallScript": true,
      "license": "MIT",
      "optional": true,
      "os": [
        "darwin"
      ],
      "engines": {
        "node": "^8.16.0 || ^10.6.0 || >=11.0.0"
      }
    },
    "node_modules/function-bind": {
      "version": "1.1.2",
      "resolved": "https://registry.npmjs.org/function-bind/-/function-bind-1.1.2.tgz",
      "integrity": "sha512-7XHNxH7qX9xG5mIwxkhumTox/MIRNcOgDrxWsMt2pAr23WHp6MrRlN7FBSFpCpr+oVO0F744iUgR82nJMfG2SA==",
      "license": "MIT",
      "funding": {
        "url": "https://github.com/sponsors/ljharb"
      }
    },
    "node_modules/function.prototype.name": {
      "version": "1.1.8",
      "resolved": "https://registry.npmjs.org/function.prototype.name/-/function.prototype.name-1.1.8.tgz",
      "integrity": "sha512-e5iwyodOHhbMr/yNrc7fDYG4qlbIvI5gajyzPnb5TCwyhjApznQh1BMFou9b30SevY43gCJKXycoCBjMbsuW0Q==",
      "dev": true,
      "license": "MIT",
      "dependencies": {
        "call-bind": "^1.0.8",
        "call-bound": "^1.0.3",
        "define-properties": "^1.2.1",
        "functions-have-names": "^1.2.3",
        "hasown": "^2.0.2",
        "is-callable": "^1.2.7"
      },
      "engines": {
        "node": ">= 0.4"
      },
      "funding": {
        "url": "https://github.com/sponsors/ljharb"
      }
    },
    "node_modules/functions-have-names": {
      "version": "1.2.3",
      "resolved": "https://registry.npmjs.org/functions-have-names/-/functions-have-names-1.2.3.tgz",
      "integrity": "sha512-xckBUXyTIqT97tq2x2AMb+g163b5JFysYk0x4qxNFwbfQkmNZoiRHb6sPzI9/QV33WeuvVYBUIiD4NzNIyqaRQ==",
      "license": "MIT",
      "funding": {
        "url": "https://github.com/sponsors/ljharb"
      }
    },
    "node_modules/generator-function": {
      "version": "2.0.1",
      "resolved": "https://registry.npmjs.org/generator-function/-/generator-function-2.0.1.tgz",
      "integrity": "sha512-SFdFmIJi+ybC0vjlHN0ZGVGHc3lgE0DxPAT0djjVg+kjOnSqclqmj0KQ7ykTOLP6YxoqOvuAODGdcHJn+43q3g==",
      "dev": true,
      "license": "MIT",
      "engines": {
        "node": ">= 0.4"
      }
    },
    "node_modules/gensync": {
      "version": "1.0.0-beta.2",
      "resolved": "https://registry.npmjs.org/gensync/-/gensync-1.0.0-beta.2.tgz",
      "integrity": "sha512-3hN7NaskYvMDLQY55gnW3NQ+mesEAepTqlg+VEbj7zzqEMBVNhzcGYYeqFo/TlYz6eQiFcp1HcsCZO+nGgS8zg==",
      "dev": true,
      "license": "MIT",
      "engines": {
        "node": ">=6.9.0"
      }
    },
    "node_modules/get-intrinsic": {
      "version": "1.3.0",
      "resolved": "https://registry.npmjs.org/get-intrinsic/-/get-intrinsic-1.3.0.tgz",
      "integrity": "sha512-9fSjSaos/fRIVIp+xSJlE6lfwhES7LNtKaCBIamHsjr2na1BiABJPo0mOjjz8GJDURarmCPGqaiVg5mfjb98CQ==",
      "license": "MIT",
      "dependencies": {
        "call-bind-apply-helpers": "^1.0.2",
        "es-define-property": "^1.0.1",
        "es-errors": "^1.3.0",
        "es-object-atoms": "^1.1.1",
        "function-bind": "^1.1.2",
        "get-proto": "^1.0.1",
        "gopd": "^1.2.0",
        "has-symbols": "^1.1.0",
        "hasown": "^2.0.2",
        "math-intrinsics": "^1.1.0"
      },
      "engines": {
        "node": ">= 0.4"
      },
      "funding": {
        "url": "https://github.com/sponsors/ljharb"
      }
    },
    "node_modules/get-nonce": {
      "version": "1.0.1",
      "resolved": "https://registry.npmjs.org/get-nonce/-/get-nonce-1.0.1.tgz",
      "integrity": "sha512-FJhYRoDaiatfEkUK8HKlicmu/3SGFD51q3itKDGoSTysQJBnfOcxU5GxnhE1E6soB76MbT0MBtnKJuXyAx+96Q==",
      "license": "MIT",
      "engines": {
        "node": ">=6"
      }
    },
    "node_modules/get-proto": {
      "version": "1.0.1",
      "resolved": "https://registry.npmjs.org/get-proto/-/get-proto-1.0.1.tgz",
      "integrity": "sha512-sTSfBjoXBp89JvIKIefqw7U2CCebsc74kiY6awiGogKtoSGbgjYE/G/+l9sF3MWFPNc9IcoOC4ODfKHfxFmp0g==",
      "license": "MIT",
      "dependencies": {
        "dunder-proto": "^1.0.1",
        "es-object-atoms": "^1.0.0"
      },
      "engines": {
        "node": ">= 0.4"
      }
    },
    "node_modules/get-symbol-description": {
      "version": "1.1.0",
      "resolved": "https://registry.npmjs.org/get-symbol-description/-/get-symbol-description-1.1.0.tgz",
      "integrity": "sha512-w9UMqWwJxHNOvoNzSJ2oPF5wvYcvP7jUvYzhp67yEhTi17ZDBBC1z9pTdGuzjD+EFIqLSYRweZjqfiPzQ06Ebg==",
      "dev": true,
      "license": "MIT",
      "dependencies": {
        "call-bound": "^1.0.3",
        "es-errors": "^1.3.0",
        "get-intrinsic": "^1.2.6"
      },
      "engines": {
        "node": ">= 0.4"
      },
      "funding": {
        "url": "https://github.com/sponsors/ljharb"
      }
    },
    "node_modules/glob-parent": {
      "version": "6.0.2",
      "resolved": "https://registry.npmjs.org/glob-parent/-/glob-parent-6.0.2.tgz",
      "integrity": "sha512-XxwI8EOhVQgWp6iDL+3b0r86f4d6AX6zSU55HfB4ydCEuXLXc5FcYeOu+nnGftS4TEju/11rt4KJPTMgbfmv4A==",
      "license": "ISC",
      "dependencies": {
        "is-glob": "^4.0.3"
      },
      "engines": {
        "node": ">=10.13.0"
      }
    },
    "node_modules/globals": {
      "version": "15.15.0",
      "resolved": "https://registry.npmjs.org/globals/-/globals-15.15.0.tgz",
      "integrity": "sha512-7ACyT3wmyp3I61S4fG682L0VA2RGD9otkqGJIwNUMF1SWUombIIk+af1unuDYgMm082aHYwD+mzJvv9Iu8dsgg==",
      "dev": true,
      "license": "MIT",
      "engines": {
        "node": ">=18"
      },
      "funding": {
        "url": "https://github.com/sponsors/sindresorhus"
      }
    },
    "node_modules/globalthis": {
      "version": "1.0.4",
      "resolved": "https://registry.npmjs.org/globalthis/-/globalthis-1.0.4.tgz",
      "integrity": "sha512-DpLKbNU4WylpxJykQujfCcwYWiV/Jhm50Goo0wrVILAv5jOr9d+H+UR3PhSCD2rCCEIg0uc+G+muBTwD54JhDQ==",
      "dev": true,
      "license": "MIT",
      "dependencies": {
        "define-properties": "^1.2.1",
        "gopd": "^1.0.1"
      },
      "engines": {
        "node": ">= 0.4"
      },
      "funding": {
        "url": "https://github.com/sponsors/ljharb"
      }
    },
    "node_modules/goober": {
      "version": "2.1.18",
      "resolved": "https://registry.npmjs.org/goober/-/goober-2.1.18.tgz",
      "integrity": "sha512-2vFqsaDVIT9Gz7N6kAL++pLpp41l3PfDuusHcjnGLfR6+huZkl6ziX+zgVC3ZxpqWhzH6pyDdGrCeDhMIvwaxw==",
      "license": "MIT",
      "peerDependencies": {
        "csstype": "^3.0.10"
      }
    },
    "node_modules/gopd": {
      "version": "1.2.0",
      "resolved": "https://registry.npmjs.org/gopd/-/gopd-1.2.0.tgz",
      "integrity": "sha512-ZUKRh6/kUFoAiTAtTYPZJ3hw9wNxx+BIBOijnlG9PnrJsCcSjs1wyyD6vJpaYtgnzDrKYRSqf3OO6Rfa93xsRg==",
      "license": "MIT",
      "engines": {
        "node": ">= 0.4"
      },
      "funding": {
        "url": "https://github.com/sponsors/ljharb"
      }
    },
    "node_modules/has-bigints": {
      "version": "1.1.0",
      "resolved": "https://registry.npmjs.org/has-bigints/-/has-bigints-1.1.0.tgz",
      "integrity": "sha512-R3pbpkcIqv2Pm3dUwgjclDRVmWpTJW2DcMzcIhEXEx1oh/CEMObMm3KLmRJOdvhM7o4uQBnwr8pzRK2sJWIqfg==",
      "dev": true,
      "license": "MIT",
      "engines": {
        "node": ">= 0.4"
      },
      "funding": {
        "url": "https://github.com/sponsors/ljharb"
      }
    },
    "node_modules/has-flag": {
      "version": "4.0.0",
      "resolved": "https://registry.npmjs.org/has-flag/-/has-flag-4.0.0.tgz",
      "integrity": "sha512-EykJT/Q1KjTWctppgIAgfSO0tKVuZUjhgMr17kqTumMl6Afv3EISleU7qZUzoXDFTAHTDC4NOoG/ZxU3EvlMPQ==",
      "dev": true,
      "license": "MIT",
      "engines": {
        "node": ">=8"
      }
    },
    "node_modules/has-property-descriptors": {
      "version": "1.0.2",
      "resolved": "https://registry.npmjs.org/has-property-descriptors/-/has-property-descriptors-1.0.2.tgz",
      "integrity": "sha512-55JNKuIW+vq4Ke1BjOTjM2YctQIvCT7GFzHwmfZPGo5wnrgkid0YQtnAleFSqumZm4az3n2BS+erby5ipJdgrg==",
      "license": "MIT",
      "dependencies": {
        "es-define-property": "^1.0.0"
      },
      "funding": {
        "url": "https://github.com/sponsors/ljharb"
      }
    },
    "node_modules/has-proto": {
      "version": "1.2.0",
      "resolved": "https://registry.npmjs.org/has-proto/-/has-proto-1.2.0.tgz",
      "integrity": "sha512-KIL7eQPfHQRC8+XluaIw7BHUwwqL19bQn4hzNgdr+1wXoU0KKj6rufu47lhY7KbJR2C6T6+PfyN0Ea7wkSS+qQ==",
      "dev": true,
      "license": "MIT",
      "dependencies": {
        "dunder-proto": "^1.0.0"
      },
      "engines": {
        "node": ">= 0.4"
      },
      "funding": {
        "url": "https://github.com/sponsors/ljharb"
      }
    },
    "node_modules/has-symbols": {
      "version": "1.1.0",
      "resolved": "https://registry.npmjs.org/has-symbols/-/has-symbols-1.1.0.tgz",
      "integrity": "sha512-1cDNdwJ2Jaohmb3sg4OmKaMBwuC48sYni5HUw2DvsC8LjGTLK9h+eb1X6RyuOHe4hT0ULCW68iomhjUoKUqlPQ==",
      "license": "MIT",
      "engines": {
        "node": ">= 0.4"
      },
      "funding": {
        "url": "https://github.com/sponsors/ljharb"
      }
    },
    "node_modules/has-tostringtag": {
      "version": "1.0.2",
      "resolved": "https://registry.npmjs.org/has-tostringtag/-/has-tostringtag-1.0.2.tgz",
      "integrity": "sha512-NqADB8VjPFLM2V0VvHUewwwsw0ZWBaIdgo+ieHtK3hasLz4qeCRjYcqfB6AQrBggRKppKF8L52/VqdVsO47Dlw==",
      "license": "MIT",
      "dependencies": {
        "has-symbols": "^1.0.3"
      },
      "engines": {
        "node": ">= 0.4"
      },
      "funding": {
        "url": "https://github.com/sponsors/ljharb"
      }
    },
    "node_modules/hasown": {
      "version": "2.0.4",
      "resolved": "https://registry.npmjs.org/hasown/-/hasown-2.0.4.tgz",
      "integrity": "sha512-T2UbfbBEF32wiepXIsMlTW9+dDYC6wMh/t/vYA4tuOMKqWz/n3vr1NFSxQiyP+zk2mXsoMA/i/7qV6LKut1t1A==",
      "license": "MIT",
      "dependencies": {
        "function-bind": "^1.1.2"
      },
      "engines": {
        "node": ">= 0.4"
      }
    },
    "node_modules/hast-util-to-jsx-runtime": {
      "version": "2.3.6",
      "resolved": "https://registry.npmjs.org/hast-util-to-jsx-runtime/-/hast-util-to-jsx-runtime-2.3.6.tgz",
      "integrity": "sha512-zl6s8LwNyo1P9uw+XJGvZtdFF1GdAkOg8ujOw+4Pyb76874fLps4ueHXDhXWdk6YHQ6OgUtinliG7RsYvCbbBg==",
      "license": "MIT",
      "dependencies": {
        "@types/estree": "^1.0.0",
        "@types/hast": "^3.0.0",
        "@types/unist": "^3.0.0",
        "comma-separated-tokens": "^2.0.0",
        "devlop": "^1.0.0",
        "estree-util-is-identifier-name": "^3.0.0",
        "hast-util-whitespace": "^3.0.0",
        "mdast-util-mdx-expression": "^2.0.0",
        "mdast-util-mdx-jsx": "^3.0.0",
        "mdast-util-mdxjs-esm": "^2.0.0",
        "property-information": "^7.0.0",
        "space-separated-tokens": "^2.0.0",
        "style-to-js": "^1.0.0",
        "unist-util-position": "^5.0.0",
        "vfile-message": "^4.0.0"
      },
      "funding": {
        "type": "opencollective",
        "url": "https://opencollective.com/unified"
      }
    },
    "node_modules/hast-util-whitespace": {
      "version": "3.0.0",
      "resolved": "https://registry.npmjs.org/hast-util-whitespace/-/hast-util-whitespace-3.0.0.tgz",
      "integrity": "sha512-88JUN06ipLwsnv+dVn+OIYOvAuvBMy/Qoi6O7mQHxdPXpjy+Cd6xRkWwux7DKO+4sYILtLBRIKgsdpS2gQc7qw==",
      "license": "MIT",
      "dependencies": {
        "@types/hast": "^3.0.0"
      },
      "funding": {
        "type": "opencollective",
        "url": "https://opencollective.com/unified"
      }
    },
    "node_modules/html-url-attributes": {
      "version": "3.0.1",
      "resolved": "https://registry.npmjs.org/html-url-attributes/-/html-url-attributes-3.0.1.tgz",
      "integrity": "sha512-ol6UPyBWqsrO6EJySPz2O7ZSr856WDrEzM5zMqp+FJJLGMW35cLYmmZnl0vztAZxRUoNZJFTCohfjuIJ8I4QBQ==",
      "license": "MIT",
      "funding": {
        "type": "opencollective",
        "url": "https://opencollective.com/unified"
      }
    },
    "node_modules/html2canvas": {
      "version": "1.4.1",
      "resolved": "https://registry.npmjs.org/html2canvas/-/html2canvas-1.4.1.tgz",
      "integrity": "sha512-fPU6BHNpsyIhr8yyMpTLLxAbkaK8ArIBcmZIRiBLiDhjeqvXolaEmDGmELFuX9I4xDcaKKcJl+TKZLqruBbmWA==",
      "license": "MIT",
      "dependencies": {
        "css-line-break": "^2.1.0",
        "text-segmentation": "^1.0.3"
      },
      "engines": {
        "node": ">=8.0.0"
      }
    },
    "node_modules/https-proxy-agent": {
      "version": "5.0.1",
      "resolved": "https://registry.npmjs.org/https-proxy-agent/-/https-proxy-agent-5.0.1.tgz",
      "integrity": "sha512-dFcAjpTQFgoLMzC2VwU+C/CbS7uRL0lWmxDITmqm7C+7F0Odmj6s9l6alZc6AELXhrnggM2CeWSXHGOdX2YtwA==",
      "license": "MIT",
      "dependencies": {
        "agent-base": "6",
        "debug": "4"
      },
      "engines": {
        "node": ">= 6"
      }
    },
    "node_modules/ignore": {
      "version": "5.3.2",
      "resolved": "https://registry.npmjs.org/ignore/-/ignore-5.3.2.tgz",
      "integrity": "sha512-hsBTNUqQTDwkWtcdYI2i06Y/nUBEsNEDJKjWdigLvegy8kDuJAS8uRlpkkcQpyEXL0Z/pjDy5HBmMjRCJ2gq+g==",
      "dev": true,
      "license": "MIT",
      "engines": {
        "node": ">= 4"
      }
    },
    "node_modules/import-fresh": {
      "version": "3.3.1",
      "resolved": "https://registry.npmjs.org/import-fresh/-/import-fresh-3.3.1.tgz",
      "integrity": "sha512-TR3KfrTZTYLPB6jUjfx6MF9WcWrHL9su5TObK4ZkYgBdWKPOFoSoQIdEuTuR82pmtxH2spWG9h6etwfr1pLBqQ==",
      "dev": true,
      "license": "MIT",
      "dependencies": {
        "parent-module": "^1.0.0",
        "resolve-from": "^4.0.0"
      },
      "engines": {
        "node": ">=6"
      },
      "funding": {
        "url": "https://github.com/sponsors/sindresorhus"
      }
    },
    "node_modules/imurmurhash": {
      "version": "0.1.4",
      "resolved": "https://registry.npmjs.org/imurmurhash/-/imurmurhash-0.1.4.tgz",
      "integrity": "sha512-JmXMZ6wuvDmLiHEml9ykzqO6lwFbof0GG4IkcGaENdCRDDmMVnny7s5HsIgHCbaq0w2MyPhDqkhTUgS2LU2PHA==",
      "dev": true,
      "license": "MIT",
      "engines": {
        "node": ">=0.8.19"
      }
    },
    "node_modules/inline-style-parser": {
      "version": "0.2.7",
      "resolved": "https://registry.npmjs.org/inline-style-parser/-/inline-style-parser-0.2.7.tgz",
      "integrity": "sha512-Nb2ctOyNR8DqQoR0OwRG95uNWIC0C1lCgf5Naz5H6Ji72KZ8OcFZLz2P5sNgwlyoJ8Yif11oMuYs5pBQa86csA==",
      "license": "MIT"
    },
    "node_modules/input-otp": {
      "version": "1.4.2",
      "resolved": "https://registry.npmjs.org/input-otp/-/input-otp-1.4.2.tgz",
      "integrity": "sha512-l3jWwYNvrEa6NTCt7BECfCm48GvwuZzkoeG3gBL2w4CHeOXW3eKFmf9UNYkNfYc3mxMrthMnxjIE07MT0zLBQA==",
      "license": "MIT",
      "peerDependencies": {
        "react": "^16.8 || ^17.0 || ^18.0 || ^19.0.0 || ^19.0.0-rc",
        "react-dom": "^16.8 || ^17.0 || ^18.0 || ^19.0.0 || ^19.0.0-rc"
      }
    },
    "node_modules/internal-slot": {
      "version": "1.1.0",
      "resolved": "https://registry.npmjs.org/internal-slot/-/internal-slot-1.1.0.tgz",
      "integrity": "sha512-4gd7VpWNQNB4UKKCFFVcp1AVv+FMOgs9NKzjHKusc8jTMhd5eL1NqQqOpE0KzMds804/yHlglp3uxgluOqAPLw==",
      "dev": true,
      "license": "MIT",
      "dependencies": {
        "es-errors": "^1.3.0",
        "hasown": "^2.0.2",
        "side-channel": "^1.1.0"
      },
      "engines": {
        "node": ">= 0.4"
      }
    },
    "node_modules/internmap": {
      "version": "2.0.3",
      "resolved": "https://registry.npmjs.org/internmap/-/internmap-2.0.3.tgz",
      "integrity": "sha512-5Hh7Y1wQbvY5ooGgPbDaL5iYLAPzMTUrjMulskHLH6wnv/A+1q5rgEaiuqEjB+oxGXIVZs1FF+R/KPN3ZSQYYg==",
      "license": "ISC",
      "engines": {
        "node": ">=12"
      }
    },
    "node_modules/iobuffer": {
      "version": "5.4.0",
      "resolved": "https://registry.npmjs.org/iobuffer/-/iobuffer-5.4.0.tgz",
      "integrity": "sha512-DRebOWuqDvxunfkNJAlc3IzWIPD5xVxwUNbHr7xKB8E6aLJxIPfNX3CoMJghcFjpv6RWQsrcJbghtEwSPoJqMA==",
      "license": "MIT"
    },
    "node_modules/is-alphabetical": {
      "version": "2.0.1",
      "resolved": "https://registry.npmjs.org/is-alphabetical/-/is-alphabetical-2.0.1.tgz",
      "integrity": "sha512-FWyyY60MeTNyeSRpkM2Iry0G9hpr7/9kD40mD/cGQEuilcZYS4okz8SN2Q6rLCJ8gbCt6fN+rC+6tMGS99LaxQ==",
      "license": "MIT",
      "funding": {
        "type": "github",
        "url": "https://github.com/sponsors/wooorm"
      }
    },
    "node_modules/is-alphanumerical": {
      "version": "2.0.1",
      "resolved": "https://registry.npmjs.org/is-alphanumerical/-/is-alphanumerical-2.0.1.tgz",
      "integrity": "sha512-hmbYhX/9MUMF5uh7tOXyK/n0ZvWpad5caBA17GsC6vyuCqaWliRG5K1qS9inmUhEMaOBIW7/whAnSwveW/LtZw==",
      "license": "MIT",
      "dependencies": {
        "is-alphabetical": "^2.0.0",
        "is-decimal": "^2.0.0"
      },
      "funding": {
        "type": "github",
        "url": "https://github.com/sponsors/wooorm"
      }
    },
    "node_modules/is-arguments": {
      "version": "1.2.0",
      "resolved": "https://registry.npmjs.org/is-arguments/-/is-arguments-1.2.0.tgz",
      "integrity": "sha512-7bVbi0huj/wrIAOzb8U1aszg9kdi3KN/CyU19CTI7tAoZYEZoL9yCDXpbXN+uPsuWnP02cyug1gleqq+TU+YCA==",
      "license": "MIT",
      "dependencies": {
        "call-bound": "^1.0.2",
        "has-tostringtag": "^1.0.2"
      },
      "engines": {
        "node": ">= 0.4"
      },
      "funding": {
        "url": "https://github.com/sponsors/ljharb"
      }
    },
    "node_modules/is-array-buffer": {
      "version": "3.0.5",
      "resolved": "https://registry.npmjs.org/is-array-buffer/-/is-array-buffer-3.0.5.tgz",
      "integrity": "sha512-DDfANUiiG2wC1qawP66qlTugJeL5HyzMpfr8lLK+jMQirGzNod0B12cFB/9q838Ru27sBwfw78/rdoU7RERz6A==",
      "dev": true,
      "license": "MIT",
      "dependencies": {
        "call-bind": "^1.0.8",
        "call-bound": "^1.0.3",
        "get-intrinsic": "^1.2.6"
      },
      "engines": {
        "node": ">= 0.4"
      },
      "funding": {
        "url": "https://github.com/sponsors/ljharb"
      }
    },
    "node_modules/is-async-function": {
      "version": "2.1.1",
      "resolved": "https://registry.npmjs.org/is-async-function/-/is-async-function-2.1.1.tgz",
      "integrity": "sha512-9dgM/cZBnNvjzaMYHVoxxfPj2QXt22Ev7SuuPrs+xav0ukGB0S6d4ydZdEiM48kLx5kDV+QBPrpVnFyefL8kkQ==",
      "dev": true,
      "license": "MIT",
      "dependencies": {
        "async-function": "^1.0.0",
        "call-bound": "^1.0.3",
        "get-proto": "^1.0.1",
        "has-tostringtag": "^1.0.2",
        "safe-regex-test": "^1.1.0"
      },
      "engines": {
        "node": ">= 0.4"
      },
      "funding": {
        "url": "https://github.com/sponsors/ljharb"
      }
    },
    "node_modules/is-bigint": {
      "version": "1.1.0",
      "resolved": "https://registry.npmjs.org/is-bigint/-/is-bigint-1.1.0.tgz",
      "integrity": "sha512-n4ZT37wG78iz03xPRKJrHTdZbe3IicyucEtdRsV5yglwc3GyUfbAfpSeD0FJ41NbUNSt5wbhqfp1fS+BgnvDFQ==",
      "dev": true,
      "license": "MIT",
      "dependencies": {
        "has-bigints": "^1.0.2"
      },
      "engines": {
        "node": ">= 0.4"
      },
      "funding": {
        "url": "https://github.com/sponsors/ljharb"
      }
    },
    "node_modules/is-binary-path": {
      "version": "2.1.0",
      "resolved": "https://registry.npmjs.org/is-binary-path/-/is-binary-path-2.1.0.tgz",
      "integrity": "sha512-ZMERYes6pDydyuGidse7OsHxtbI7WVeUEozgR/g7rd0xUimYNlvZRE/K2MgZTjWy725IfelLeVcEM97mmtRGXw==",
      "license": "MIT",
      "dependencies": {
        "binary-extensions": "^2.0.0"
      },
      "engines": {
        "node": ">=8"
      }
    },
    "node_modules/is-boolean-object": {
      "version": "1.2.2",
      "resolved": "https://registry.npmjs.org/is-boolean-object/-/is-boolean-object-1.2.2.tgz",
      "integrity": "sha512-wa56o2/ElJMYqjCjGkXri7it5FbebW5usLw/nPmCMs5DeZ7eziSYZhSmPRn0txqeW4LnAmQQU7FgqLpsEFKM4A==",
      "dev": true,
      "license": "MIT",
      "dependencies": {
        "call-bound": "^1.0.3",
        "has-tostringtag": "^1.0.2"
      },
      "engines": {
        "node": ">= 0.4"
      },
      "funding": {
        "url": "https://github.com/sponsors/ljharb"
      }
    },
    "node_modules/is-callable": {
      "version": "1.2.7",
      "resolved": "https://registry.npmjs.org/is-callable/-/is-callable-1.2.7.tgz",
      "integrity": "sha512-1BC0BVFhS/p0qtw6enp8e+8OD0UrK0oFLztSjNzhcKA3WDuJxxAPXzPuPtKkjEY9UUoEWlX/8fgKeu2S8i9JTA==",
      "dev": true,
      "license": "MIT",
      "engines": {
        "node": ">= 0.4"
      },
      "funding": {
        "url": "https://github.com/sponsors/ljharb"
      }
    },
    "node_modules/is-core-module": {
      "version": "2.16.1",
      "resolved": "https://registry.npmjs.org/is-core-module/-/is-core-module-2.16.1.tgz",
      "integrity": "sha512-UfoeMA6fIJ8wTYFEUjelnaGI67v6+N7qXJEvQuIGa99l4xsCruSYOVSQ0uPANn4dAzm8lkYPaKLrrijLq7x23w==",
      "license": "MIT",
      "dependencies": {
        "hasown": "^2.0.2"
      },
      "engines": {
        "node": ">= 0.4"
      },
      "funding": {
        "url": "https://github.com/sponsors/ljharb"
      }
    },
    "node_modules/is-data-view": {
      "version": "1.0.2",
      "resolved": "https://registry.npmjs.org/is-data-view/-/is-data-view-1.0.2.tgz",
      "integrity": "sha512-RKtWF8pGmS87i2D6gqQu/l7EYRlVdfzemCJN/P3UOs//x1QE7mfhvzHIApBTRf7axvT6DMGwSwBXYCT0nfB9xw==",
      "dev": true,
      "license": "MIT",
      "dependencies": {
        "call-bound": "^1.0.2",
        "get-intrinsic": "^1.2.6",
        "is-typed-array": "^1.1.13"
      },
      "engines": {
        "node": ">= 0.4"
      },
      "funding": {
        "url": "https://github.com/sponsors/ljharb"
      }
    },
    "node_modules/is-date-object": {
      "version": "1.1.0",
      "resolved": "https://registry.npmjs.org/is-date-object/-/is-date-object-1.1.0.tgz",
      "integrity": "sha512-PwwhEakHVKTdRNVOw+/Gyh0+MzlCl4R6qKvkhuvLtPMggI1WAHt9sOwZxQLSGpUaDnrdyDsomoRgNnCfKNSXXg==",
      "license": "MIT",
      "dependencies": {
        "call-bound": "^1.0.2",
        "has-tostringtag": "^1.0.2"
      },
      "engines": {
        "node": ">= 0.4"
      },
      "funding": {
        "url": "https://github.com/sponsors/ljharb"
      }
    },
    "node_modules/is-decimal": {
      "version": "2.0.1",
      "resolved": "https://registry.npmjs.org/is-decimal/-/is-decimal-2.0.1.tgz",
      "integrity": "sha512-AAB9hiomQs5DXWcRB1rqsxGUstbRroFOPPVAomNk/3XHR5JyEZChOyTWe2oayKnsSsr/kcGqF+z6yuH6HHpN0A==",
      "license": "MIT",
      "funding": {
        "type": "github",
        "url": "https://github.com/sponsors/wooorm"
      }
    },
    "node_modules/is-extglob": {
      "version": "2.1.1",
      "resolved": "https://registry.npmjs.org/is-extglob/-/is-extglob-2.1.1.tgz",
      "integrity": "sha512-SbKbANkN603Vi4jEZv49LeVJMn4yGwsbzZworEoyEiutsN3nJYdbO36zfhGJ6QEDpOZIFkDtnq5JRxmvl3jsoQ==",
      "license": "MIT",
      "engines": {
        "node": ">=0.10.0"
      }
    },
    "node_modules/is-finalizationregistry": {
      "version": "1.1.1",
      "resolved": "https://registry.npmjs.org/is-finalizationregistry/-/is-finalizationregistry-1.1.1.tgz",
      "integrity": "sha512-1pC6N8qWJbWoPtEjgcL2xyhQOP491EQjeUo3qTKcmV8YSDDJrOepfG8pcC7h/QgnQHYSv0mJ3Z/ZWxmatVrysg==",
      "dev": true,
      "license": "MIT",
      "dependencies": {
        "call-bound": "^1.0.3"
      },
      "engines": {
        "node": ">= 0.4"
      },
      "funding": {
        "url": "https://github.com/sponsors/ljharb"
      }
    },
    "node_modules/is-generator-function": {
      "version": "1.1.2",
      "resolved": "https://registry.npmjs.org/is-generator-function/-/is-generator-function-1.1.2.tgz",
      "integrity": "sha512-upqt1SkGkODW9tsGNG5mtXTXtECizwtS2kA161M+gJPc1xdb/Ax629af6YrTwcOeQHbewrPNlE5Dx7kzvXTizA==",
      "dev": true,
      "license": "MIT",
      "dependencies": {
        "call-bound": "^1.0.4",
        "generator-function": "^2.0.0",
        "get-proto": "^1.0.1",
        "has-tostringtag": "^1.0.2",
        "safe-regex-test": "^1.1.0"
      },
      "engines": {
        "node": ">= 0.4"
      },
      "funding": {
        "url": "https://github.com/sponsors/ljharb"
      }
    },
    "node_modules/is-glob": {
      "version": "4.0.3",
      "resolved": "https://registry.npmjs.org/is-glob/-/is-glob-4.0.3.tgz",
      "integrity": "sha512-xelSayHH36ZgE7ZWhli7pW34hNbNl8Ojv5KVmkJD4hBdD3th8Tfk9vYasLM+mXWOZhFkgZfxhLSnrwRr4elSSg==",
      "license": "MIT",
      "dependencies": {
        "is-extglob": "^2.1.1"
      },
      "engines": {
        "node": ">=0.10.0"
      }
    },
    "node_modules/is-hexadecimal": {
      "version": "2.0.1",
      "resolved": "https://registry.npmjs.org/is-hexadecimal/-/is-hexadecimal-2.0.1.tgz",
      "integrity": "sha512-DgZQp241c8oO6cA1SbTEWiXeoxV42vlcJxgH+B3hi1AiqqKruZR3ZGF8In3fj4+/y/7rHvlOZLZtgJ/4ttYGZg==",
      "license": "MIT",
      "funding": {
        "type": "github",
        "url": "https://github.com/sponsors/wooorm"
      }
    },
    "node_modules/is-map": {
      "version": "2.0.3",
      "resolved": "https://registry.npmjs.org/is-map/-/is-map-2.0.3.tgz",
      "integrity": "sha512-1Qed0/Hr2m+YqxnM09CjA2d/i6YZNfF6R2oRAOj36eUdS6qIV/huPJNSEpKbupewFs+ZsJlxsjjPbc0/afW6Lw==",
      "dev": true,
      "license": "MIT",
      "engines": {
        "node": ">= 0.4"
      },
      "funding": {
        "url": "https://github.com/sponsors/ljharb"
      }
    },
    "node_modules/is-negative-zero": {
      "version": "2.0.3",
      "resolved": "https://registry.npmjs.org/is-negative-zero/-/is-negative-zero-2.0.3.tgz",
      "integrity": "sha512-5KoIu2Ngpyek75jXodFvnafB6DJgr3u8uuK0LEZJjrU19DrMD3EVERaR8sjz8CCGgpZvxPl9SuE1GMVPFHx1mw==",
      "dev": true,
      "license": "MIT",
      "engines": {
        "node": ">= 0.4"
      },
      "funding": {
        "url": "https://github.com/sponsors/ljharb"
      }
    },
    "node_modules/is-number": {
      "version": "7.0.0",
      "resolved": "https://registry.npmjs.org/is-number/-/is-number-7.0.0.tgz",
      "integrity": "sha512-41Cifkg6e8TylSpdtTpeLVMqvSBEVzTttHvERD741+pnZ8ANv0004MRL43QKPDlK9cGvNp6NZWZUBlbGXYxxng==",
      "license": "MIT",
      "engines": {
        "node": ">=0.12.0"
      }
    },
    "node_modules/is-number-object": {
      "version": "1.1.1",
      "resolved": "https://registry.npmjs.org/is-number-object/-/is-number-object-1.1.1.tgz",
      "integrity": "sha512-lZhclumE1G6VYD8VHe35wFaIif+CTy5SJIi5+3y4psDgWu4wPDoBhF8NxUOinEc7pHgiTsT6MaBb92rKhhD+Xw==",
      "dev": true,
      "license": "MIT",
      "dependencies": {
        "call-bound": "^1.0.3",
        "has-tostringtag": "^1.0.2"
      },
      "engines": {
        "node": ">= 0.4"
      },
      "funding": {
        "url": "https://github.com/sponsors/ljharb"
      }
    },
    "node_modules/is-plain-obj": {
      "version": "4.1.0",
      "resolved": "https://registry.npmjs.org/is-plain-obj/-/is-plain-obj-4.1.0.tgz",
      "integrity": "sha512-+Pgi+vMuUNkJyExiMBt5IlFoMyKnr5zhJ4Uspz58WOhBF5QoIZkFyNHIbBAtHwzVAgk5RtndVNsDRN61/mmDqg==",
      "license": "MIT",
      "engines": {
        "node": ">=12"
      },
      "funding": {
        "url": "https://github.com/sponsors/sindresorhus"
      }
    },
    "node_modules/is-regex": {
      "version": "1.2.1",
      "resolved": "https://registry.npmjs.org/is-regex/-/is-regex-1.2.1.tgz",
      "integrity": "sha512-MjYsKHO5O7mCsmRGxWcLWheFqN9DJ/2TmngvjKXihe6efViPqc274+Fx/4fYj/r03+ESvBdTXK0V6tA3rgez1g==",
      "license": "MIT",
      "dependencies": {
        "call-bound": "^1.0.2",
        "gopd": "^1.2.0",
        "has-tostringtag": "^1.0.2",
        "hasown": "^2.0.2"
      },
      "engines": {
        "node": ">= 0.4"
      },
      "funding": {
        "url": "https://github.com/sponsors/ljharb"
      }
    },
    "node_modules/is-set": {
      "version": "2.0.3",
      "resolved": "https://registry.npmjs.org/is-set/-/is-set-2.0.3.tgz",
      "integrity": "sha512-iPAjerrse27/ygGLxw+EBR9agv9Y6uLeYVJMu+QNCoouJ1/1ri0mGrcWpfCqFZuzzx3WjtwxG098X+n4OuRkPg==",
      "dev": true,
      "license": "MIT",
      "engines": {
        "node": ">= 0.4"
      },
      "funding": {
        "url": "https://github.com/sponsors/ljharb"
      }
    },
    "node_modules/is-shared-array-buffer": {
      "version": "1.0.4",
      "resolved": "https://registry.npmjs.org/is-shared-array-buffer/-/is-shared-array-buffer-1.0.4.tgz",
      "integrity": "sha512-ISWac8drv4ZGfwKl5slpHG9OwPNty4jOWPRIhBpxOoD+hqITiwuipOQ2bNthAzwA3B4fIjO4Nln74N0S9byq8A==",
      "dev": true,
      "license": "MIT",
      "dependencies": {
        "call-bound": "^1.0.3"
      },
      "engines": {
        "node": ">= 0.4"
      },
      "funding": {
        "url": "https://github.com/sponsors/ljharb"
      }
    },
    "node_modules/is-string": {
      "version": "1.1.1",
      "resolved": "https://registry.npmjs.org/is-string/-/is-string-1.1.1.tgz",
      "integrity": "sha512-BtEeSsoaQjlSPBemMQIrY1MY0uM6vnS1g5fmufYOtnxLGUZM2178PKbhsk7Ffv58IX+ZtcvoGwccYsh0PglkAA==",
      "dev": true,
      "license": "MIT",
      "dependencies": {
        "call-bound": "^1.0.3",
        "has-tostringtag": "^1.0.2"
      },
      "engines": {
        "node": ">= 0.4"
      },
      "funding": {
        "url": "https://github.com/sponsors/ljharb"
      }
    },
    "node_modules/is-symbol": {
      "version": "1.1.1",
      "resolved": "https://registry.npmjs.org/is-symbol/-/is-symbol-1.1.1.tgz",
      "integrity": "sha512-9gGx6GTtCQM73BgmHQXfDmLtfjjTUDSyoxTCbp5WtoixAhfgsDirWIcVQ/IHpvI5Vgd5i/J5F7B9cN/WlVbC/w==",
      "dev": true,
      "license": "MIT",
      "dependencies": {
        "call-bound": "^1.0.2",
        "has-symbols": "^1.1.0",
        "safe-regex-test": "^1.1.0"
      },
      "engines": {
        "node": ">= 0.4"
      },
      "funding": {
        "url": "https://github.com/sponsors/ljharb"
      }
    },
    "node_modules/is-typed-array": {
      "version": "1.1.15",
      "resolved": "https://registry.npmjs.org/is-typed-array/-/is-typed-array-1.1.15.tgz",
      "integrity": "sha512-p3EcsicXjit7SaskXHs1hA91QxgTw46Fv6EFKKGS5DRFLD8yKnohjF3hxoju94b/OcMZoQukzpPpBE9uLVKzgQ==",
      "dev": true,
      "license": "MIT",
      "dependencies": {
        "which-typed-array": "^1.1.16"
      },
      "engines": {
        "node": ">= 0.4"
      },
      "funding": {
        "url": "https://github.com/sponsors/ljharb"
      }
    },
    "node_modules/is-weakmap": {
      "version": "2.0.2",
      "resolved": "https://registry.npmjs.org/is-weakmap/-/is-weakmap-2.0.2.tgz",
      "integrity": "sha512-K5pXYOm9wqY1RgjpL3YTkF39tni1XajUIkawTLUo9EZEVUFga5gSQJF8nNS7ZwJQ02y+1YCNYcMh+HIf1ZqE+w==",
      "dev": true,
      "license": "MIT",
      "engines": {
        "node": ">= 0.4"
      },
      "funding": {
        "url": "https://github.com/sponsors/ljharb"
      }
    },
    "node_modules/is-weakref": {
      "version": "1.1.1",
      "resolved": "https://registry.npmjs.org/is-weakref/-/is-weakref-1.1.1.tgz",
      "integrity": "sha512-6i9mGWSlqzNMEqpCp93KwRS1uUOodk2OJ6b+sq7ZPDSy2WuI5NFIxp/254TytR8ftefexkWn5xNiHUNpPOfSew==",
      "dev": true,
      "license": "MIT",
      "dependencies": {
        "call-bound": "^1.0.3"
      },
      "engines": {
        "node": ">= 0.4"
      },
      "funding": {
        "url": "https://github.com/sponsors/ljharb"
      }
    },
    "node_modules/is-weakset": {
      "version": "2.0.4",
      "resolved": "https://registry.npmjs.org/is-weakset/-/is-weakset-2.0.4.tgz",
      "integrity": "sha512-mfcwb6IzQyOKTs84CQMrOwW4gQcaTOAWJ0zzJCl2WSPDrWk/OzDaImWFH3djXhb24g4eudZfLRozAvPGw4d9hQ==",
      "dev": true,
      "license": "MIT",
      "dependencies": {
        "call-bound": "^1.0.3",
        "get-intrinsic": "^1.2.6"
      },
      "engines": {
        "node": ">= 0.4"
      },
      "funding": {
        "url": "https://github.com/sponsors/ljharb"
      }
    },
    "node_modules/isarray": {
      "version": "2.0.5",
      "resolved": "https://registry.npmjs.org/isarray/-/isarray-2.0.5.tgz",
      "integrity": "sha512-xHjhDr3cNBK0BzdUJSPXZntQUx/mwMS5Rw4A7lPJ90XGAO6ISP/ePDNuo0vhqOZU+UD5JoodwCAAoZQd3FeAKw==",
      "dev": true,
      "license": "MIT"
    },
    "node_modules/isexe": {
      "version": "2.0.0",
      "resolved": "https://registry.npmjs.org/isexe/-/isexe-2.0.0.tgz",
      "integrity": "sha512-RHxMLp9lnKHGHRng9QFhRCMbYAcVpn69smSGcq3f36xjgVVWThj4qqLbTLlq7Ssj8B+fIQ1EuCEGI2lKsyQeIw==",
      "dev": true,
      "license": "ISC"
    },
    "node_modules/iterator.prototype": {
      "version": "1.1.5",
      "resolved": "https://registry.npmjs.org/iterator.prototype/-/iterator.prototype-1.1.5.tgz",
      "integrity": "sha512-H0dkQoCa3b2VEeKQBOxFph+JAbcrQdE7KC0UkqwpLmv2EC4P41QXP+rqo9wYodACiG5/WM5s9oDApTU8utwj9g==",
      "dev": true,
      "license": "MIT",
      "dependencies": {
        "define-data-property": "^1.1.4",
        "es-object-atoms": "^1.0.0",
        "get-intrinsic": "^1.2.6",
        "get-proto": "^1.0.0",
        "has-symbols": "^1.1.0",
        "set-function-name": "^2.0.2"
      },
      "engines": {
        "node": ">= 0.4"
      }
    },
    "node_modules/jiti": {
      "version": "1.21.7",
      "resolved": "https://registry.npmjs.org/jiti/-/jiti-1.21.7.tgz",
      "integrity": "sha512-/imKNG4EbWNrVjoNC/1H5/9GFy+tqjGBHCaSsN+P2RnPqjsLmv6UD3Ej+Kj8nBWaRAwyk7kK5ZUc+OEatnTR3A==",
      "license": "MIT",
      "bin": {
        "jiti": "bin/jiti.js"
      }
    },
    "node_modules/js-tokens": {
      "version": "4.0.0",
      "resolved": "https://registry.npmjs.org/js-tokens/-/js-tokens-4.0.0.tgz",
      "integrity": "sha512-RdJUflcE3cUzKiMqQgsCu06FPu9UdIJO0beYbPhHN4k6apgJtifcoCtT9bcxOpYBtpD2kCM6Sbzg4CausW/PKQ==",
      "license": "MIT"
    },
    "node_modules/js-yaml": {
      "version": "4.2.0",
      "resolved": "https://registry.npmjs.org/js-yaml/-/js-yaml-4.2.0.tgz",
      "integrity": "sha512-ePWsvanv0DWuDRsW8dnt+R4jQ31SCRCQ7hhNcPXZPsoBZiemuZNYGf7adZdqX2D86j6rvKp3RpCxVTSb8WQlOw==",
      "dev": true,
      "funding": [
        {
          "type": "github",
          "url": "https://github.com/sponsors/puzrin"
        },
        {
          "type": "github",
          "url": "https://github.com/sponsors/nodeca"
        }
      ],
      "license": "MIT",
      "dependencies": {
        "argparse": "^2.0.1"
      },
      "bin": {
        "js-yaml": "bin/js-yaml.js"
      }
    },
    "node_modules/jsesc": {
      "version": "3.1.0",
      "resolved": "https://registry.npmjs.org/jsesc/-/jsesc-3.1.0.tgz",
      "integrity": "sha512-/sM3dO2FOzXjKQhJuo0Q173wf2KOo8t4I8vHy6lF9poUp7bKT0/NHE8fPX23PwfhnykfqnC2xRxOnVw5XuGIaA==",
      "license": "MIT",
      "bin": {
        "jsesc": "bin/jsesc"
      },
      "engines": {
        "node": ">=6"
      }
    },
    "node_modules/json-buffer": {
      "version": "3.0.1",
      "resolved": "https://registry.npmjs.org/json-buffer/-/json-buffer-3.0.1.tgz",
      "integrity": "sha512-4bV5BfR2mqfQTJm+V5tPPdf+ZpuhiIvTuAB5g8kcrXOZpTT/QwwVRWBywX1ozr6lEuPdbHxwaJlm9G6mI2sfSQ==",
      "dev": true,
      "license": "MIT"
    },
    "node_modules/json-schema-traverse": {
      "version": "0.4.1",
      "resolved": "https://registry.npmjs.org/json-schema-traverse/-/json-schema-traverse-0.4.1.tgz",
      "integrity": "sha512-xbbCH5dCYU5T8LcEhhuh7HJ88HXuW3qsI3Y0zOZFKfZEHcpWiHU/Jxzk629Brsab/mMiHQti9wMP+845RPe3Vg==",
      "dev": true,
      "license": "MIT"
    },
    "node_modules/json-stable-stringify-without-jsonify": {
      "version": "1.0.1",
      "resolved": "https://registry.npmjs.org/json-stable-stringify-without-jsonify/-/json-stable-stringify-without-jsonify-1.0.1.tgz",
      "integrity": "sha512-Bdboy+l7tA3OGW6FjyFHWkP5LuByj1Tk33Ljyq0axyzdk9//JSi2u3fP1QSmd1KNwq6VOKYGlAu87CisVir6Pw==",
      "dev": true,
      "license": "MIT"
    },
    "node_modules/json5": {
      "version": "2.2.3",
      "resolved": "https://registry.npmjs.org/json5/-/json5-2.2.3.tgz",
      "integrity": "sha512-XmOWe7eyHYH14cLdVPoyg+GOH3rYX++KpzrylJwSW98t3Nk+U8XOl8FWKOgwtzdb8lXGf6zYwDUzeHMWfxasyg==",
      "dev": true,
      "license": "MIT",
      "bin": {
        "json5": "lib/cli.js"
      },
      "engines": {
        "node": ">=6"
      }
    },
    "node_modules/jspdf": {
      "version": "4.2.1",
      "resolved": "https://registry.npmjs.org/jspdf/-/jspdf-4.2.1.tgz",
      "integrity": "sha512-YyAXyvnmjTbR4bHQRLzex3CuINCDlQnBqoSYyjJwTP2x9jDLuKDzy7aKUl0hgx3uhcl7xzg32agn5vlie6HIlQ==",
      "license": "MIT",
      "dependencies": {
        "@babel/runtime": "^7.28.6",
        "fast-png": "^6.2.0",
        "fflate": "^0.8.1"
      },
      "optionalDependencies": {
        "canvg": "^3.0.11",
        "core-js": "^3.6.0",
        "dompurify": "^3.3.1",
        "html2canvas": "^1.0.0-rc.5"
      }
    },
    "node_modules/jsx-ast-utils": {
      "version": "3.3.5",
      "resolved": "https://registry.npmjs.org/jsx-ast-utils/-/jsx-ast-utils-3.3.5.tgz",
      "integrity": "sha512-ZZow9HBI5O6EPgSJLUb8n2NKgmVWTwCvHGwFuJlMjvLFqlGG6pjirPhtdsseaLZjSibD8eegzmYpUZwoIlj2cQ==",
      "dev": true,
      "license": "MIT",
      "dependencies": {
        "array-includes": "^3.1.6",
        "array.prototype.flat": "^1.3.1",
        "object.assign": "^4.1.4",
        "object.values": "^1.1.6"
      },
      "engines": {
        "node": ">=4.0"
      }
    },
    "node_modules/keyv": {
      "version": "4.5.4",
      "resolved": "https://registry.npmjs.org/keyv/-/keyv-4.5.4.tgz",
      "integrity": "sha512-oxVHkHR/EJf2CNXnWxRLW6mg7JyCCUcG0DtEGmL2ctUo1PNTin1PUil+r/+4r5MpVgC/fn1kjsx7mjSujKqIpw==",
      "dev": true,
      "license": "MIT",
      "dependencies": {
        "json-buffer": "3.0.1"
      }
    },
    "node_modules/leaflet": {
      "version": "1.9.4",
      "resolved": "https://registry.npmjs.org/leaflet/-/leaflet-1.9.4.tgz",
      "integrity": "sha512-nxS1ynzJOmOlHp+iL3FyWqK89GtNL8U8rvlMOsQdTTssxZwCXh8N2NB3GDQOL+YR3XnWyZAxwQixURb+FA74PA==",
      "license": "BSD-2-Clause",
      "peer": true
    },
    "node_modules/levn": {
      "version": "0.4.1",
      "resolved": "https://registry.npmjs.org/levn/-/levn-0.4.1.tgz",
      "integrity": "sha512-+bT2uH4E5LGE7h/n3evcS/sQlJXCpIp6ym8OWJ5eV6+67Dsql/LaaT7qJBAt2rzfoa/5QBGBhxDix1dMt2kQKQ==",
      "dev": true,
      "license": "MIT",
      "dependencies": {
        "prelude-ls": "^1.2.1",
        "type-check": "~0.4.0"
      },
      "engines": {
        "node": ">= 0.8.0"
      }
    },
    "node_modules/lilconfig": {
      "version": "3.1.3",
      "resolved": "https://registry.npmjs.org/lilconfig/-/lilconfig-3.1.3.tgz",
      "integrity": "sha512-/vlFKAoH5Cgt3Ie+JLhRbwOsCQePABiU3tJ1egGvyQ+33R/vcwM2Zl2QR/LzjsBeItPt3oSVXapn+m4nQDvpzw==",
      "license": "MIT",
      "engines": {
        "node": ">=14"
      },
      "funding": {
        "url": "https://github.com/sponsors/antonk52"
      }
    },
    "node_modules/lines-and-columns": {
      "version": "1.2.4",
      "resolved": "https://registry.npmjs.org/lines-and-columns/-/lines-and-columns-1.2.4.tgz",
      "integrity": "sha512-7ylylesZQ/PV29jhEDl3Ufjo6ZX7gCqJr5F7PKrqc93v7fzSymt1BpwEU8nAUXs8qzzvqhbjhK5QZg6Mt/HkBg==",
      "license": "MIT"
    },
    "node_modules/locate-path": {
      "version": "6.0.0",
      "resolved": "https://registry.npmjs.org/locate-path/-/locate-path-6.0.0.tgz",
      "integrity": "sha512-iPZK6eYjbxRu3uB4/WZ3EsEIMJFMqAoopl3R+zuq0UjcAm/MO6KCweDgPfP3elTztoKP3KtnVHxTn2NHBSDVUw==",
      "dev": true,
      "license": "MIT",
      "dependencies": {
        "p-locate": "^5.0.0"
      },
      "engines": {
        "node": ">=10"
      },
      "funding": {
        "url": "https://github.com/sponsors/sindresorhus"
      }
    },
    "node_modules/lodash": {
      "version": "4.18.1",
      "resolved": "https://registry.npmjs.org/lodash/-/lodash-4.18.1.tgz",
      "integrity": "sha512-dMInicTPVE8d1e5otfwmmjlxkZoUpiVLwyeTdUsi/Caj/gfzzblBcCE5sRHV/AsjuCmxWrte2TNGSYuCeCq+0Q==",
      "license": "MIT"
    },
    "node_modules/lodash.merge": {
      "version": "4.6.2",
      "resolved": "https://registry.npmjs.org/lodash.merge/-/lodash.merge-4.6.2.tgz",
      "integrity": "sha512-0KpjqXRVvrYyCsX1swR/XTK0va6VQkQM6MNo7PqW77ByjAhoARA8EfrP1N4+KlKj8YS0ZUCtRT/YUuhyYDujIQ==",
      "dev": true,
      "license": "MIT"
    },
    "node_modules/longest-streak": {
      "version": "3.1.0",
      "resolved": "https://registry.npmjs.org/longest-streak/-/longest-streak-3.1.0.tgz",
      "integrity": "sha512-9Ri+o0JYgehTaVBBDoMqIl8GXtbWg711O3srftcHhZ0dqnETqLaoIK0x17fUw9rFSlK/0NlsKe0Ahhyl5pXE2g==",
      "license": "MIT",
      "funding": {
        "type": "github",
        "url": "https://github.com/sponsors/wooorm"
      }
    },
    "node_modules/loose-envify": {
      "version": "1.4.0",
      "resolved": "https://registry.npmjs.org/loose-envify/-/loose-envify-1.4.0.tgz",
      "integrity": "sha512-lyuxPGr/Wfhrlem2CL/UcnUc1zcqKAImBDzukY7Y5F/yQiNdko6+fRLevlw1HgMySw7f611UIY408EtxRSoK3Q==",
      "license": "MIT",
      "dependencies": {
        "js-tokens": "^3.0.0 || ^4.0.0"
      },
      "bin": {
        "loose-envify": "cli.js"
      }
    },
    "node_modules/lru-cache": {
      "version": "5.1.1",
      "resolved": "https://registry.npmjs.org/lru-cache/-/lru-cache-5.1.1.tgz",
      "integrity": "sha512-KpNARQA3Iwv+jTA0utUVVbrh+Jlrr1Fv0e56GGzAFOXN7dk/FviaDW8LHmK52DlcH4WP2n6gI8vN1aesBFgo9w==",
      "dev": true,
      "license": "ISC",
      "dependencies": {
        "yallist": "^3.0.2"
      }
    },
    "node_modules/lucide-react": {
      "version": "0.475.0",
      "resolved": "https://registry.npmjs.org/lucide-react/-/lucide-react-0.475.0.tgz",
      "integrity": "sha512-NJzvVu1HwFVeZ+Gwq2q00KygM1aBhy/ZrhY9FsAgJtpB+E4R7uxRk9M2iKvHa6/vNxZydIB59htha4c2vvwvVg==",
      "license": "ISC",
      "peerDependencies": {
        "react": "^16.5.1 || ^17.0.0 || ^18.0.0 || ^19.0.0"
      }
    },
    "node_modules/math-intrinsics": {
      "version": "1.1.0",
      "resolved": "https://registry.npmjs.org/math-intrinsics/-/math-intrinsics-1.1.0.tgz",
      "integrity": "sha512-/IXtbwEk5HTPyEwyKX6hGkYXxM9nbj64B+ilVJnC/R6B0pH5G4V3b0pVbL7DBj4tkhBAppbQUlf6F6Xl9LHu1g==",
      "license": "MIT",
      "engines": {
        "node": ">= 0.4"
      }
    },
    "node_modules/mdast-util-from-markdown": {
      "version": "2.0.2",
      "resolved": "https://registry.npmjs.org/mdast-util-from-markdown/-/mdast-util-from-markdown-2.0.2.tgz",
      "integrity": "sha512-uZhTV/8NBuw0WHkPTrCqDOl0zVe1BIng5ZtHoDk49ME1qqcjYmmLmOf0gELgcRMxN4w2iuIeVso5/6QymSrgmA==",
      "license": "MIT",
      "dependencies": {
        "@types/mdast": "^4.0.0",
        "@types/unist": "^3.0.0",
        "decode-named-character-reference": "^1.0.0",
        "devlop": "^1.0.0",
        "mdast-util-to-string": "^4.0.0",
        "micromark": "^4.0.0",
        "micromark-util-decode-numeric-character-reference": "^2.0.0",
        "micromark-util-decode-string": "^2.0.0",
        "micromark-util-normalize-identifier": "^2.0.0",
        "micromark-util-symbol": "^2.0.0",
        "micromark-util-types": "^2.0.0",
        "unist-util-stringify-position": "^4.0.0"
      },
      "funding": {
        "type": "opencollective",
        "url": "https://opencollective.com/unified"
      }
    },
    "node_modules/mdast-util-mdx-expression": {
      "version": "2.0.1",
      "resolved": "https://registry.npmjs.org/mdast-util-mdx-expression/-/mdast-util-mdx-expression-2.0.1.tgz",
      "integrity": "sha512-J6f+9hUp+ldTZqKRSg7Vw5V6MqjATc+3E4gf3CFNcuZNWD8XdyI6zQ8GqH7f8169MM6P7hMBRDVGnn7oHB9kXQ==",
      "license": "MIT",
      "dependencies": {
        "@types/estree-jsx": "^1.0.0",
        "@types/hast": "^3.0.0",
        "@types/mdast": "^4.0.0",
        "devlop": "^1.0.0",
        "mdast-util-from-markdown": "^2.0.0",
        "mdast-util-to-markdown": "^2.0.0"
      },
      "funding": {
        "type": "opencollective",
        "url": "https://opencollective.com/unified"
      }
    },
    "node_modules/mdast-util-mdx-jsx": {
      "version": "3.2.0",
      "resolved": "https://registry.npmjs.org/mdast-util-mdx-jsx/-/mdast-util-mdx-jsx-3.2.0.tgz",
      "integrity": "sha512-lj/z8v0r6ZtsN/cGNNtemmmfoLAFZnjMbNyLzBafjzikOM+glrjNHPlf6lQDOTccj9n5b0PPihEBbhneMyGs1Q==",
      "license": "MIT",
      "dependencies": {
        "@types/estree-jsx": "^1.0.0",
        "@types/hast": "^3.0.0",
        "@types/mdast": "^4.0.0",
        "@types/unist": "^3.0.0",
        "ccount": "^2.0.0",
        "devlop": "^1.1.0",
        "mdast-util-from-markdown": "^2.0.0",
        "mdast-util-to-markdown": "^2.0.0",
        "parse-entities": "^4.0.0",
        "stringify-entities": "^4.0.0",
        "unist-util-stringify-position": "^4.0.0",
        "vfile-message": "^4.0.0"
      },
      "funding": {
        "type": "opencollective",
        "url": "https://opencollective.com/unified"
      }
    },
    "node_modules/mdast-util-mdxjs-esm": {
      "version": "2.0.1",
      "resolved": "https://registry.npmjs.org/mdast-util-mdxjs-esm/-/mdast-util-mdxjs-esm-2.0.1.tgz",
      "integrity": "sha512-EcmOpxsZ96CvlP03NghtH1EsLtr0n9Tm4lPUJUBccV9RwUOneqSycg19n5HGzCf+10LozMRSObtVr3ee1WoHtg==",
      "license": "MIT",
      "dependencies": {
        "@types/estree-jsx": "^1.0.0",
        "@types/hast": "^3.0.0",
        "@types/mdast": "^4.0.0",
        "devlop": "^1.0.0",
        "mdast-util-from-markdown": "^2.0.0",
        "mdast-util-to-markdown": "^2.0.0"
      },
      "funding": {
        "type": "opencollective",
        "url": "https://opencollective.com/unified"
      }
    },
    "node_modules/mdast-util-phrasing": {
      "version": "4.1.0",
      "resolved": "https://registry.npmjs.org/mdast-util-phrasing/-/mdast-util-phrasing-4.1.0.tgz",
      "integrity": "sha512-TqICwyvJJpBwvGAMZjj4J2n0X8QWp21b9l0o7eXyVJ25YNWYbJDVIyD1bZXE6WtV6RmKJVYmQAKWa0zWOABz2w==",
      "license": "MIT",
      "dependencies": {
        "@types/mdast": "^4.0.0",
        "unist-util-is": "^6.0.0"
      },
      "funding": {
        "type": "opencollective",
        "url": "https://opencollective.com/unified"
      }
    },
    "node_modules/mdast-util-to-hast": {
      "version": "13.2.1",
      "resolved": "https://registry.npmjs.org/mdast-util-to-hast/-/mdast-util-to-hast-13.2.1.tgz",
      "integrity": "sha512-cctsq2wp5vTsLIcaymblUriiTcZd0CwWtCbLvrOzYCDZoWyMNV8sZ7krj09FSnsiJi3WVsHLM4k6Dq/yaPyCXA==",
      "license": "MIT",
      "dependencies": {
        "@types/hast": "^3.0.0",
        "@types/mdast": "^4.0.0",
        "@ungap/structured-clone": "^1.0.0",
        "devlop": "^1.0.0",
        "micromark-util-sanitize-uri": "^2.0.0",
        "trim-lines": "^3.0.0",
        "unist-util-position": "^5.0.0",
        "unist-util-visit": "^5.0.0",
        "vfile": "^6.0.0"
      },
      "funding": {
        "type": "opencollective",
        "url": "https://opencollective.com/unified"
      }
    },
    "node_modules/mdast-util-to-markdown": {
      "version": "2.1.2",
      "resolved": "https://registry.npmjs.org/mdast-util-to-markdown/-/mdast-util-to-markdown-2.1.2.tgz",
      "integrity": "sha512-xj68wMTvGXVOKonmog6LwyJKrYXZPvlwabaryTjLh9LuvovB/KAH+kvi8Gjj+7rJjsFi23nkUxRQv1KqSroMqA==",
      "license": "MIT",
      "dependencies": {
        "@types/mdast": "^4.0.0",
        "@types/unist": "^3.0.0",
        "longest-streak": "^3.0.0",
        "mdast-util-phrasing": "^4.0.0",
        "mdast-util-to-string": "^4.0.0",
        "micromark-util-classify-character": "^2.0.0",
        "micromark-util-decode-string": "^2.0.0",
        "unist-util-visit": "^5.0.0",
        "zwitch": "^2.0.0"
      },
      "funding": {
        "type": "opencollective",
        "url": "https://opencollective.com/unified"
      }
    },
    "node_modules/mdast-util-to-string": {
      "version": "4.0.0",
      "resolved": "https://registry.npmjs.org/mdast-util-to-string/-/mdast-util-to-string-4.0.0.tgz",
      "integrity": "sha512-0H44vDimn51F0YwvxSJSm0eCDOJTRlmN0R1yBh4HLj9wiV1Dn0QoXGbvFAWj2hSItVTlCmBF1hqKlIyUBVFLPg==",
      "license": "MIT",
      "dependencies": {
        "@types/mdast": "^4.0.0"
      },
      "funding": {
        "type": "opencollective",
        "url": "https://opencollective.com/unified"
      }
    },
    "node_modules/memoize-one": {
      "version": "6.0.0",
      "resolved": "https://registry.npmjs.org/memoize-one/-/memoize-one-6.0.0.tgz",
      "integrity": "sha512-rkpe71W0N0c0Xz6QD0eJETuWAJGnJ9afsl1srmwPrI+yBCkge5EycXXbYRyvL29zZVUWQCY7InPRCv3GDXuZNw==",
      "license": "MIT"
    },
    "node_modules/merge2": {
      "version": "1.4.1",
      "resolved": "https://registry.npmjs.org/merge2/-/merge2-1.4.1.tgz",
      "integrity": "sha512-8q7VEgMJW4J8tcfVPy8g09NcQwZdbwFEqhe/WZkoIzjn/3TGDwtOCYtXGxA3O8tPzpczCCDgv+P2P5y00ZJOOg==",
      "license": "MIT",
      "engines": {
        "node": ">= 8"
      }
    },
    "node_modules/micromark": {
      "version": "4.0.2",
      "resolved": "https://registry.npmjs.org/micromark/-/micromark-4.0.2.tgz",
      "integrity": "sha512-zpe98Q6kvavpCr1NPVSCMebCKfD7CA2NqZ+rykeNhONIJBpc1tFKt9hucLGwha3jNTNI8lHpctWJWoimVF4PfA==",
      "funding": [
        {
          "type": "GitHub Sponsors",
          "url": "https://github.com/sponsors/unifiedjs"
        },
        {
          "type": "OpenCollective",
          "url": "https://opencollective.com/unified"
        }
      ],
      "license": "MIT",
      "dependencies": {
        "@types/debug": "^4.0.0",
        "debug": "^4.0.0",
        "decode-named-character-reference": "^1.0.0",
        "devlop": "^1.0.0",
        "micromark-core-commonmark": "^2.0.0",
        "micromark-factory-space": "^2.0.0",
        "micromark-util-character": "^2.0.0",
        "micromark-util-chunked": "^2.0.0",
        "micromark-util-combine-extensions": "^2.0.0",
        "micromark-util-decode-numeric-character-reference": "^2.0.0",
        "micromark-util-encode": "^2.0.0",
        "micromark-util-normalize-identifier": "^2.0.0",
        "micromark-util-resolve-all": "^2.0.0",
        "micromark-util-sanitize-uri": "^2.0.0",
        "micromark-util-subtokenize": "^2.0.0",
        "micromark-util-symbol": "^2.0.0",
        "micromark-util-types": "^2.0.0"
      }
    },
    "node_modules/micromark-core-commonmark": {
      "version": "2.0.3",
      "resolved": "https://registry.npmjs.org/micromark-core-commonmark/-/micromark-core-commonmark-2.0.3.tgz",
      "integrity": "sha512-RDBrHEMSxVFLg6xvnXmb1Ayr2WzLAWjeSATAoxwKYJV94TeNavgoIdA0a9ytzDSVzBy2YKFK+emCPOEibLeCrg==",
      "funding": [
        {
          "type": "GitHub Sponsors",
          "url": "https://github.com/sponsors/unifiedjs"
        },
        {
          "type": "OpenCollective",
          "url": "https://opencollective.com/unified"
        }
      ],
      "license": "MIT",
      "dependencies": {
        "decode-named-character-reference": "^1.0.0",
        "devlop": "^1.0.0",
        "micromark-factory-destination": "^2.0.0",
        "micromark-factory-label": "^2.0.0",
        "micromark-factory-space": "^2.0.0",
        "micromark-factory-title": "^2.0.0",
        "micromark-factory-whitespace": "^2.0.0",
        "micromark-util-character": "^2.0.0",
        "micromark-util-chunked": "^2.0.0",
        "micromark-util-classify-character": "^2.0.0",
        "micromark-util-html-tag-name": "^2.0.0",
        "micromark-util-normalize-identifier": "^2.0.0",
        "micromark-util-resolve-all": "^2.0.0",
        "micromark-util-subtokenize": "^2.0.0",
        "micromark-util-symbol": "^2.0.0",
        "micromark-util-types": "^2.0.0"
      }
    },
    "node_modules/micromark-factory-destination": {
      "version": "2.0.1",
      "resolved": "https://registry.npmjs.org/micromark-factory-destination/-/micromark-factory-destination-2.0.1.tgz",
      "integrity": "sha512-Xe6rDdJlkmbFRExpTOmRj9N3MaWmbAgdpSrBQvCFqhezUn4AHqJHbaEnfbVYYiexVSs//tqOdY/DxhjdCiJnIA==",
      "funding": [
        {
          "type": "GitHub Sponsors",
          "url": "https://github.com/sponsors/unifiedjs"
        },
        {
          "type": "OpenCollective",
          "url": "https://opencollective.com/unified"
        }
      ],
      "license": "MIT",
      "dependencies": {
        "micromark-util-character": "^2.0.0",
        "micromark-util-symbol": "^2.0.0",
        "micromark-util-types": "^2.0.0"
      }
    },
    "node_modules/micromark-factory-label": {
      "version": "2.0.1",
      "resolved": "https://registry.npmjs.org/micromark-factory-label/-/micromark-factory-label-2.0.1.tgz",
      "integrity": "sha512-VFMekyQExqIW7xIChcXn4ok29YE3rnuyveW3wZQWWqF4Nv9Wk5rgJ99KzPvHjkmPXF93FXIbBp6YdW3t71/7Vg==",
      "funding": [
        {
          "type": "GitHub Sponsors",
          "url": "https://github.com/sponsors/unifiedjs"
        },
        {
          "type": "OpenCollective",
          "url": "https://opencollective.com/unified"
        }
      ],
      "license": "MIT",
      "dependencies": {
        "devlop": "^1.0.0",
        "micromark-util-character": "^2.0.0",
        "micromark-util-symbol": "^2.0.0",
        "micromark-util-types": "^2.0.0"
      }
    },
    "node_modules/micromark-factory-space": {
      "version": "2.0.1",
      "resolved": "https://registry.npmjs.org/micromark-factory-space/-/micromark-factory-space-2.0.1.tgz",
      "integrity": "sha512-zRkxjtBxxLd2Sc0d+fbnEunsTj46SWXgXciZmHq0kDYGnck/ZSGj9/wULTV95uoeYiK5hRXP2mJ98Uo4cq/LQg==",
      "funding": [
        {
          "type": "GitHub Sponsors",
          "url": "https://github.com/sponsors/unifiedjs"
        },
        {
          "type": "OpenCollective",
          "url": "https://opencollective.com/unified"
        }
      ],
      "license": "MIT",
      "dependencies": {
        "micromark-util-character": "^2.0.0",
        "micromark-util-types": "^2.0.0"
      }
    },
    "node_modules/micromark-factory-title": {
      "version": "2.0.1",
      "resolved": "https://registry.npmjs.org/micromark-factory-title/-/micromark-factory-title-2.0.1.tgz",
      "integrity": "sha512-5bZ+3CjhAd9eChYTHsjy6TGxpOFSKgKKJPJxr293jTbfry2KDoWkhBb6TcPVB4NmzaPhMs1Frm9AZH7OD4Cjzw==",
      "funding": [
        {
          "type": "GitHub Sponsors",
          "url": "https://github.com/sponsors/unifiedjs"
        },
        {
          "type": "OpenCollective",
          "url": "https://opencollective.com/unified"
        }
      ],
      "license": "MIT",
      "dependencies": {
        "micromark-factory-space": "^2.0.0",
        "micromark-util-character": "^2.0.0",
        "micromark-util-symbol": "^2.0.0",
        "micromark-util-types": "^2.0.0"
      }
    },
    "node_modules/micromark-factory-whitespace": {
      "version": "2.0.1",
      "resolved": "https://registry.npmjs.org/micromark-factory-whitespace/-/micromark-factory-whitespace-2.0.1.tgz",
      "integrity": "sha512-Ob0nuZ3PKt/n0hORHyvoD9uZhr+Za8sFoP+OnMcnWK5lngSzALgQYKMr9RJVOWLqQYuyn6ulqGWSXdwf6F80lQ==",
      "funding": [
        {
          "type": "GitHub Sponsors",
          "url": "https://github.com/sponsors/unifiedjs"
        },
        {
          "type": "OpenCollective",
          "url": "https://opencollective.com/unified"
        }
      ],
      "license": "MIT",
      "dependencies": {
        "micromark-factory-space": "^2.0.0",
        "micromark-util-character": "^2.0.0",
        "micromark-util-symbol": "^2.0.0",
        "micromark-util-types": "^2.0.0"
      }
    },
    "node_modules/micromark-util-character": {
      "version": "2.1.1",
      "resolved": "https://registry.npmjs.org/micromark-util-character/-/micromark-util-character-2.1.1.tgz",
      "integrity": "sha512-wv8tdUTJ3thSFFFJKtpYKOYiGP2+v96Hvk4Tu8KpCAsTMs6yi+nVmGh1syvSCsaxz45J6Jbw+9DD6g97+NV67Q==",
      "funding": [
        {
          "type": "GitHub Sponsors",
          "url": "https://github.com/sponsors/unifiedjs"
        },
        {
          "type": "OpenCollective",
          "url": "https://opencollective.com/unified"
        }
      ],
      "license": "MIT",
      "dependencies": {
        "micromark-util-symbol": "^2.0.0",
        "micromark-util-types": "^2.0.0"
      }
    },
    "node_modules/micromark-util-chunked": {
      "version": "2.0.1",
      "resolved": "https://registry.npmjs.org/micromark-util-chunked/-/micromark-util-chunked-2.0.1.tgz",
      "integrity": "sha512-QUNFEOPELfmvv+4xiNg2sRYeS/P84pTW0TCgP5zc9FpXetHY0ab7SxKyAQCNCc1eK0459uoLI1y5oO5Vc1dbhA==",
      "funding": [
        {
          "type": "GitHub Sponsors",
          "url": "https://github.com/sponsors/unifiedjs"
        },
        {
          "type": "OpenCollective",
          "url": "https://opencollective.com/unified"
        }
      ],
      "license": "MIT",
      "dependencies": {
        "micromark-util-symbol": "^2.0.0"
      }
    },
    "node_modules/micromark-util-classify-character": {
      "version": "2.0.1",
      "resolved": "https://registry.npmjs.org/micromark-util-classify-character/-/micromark-util-classify-character-2.0.1.tgz",
      "integrity": "sha512-K0kHzM6afW/MbeWYWLjoHQv1sgg2Q9EccHEDzSkxiP/EaagNzCm7T/WMKZ3rjMbvIpvBiZgwR3dKMygtA4mG1Q==",
      "funding": [
        {
          "type": "GitHub Sponsors",
          "url": "https://github.com/sponsors/unifiedjs"
        },
        {
          "type": "OpenCollective",
          "url": "https://opencollective.com/unified"
        }
      ],
      "license": "MIT",
      "dependencies": {
        "micromark-util-character": "^2.0.0",
        "micromark-util-symbol": "^2.0.0",
        "micromark-util-types": "^2.0.0"
      }
    },
    "node_modules/micromark-util-combine-extensions": {
      "version": "2.0.1",
      "resolved": "https://registry.npmjs.org/micromark-util-combine-extensions/-/micromark-util-combine-extensions-2.0.1.tgz",
      "integrity": "sha512-OnAnH8Ujmy59JcyZw8JSbK9cGpdVY44NKgSM7E9Eh7DiLS2E9RNQf0dONaGDzEG9yjEl5hcqeIsj4hfRkLH/Bg==",
      "funding": [
        {
          "type": "GitHub Sponsors",
          "url": "https://github.com/sponsors/unifiedjs"
        },
        {
          "type": "OpenCollective",
          "url": "https://opencollective.com/unified"
        }
      ],
      "license": "MIT",
      "dependencies": {
        "micromark-util-chunked": "^2.0.0",
        "micromark-util-types": "^2.0.0"
      }
    },
    "node_modules/micromark-util-decode-numeric-character-reference": {
      "version": "2.0.2",
      "resolved": "https://registry.npmjs.org/micromark-util-decode-numeric-character-reference/-/micromark-util-decode-numeric-character-reference-2.0.2.tgz",
      "integrity": "sha512-ccUbYk6CwVdkmCQMyr64dXz42EfHGkPQlBj5p7YVGzq8I7CtjXZJrubAYezf7Rp+bjPseiROqe7G6foFd+lEuw==",
      "funding": [
        {
          "type": "GitHub Sponsors",
          "url": "https://github.com/sponsors/unifiedjs"
        },
        {
          "type": "OpenCollective",
          "url": "https://opencollective.com/unified"
        }
      ],
      "license": "MIT",
      "dependencies": {
        "micromark-util-symbol": "^2.0.0"
      }
    },
    "node_modules/micromark-util-decode-string": {
      "version": "2.0.1",
      "resolved": "https://registry.npmjs.org/micromark-util-decode-string/-/micromark-util-decode-string-2.0.1.tgz",
      "integrity": "sha512-nDV/77Fj6eH1ynwscYTOsbK7rR//Uj0bZXBwJZRfaLEJ1iGBR6kIfNmlNqaqJf649EP0F3NWNdeJi03elllNUQ==",
      "funding": [
        {
          "type": "GitHub Sponsors",
          "url": "https://github.com/sponsors/unifiedjs"
        },
        {
          "type": "OpenCollective",
          "url": "https://opencollective.com/unified"
        }
      ],
      "license": "MIT",
      "dependencies": {
        "decode-named-character-reference": "^1.0.0",
        "micromark-util-character": "^2.0.0",
        "micromark-util-decode-numeric-character-reference": "^2.0.0",
        "micromark-util-symbol": "^2.0.0"
      }
    },
    "node_modules/micromark-util-encode": {
      "version": "2.0.1",
      "resolved": "https://registry.npmjs.org/micromark-util-encode/-/micromark-util-encode-2.0.1.tgz",
      "integrity": "sha512-c3cVx2y4KqUnwopcO9b/SCdo2O67LwJJ/UyqGfbigahfegL9myoEFoDYZgkT7f36T0bLrM9hZTAaAyH+PCAXjw==",
      "funding": [
        {
          "type": "GitHub Sponsors",
          "url": "https://github.com/sponsors/unifiedjs"
        },
        {
          "type": "OpenCollective",
          "url": "https://opencollective.com/unified"
        }
      ],
      "license": "MIT"
    },
    "node_modules/micromark-util-html-tag-name": {
      "version": "2.0.1",
      "resolved": "https://registry.npmjs.org/micromark-util-html-tag-name/-/micromark-util-html-tag-name-2.0.1.tgz",
      "integrity": "sha512-2cNEiYDhCWKI+Gs9T0Tiysk136SnR13hhO8yW6BGNyhOC4qYFnwF1nKfD3HFAIXA5c45RrIG1ub11GiXeYd1xA==",
      "funding": [
        {
          "type": "GitHub Sponsors",
          "url": "https://github.com/sponsors/unifiedjs"
        },
        {
          "type": "OpenCollective",
          "url": "https://opencollective.com/unified"
        }
      ],
      "license": "MIT"
    },
    "node_modules/micromark-util-normalize-identifier": {
      "version": "2.0.1",
      "resolved": "https://registry.npmjs.org/micromark-util-normalize-identifier/-/micromark-util-normalize-identifier-2.0.1.tgz",
      "integrity": "sha512-sxPqmo70LyARJs0w2UclACPUUEqltCkJ6PhKdMIDuJ3gSf/Q+/GIe3WKl0Ijb/GyH9lOpUkRAO2wp0GVkLvS9Q==",
      "funding": [
        {
          "type": "GitHub Sponsors",
          "url": "https://github.com/sponsors/unifiedjs"
        },
        {
          "type": "OpenCollective",
          "url": "https://opencollective.com/unified"
        }
      ],
      "license": "MIT",
      "dependencies": {
        "micromark-util-symbol": "^2.0.0"
      }
    },
    "node_modules/micromark-util-resolve-all": {
      "version": "2.0.1",
      "resolved": "https://registry.npmjs.org/micromark-util-resolve-all/-/micromark-util-resolve-all-2.0.1.tgz",
      "integrity": "sha512-VdQyxFWFT2/FGJgwQnJYbe1jjQoNTS4RjglmSjTUlpUMa95Htx9NHeYW4rGDJzbjvCsl9eLjMQwGeElsqmzcHg==",
      "funding": [
        {
          "type": "GitHub Sponsors",
          "url": "https://github.com/sponsors/unifiedjs"
        },
        {
          "type": "OpenCollective",
          "url": "https://opencollective.com/unified"
        }
      ],
      "license": "MIT",
      "dependencies": {
        "micromark-util-types": "^2.0.0"
      }
    },
    "node_modules/micromark-util-sanitize-uri": {
      "version": "2.0.1",
      "resolved": "https://registry.npmjs.org/micromark-util-sanitize-uri/-/micromark-util-sanitize-uri-2.0.1.tgz",
      "integrity": "sha512-9N9IomZ/YuGGZZmQec1MbgxtlgougxTodVwDzzEouPKo3qFWvymFHWcnDi2vzV1ff6kas9ucW+o3yzJK9YB1AQ==",
      "funding": [
        {
          "type": "GitHub Sponsors",
          "url": "https://github.com/sponsors/unifiedjs"
        },
        {
          "type": "OpenCollective",
          "url": "https://opencollective.com/unified"
        }
      ],
      "license": "MIT",
      "dependencies": {
        "micromark-util-character": "^2.0.0",
        "micromark-util-encode": "^2.0.0",
        "micromark-util-symbol": "^2.0.0"
      }
    },
    "node_modules/micromark-util-subtokenize": {
      "version": "2.1.0",
      "resolved": "https://registry.npmjs.org/micromark-util-subtokenize/-/micromark-util-subtokenize-2.1.0.tgz",
      "integrity": "sha512-XQLu552iSctvnEcgXw6+Sx75GflAPNED1qx7eBJ+wydBb2KCbRZe+NwvIEEMM83uml1+2WSXpBAcp9IUCgCYWA==",
      "funding": [
        {
          "type": "GitHub Sponsors",
          "url": "https://github.com/sponsors/unifiedjs"
        },
        {
          "type": "OpenCollective",
          "url": "https://opencollective.com/unified"
        }
      ],
      "license": "MIT",
      "dependencies": {
        "devlop": "^1.0.0",
        "micromark-util-chunked": "^2.0.0",
        "micromark-util-symbol": "^2.0.0",
        "micromark-util-types": "^2.0.0"
      }
    },
    "node_modules/micromark-util-symbol": {
      "version": "2.0.1",
      "resolved": "https://registry.npmjs.org/micromark-util-symbol/-/micromark-util-symbol-2.0.1.tgz",
      "integrity": "sha512-vs5t8Apaud9N28kgCrRUdEed4UJ+wWNvicHLPxCa9ENlYuAY31M0ETy5y1vA33YoNPDFTghEbnh6efaE8h4x0Q==",
      "funding": [
        {
          "type": "GitHub Sponsors",
          "url": "https://github.com/sponsors/unifiedjs"
        },
        {
          "type": "OpenCollective",
          "url": "https://opencollective.com/unified"
        }
      ],
      "license": "MIT"
    },
    "node_modules/micromark-util-types": {
      "version": "2.0.2",
      "resolved": "https://registry.npmjs.org/micromark-util-types/-/micromark-util-types-2.0.2.tgz",
      "integrity": "sha512-Yw0ECSpJoViF1qTU4DC6NwtC4aWGt1EkzaQB8KPPyCRR8z9TWeV0HbEFGTO+ZY1wB22zmxnJqhPyTpOVCpeHTA==",
      "funding": [
        {
          "type": "GitHub Sponsors",
          "url": "https://github.com/sponsors/unifiedjs"
        },
        {
          "type": "OpenCollective",
          "url": "https://opencollective.com/unified"
        }
      ],
      "license": "MIT"
    },
    "node_modules/micromatch": {
      "version": "4.0.8",
      "resolved": "https://registry.npmjs.org/micromatch/-/micromatch-4.0.8.tgz",
      "integrity": "sha512-PXwfBhYu0hBCPw8Dn0E+WDYb7af3dSLVWKi3HGv84IdF4TyFoC0ysxFd0Goxw7nSv4T/PzEJQxsYsEiFCKo2BA==",
      "license": "MIT",
      "dependencies": {
        "braces": "^3.0.3",
        "picomatch": "^2.3.1"
      },
      "engines": {
        "node": ">=8.6"
      }
    },
    "node_modules/mime-db": {
      "version": "1.52.0",
      "resolved": "https://registry.npmjs.org/mime-db/-/mime-db-1.52.0.tgz",
      "integrity": "sha512-sPU4uV7dYlvtWJxwwxHD0PuihVNiE7TyAbQ5SWxDCB9mUYvOgroQOwYQQOKPJ8CIbE+1ETVlOoK1UC2nU3gYvg==",
      "license": "MIT",
      "engines": {
        "node": ">= 0.6"
      }
    },
    "node_modules/mime-types": {
      "version": "2.1.35",
      "resolved": "https://registry.npmjs.org/mime-types/-/mime-types-2.1.35.tgz",
      "integrity": "sha512-ZDY+bPm5zTTF+YpCrAU9nK0UgICYPT0QtT1NZWFv4s++TNkcgVaT0g6+4R2uI4MjQjzysHB1zxuWL50hzaeXiw==",
      "license": "MIT",
      "dependencies": {
        "mime-db": "1.52.0"
      },
      "engines": {
        "node": ">= 0.6"
      }
    },
    "node_modules/minimatch": {
      "version": "3.1.5",
      "resolved": "https://registry.npmjs.org/minimatch/-/minimatch-3.1.5.tgz",
      "integrity": "sha512-VgjWUsnnT6n+NUk6eZq77zeFdpW2LWDzP6zFGrCbHXiYNul5Dzqk2HHQ5uFH2DNW5Xbp8+jVzaeNt94ssEEl4w==",
      "dev": true,
      "license": "ISC",
      "dependencies": {
        "brace-expansion": "^1.1.7"
      },
      "engines": {
        "node": "*"
      }
    },
    "node_modules/moment": {
      "version": "2.30.1",
      "resolved": "https://registry.npmjs.org/moment/-/moment-2.30.1.tgz",
      "integrity": "sha512-uEmtNhbDOrWPFS+hdjFCBfy9f2YoyzRpwcl+DqpC6taX21FzsTLQVbMV/W7PzNSX6x/bhC1zA3c2UQ5NzH6how==",
      "license": "MIT",
      "engines": {
        "node": "*"
      }
    },
    "node_modules/motion-dom": {
      "version": "11.18.1",
      "resolved": "https://registry.npmjs.org/motion-dom/-/motion-dom-11.18.1.tgz",
      "integrity": "sha512-g76KvA001z+atjfxczdRtw/RXOM3OMSdd1f4DL77qCTF/+avrRJiawSG4yDibEQ215sr9kpinSlX2pCTJ9zbhw==",
      "license": "MIT",
      "dependencies": {
        "motion-utils": "^11.18.1"
      }
    },
    "node_modules/motion-utils": {
      "version": "11.18.1",
      "resolved": "https://registry.npmjs.org/motion-utils/-/motion-utils-11.18.1.tgz",
      "integrity": "sha512-49Kt+HKjtbJKLtgO/LKj9Ld+6vw9BjH5d9sc40R/kVyH8GLAXgT42M2NnuPcJNuA3s9ZfZBUcwIgpmZWGEE+hA==",
      "license": "MIT"
    },
    "node_modules/ms": {
      "version": "2.1.3",
      "resolved": "https://registry.npmjs.org/ms/-/ms-2.1.3.tgz",
      "integrity": "sha512-6FlzubTLZG3J2a/NVCAleEhjzq5oxgHyaCU9yYXvcLsvoVaHJq/s5xXI6/XXP6tz7R9xAOtHnSO/tXtF3WRTlA==",
      "license": "MIT"
    },
    "node_modules/mz": {
      "version": "2.7.0",
      "resolved": "https://registry.npmjs.org/mz/-/mz-2.7.0.tgz",
      "integrity": "sha512-z81GNO7nnYMEhrGh9LeymoE4+Yr0Wn5McHIZMK5cfQCl+NDX08sCZgUc9/6MHni9IWuFLm1Z3HTCXu2z9fN62Q==",
      "license": "MIT",
      "dependencies": {
        "any-promise": "^1.0.0",
        "object-assign": "^4.0.1",
        "thenify-all": "^1.0.0"
      }
    },
    "node_modules/nanoid": {
      "version": "3.3.15",
      "resolved": "https://registry.npmjs.org/nanoid/-/nanoid-3.3.15.tgz",
      "integrity": "sha512-y7Wygv/7mEOvxTuEQDB8StXdMRBWf1kR/tlhAzBRUFkB2jfcLOAxO/SHmOO2zgz1pVgK29/kyupn059/bCHdjA==",
      "funding": [
        {
          "type": "github",
          "url": "https://github.com/sponsors/ai"
        }
      ],
      "license": "MIT",
      "bin": {
        "nanoid": "bin/nanoid.cjs"
      },
      "engines": {
        "node": "^10 || ^12 || ^13.7 || ^14 || >=15.0.1"
      }
    },
    "node_modules/natural-compare": {
      "version": "1.4.0",
      "resolved": "https://registry.npmjs.org/natural-compare/-/natural-compare-1.4.0.tgz",
      "integrity": "sha512-OWND8ei3VtNC9h7V60qff3SVobHr996CTwgxubgyQYEpg290h9J0buyECNNJexkFm5sOajh5G116RYA1c8ZMSw==",
      "dev": true,
      "license": "MIT"
    },
    "node_modules/next-themes": {
      "version": "0.4.6",
      "resolved": "https://registry.npmjs.org/next-themes/-/next-themes-0.4.6.tgz",
      "integrity": "sha512-pZvgD5L0IEvX5/9GWyHMf3m8BKiVQwsCMHfoFosXtXBMnaS0ZnIJ9ST4b4NqLVKDEm8QBxoNNGNaBv2JNF6XNA==",
      "license": "MIT",
      "peerDependencies": {
        "react": "^16.8 || ^17 || ^18 || ^19 || ^19.0.0-rc",
        "react-dom": "^16.8 || ^17 || ^18 || ^19 || ^19.0.0-rc"
      }
    },
    "node_modules/node-exports-info": {
      "version": "1.6.0",
      "resolved": "https://registry.npmjs.org/node-exports-info/-/node-exports-info-1.6.0.tgz",
      "integrity": "sha512-pyFS63ptit/P5WqUkt+UUfe+4oevH+bFeIiPPdfb0pFeYEu/1ELnJu5l+5EcTKYL5M7zaAa7S8ddywgXypqKCw==",
      "dev": true,
      "license": "MIT",
      "dependencies": {
        "array.prototype.flatmap": "^1.3.3",
        "es-errors": "^1.3.0",
        "object.entries": "^1.1.9",
        "semver": "^6.3.1"
      },
      "engines": {
        "node": ">= 0.4"
      },
      "funding": {
        "url": "https://github.com/sponsors/ljharb"
      }
    },
    "node_modules/node-releases": {
      "version": "2.0.27",
      "resolved": "https://registry.npmjs.org/node-releases/-/node-releases-2.0.27.tgz",
      "integrity": "sha512-nmh3lCkYZ3grZvqcCH+fjmQ7X+H0OeZgP40OierEaAptX4XofMh5kwNbWh7lBduUzCcV/8kZ+NDLCwm2iorIlA==",
      "dev": true,
      "license": "MIT"
    },
    "node_modules/normalize-path": {
      "version": "3.0.0",
      "resolved": "https://registry.npmjs.org/normalize-path/-/normalize-path-3.0.0.tgz",
      "integrity": "sha512-6eZs5Ls3WtCisHWp9S2GUy8dqkpGi4BVSz3GaqiE6ezub0512ESztXUwUB6C6IKbQkY2Pnb/mD4WYojCRwcwLA==",
      "license": "MIT",
      "engines": {
        "node": ">=0.10.0"
      }
    },
    "node_modules/object-assign": {
      "version": "4.1.1",
      "resolved": "https://registry.npmjs.org/object-assign/-/object-assign-4.1.1.tgz",
      "integrity": "sha512-rJgTQnkUnH1sFw8yT6VSU3zD3sWmu6sZhIseY8VX+GRu3P6F7Fu+JNDoXfklElbLJSnc3FUQHVe4cU5hj+BcUg==",
      "license": "MIT",
      "engines": {
        "node": ">=0.10.0"
      }
    },
    "node_modules/object-hash": {
      "version": "3.0.0",
      "resolved": "https://registry.npmjs.org/object-hash/-/object-hash-3.0.0.tgz",
      "integrity": "sha512-RSn9F68PjH9HqtltsSnqYC1XXoWe9Bju5+213R98cNGttag9q9yAOTzdbsqvIa7aNm5WffBZFpWYr2aWrklWAw==",
      "license": "MIT",
      "engines": {
        "node": ">= 6"
      }
    },
    "node_modules/object-inspect": {
      "version": "1.13.4",
      "resolved": "https://registry.npmjs.org/object-inspect/-/object-inspect-1.13.4.tgz",
      "integrity": "sha512-W67iLl4J2EXEGTbfeHCffrjDfitvLANg0UlX3wFUUSTx92KXRFegMHUVgSqE+wvhAbi4WqjGg9czysTV2Epbew==",
      "dev": true,
      "license": "MIT",
      "engines": {
        "node": ">= 0.4"
      },
      "funding": {
        "url": "https://github.com/sponsors/ljharb"
      }
    },
    "node_modules/object-is": {
      "version": "1.1.6",
      "resolved": "https://registry.npmjs.org/object-is/-/object-is-1.1.6.tgz",
      "integrity": "sha512-F8cZ+KfGlSGi09lJT7/Nd6KJZ9ygtvYC0/UYYLI9nmQKLMnydpB9yvbv9K1uSkEu7FU9vYPmVwLg328tX+ot3Q==",
      "license": "MIT",
      "dependencies": {
        "call-bind": "^1.0.7",
        "define-properties": "^1.2.1"
      },
      "engines": {
        "node": ">= 0.4"
      },
      "funding": {
        "url": "https://github.com/sponsors/ljharb"
      }
    },
    "node_modules/object-keys": {
      "version": "1.1.1",
      "resolved": "https://registry.npmjs.org/object-keys/-/object-keys-1.1.1.tgz",
      "integrity": "sha512-NuAESUOUMrlIXOfHKzD6bpPu3tYt3xvjNdRIQ+FeT0lNb4K8WR70CaDxhuNguS2XG+GjkyMwOzsN5ZktImfhLA==",
      "license": "MIT",
      "engines": {
        "node": ">= 0.4"
      }
    },
    "node_modules/object.assign": {
      "version": "4.1.7",
      "resolved": "https://registry.npmjs.org/object.assign/-/object.assign-4.1.7.tgz",
      "integrity": "sha512-nK28WOo+QIjBkDduTINE4JkF/UJJKyf2EJxvJKfblDpyg0Q+pkOHNTL0Qwy6NP6FhE/EnzV73BxxqcJaXY9anw==",
      "dev": true,
      "license": "MIT",
      "dependencies": {
        "call-bind": "^1.0.8",
        "call-bound": "^1.0.3",
        "define-properties": "^1.2.1",
        "es-object-atoms": "^1.0.0",
        "has-symbols": "^1.1.0",
        "object-keys": "^1.1.1"
      },
      "engines": {
        "node": ">= 0.4"
      },
      "funding": {
        "url": "https://github.com/sponsors/ljharb"
      }
    },
    "node_modules/object.entries": {
      "version": "1.1.9",
      "resolved": "https://registry.npmjs.org/object.entries/-/object.entries-1.1.9.tgz",
      "integrity": "sha512-8u/hfXFRBD1O0hPUjioLhoWFHRmt6tKA4/vZPyckBr18l1KE9uHrFaFaUi8MDRTpi4uak2goyPTSNJLXX2k2Hw==",
      "dev": true,
      "license": "MIT",
      "dependencies": {
        "call-bind": "^1.0.8",
        "call-bound": "^1.0.4",
        "define-properties": "^1.2.1",
        "es-object-atoms": "^1.1.1"
      },
      "engines": {
        "node": ">= 0.4"
      }
    },
    "node_modules/object.fromentries": {
      "version": "2.0.8",
      "resolved": "https://registry.npmjs.org/object.fromentries/-/object.fromentries-2.0.8.tgz",
      "integrity": "sha512-k6E21FzySsSK5a21KRADBd/NGneRegFO5pLHfdQLpRDETUNJueLXs3WCzyQ3tFRDYgbq3KHGXfTbi2bs8WQ6rQ==",
      "dev": true,
      "license": "MIT",
      "dependencies": {
        "call-bind": "^1.0.7",
        "define-properties": "^1.2.1",
        "es-abstract": "^1.23.2",
        "es-object-atoms": "^1.0.0"
      },
      "engines": {
        "node": ">= 0.4"
      },
      "funding": {
        "url": "https://github.com/sponsors/ljharb"
      }
    },
    "node_modules/object.values": {
      "version": "1.2.1",
      "resolved": "https://registry.npmjs.org/object.values/-/object.values-1.2.1.tgz",
      "integrity": "sha512-gXah6aZrcUxjWg2zR2MwouP2eHlCBzdV4pygudehaKXSGW4v2AsRQUK+lwwXhii6KFZcunEnmSUoYp5CXibxtA==",
      "dev": true,
      "license": "MIT",
      "dependencies": {
        "call-bind": "^1.0.8",
        "call-bound": "^1.0.3",
        "define-properties": "^1.2.1",
        "es-object-atoms": "^1.0.0"
      },
      "engines": {
        "node": ">= 0.4"
      },
      "funding": {
        "url": "https://github.com/sponsors/ljharb"
      }
    },
    "node_modules/optionator": {
      "version": "0.9.4",
      "resolved": "https://registry.npmjs.org/optionator/-/optionator-0.9.4.tgz",
      "integrity": "sha512-6IpQ7mKUxRcZNLIObR0hz7lxsapSSIYNZJwXPGeF0mTVqGKFIXj1DQcMoT22S3ROcLyY/rz0PWaWZ9ayWmad9g==",
      "dev": true,
      "license": "MIT",
      "dependencies": {
        "deep-is": "^0.1.3",
        "fast-levenshtein": "^2.0.6",
        "levn": "^0.4.1",
        "prelude-ls": "^1.2.1",
        "type-check": "^0.4.0",
        "word-wrap": "^1.2.5"
      },
      "engines": {
        "node": ">= 0.8.0"
      }
    },
    "node_modules/own-keys": {
      "version": "1.0.1",
      "resolved": "https://registry.npmjs.org/own-keys/-/own-keys-1.0.1.tgz",
      "integrity": "sha512-qFOyK5PjiWZd+QQIh+1jhdb9LpxTF0qs7Pm8o5QHYZ0M3vKqSqzsZaEB6oWlxZ+q2sJBMI/Ktgd2N5ZwQoRHfg==",
      "dev": true,
      "license": "MIT",
      "dependencies": {
        "get-intrinsic": "^1.2.6",
        "object-keys": "^1.1.1",
        "safe-push-apply": "^1.0.0"
      },
      "engines": {
        "node": ">= 0.4"
      },
      "funding": {
        "url": "https://github.com/sponsors/ljharb"
      }
    },
    "node_modules/p-limit": {
      "version": "3.1.0",
      "resolved": "https://registry.npmjs.org/p-limit/-/p-limit-3.1.0.tgz",
      "integrity": "sha512-TYOanM3wGwNGsZN2cVTYPArw454xnXj5qmWF1bEoAc4+cU/ol7GVh7odevjp1FNHduHc3KZMcFduxU5Xc6uJRQ==",
      "dev": true,
      "license": "MIT",
      "dependencies": {
        "yocto-queue": "^0.1.0"
      },
      "engines": {
        "node": ">=10"
      },
      "funding": {
        "url": "https://github.com/sponsors/sindresorhus"
      }
    },
    "node_modules/p-locate": {
      "version": "5.0.0",
      "resolved": "https://registry.npmjs.org/p-locate/-/p-locate-5.0.0.tgz",
      "integrity": "sha512-LaNjtRWUBY++zB5nE/NwcaoMylSPk+S+ZHNB1TzdbMJMny6dynpAGt7X/tl/QYq3TIeE6nxHppbo2LGymrG5Pw==",
      "dev": true,
      "license": "MIT",
      "dependencies": {
        "p-limit": "^3.0.2"
      },
      "engines": {
        "node": ">=10"
      },
      "funding": {
        "url": "https://github.com/sponsors/sindresorhus"
      }
    },
    "node_modules/pako": {
      "version": "2.1.0",
      "resolved": "https://registry.npmjs.org/pako/-/pako-2.1.0.tgz",
      "integrity": "sha512-w+eufiZ1WuJYgPXbV/PO3NCMEc3xqylkKHzp8bxp1uW4qaSNQUkwmLLEc3kKsfz8lpV1F8Ht3U1Cm+9Srog2ug==",
      "license": "(MIT AND Zlib)"
    },
    "node_modules/parchment": {
      "version": "1.1.4",
      "resolved": "https://registry.npmjs.org/parchment/-/parchment-1.1.4.tgz",
      "integrity": "sha512-J5FBQt/pM2inLzg4hEWmzQx/8h8D0CiDxaG3vyp9rKrQRSDgBlhjdP5jQGgosEajXPSQouXGHOmVdgo7QmJuOg==",
      "license": "BSD-3-Clause"
    },
    "node_modules/parent-module": {
      "version": "1.0.1",
      "resolved": "https://registry.npmjs.org/parent-module/-/parent-module-1.0.1.tgz",
      "integrity": "sha512-GQ2EWRpQV8/o+Aw8YqtfZZPfNRWZYkbidE9k5rpl/hC3vtHHBfGm2Ifi6qWV+coDGkrUKZAxE3Lot5kcsRlh+g==",
      "dev": true,
      "license": "MIT",
      "dependencies": {
        "callsites": "^3.0.0"
      },
      "engines": {
        "node": ">=6"
      }
    },
    "node_modules/parse-entities": {
      "version": "4.0.2",
      "resolved": "https://registry.npmjs.org/parse-entities/-/parse-entities-4.0.2.tgz",
      "integrity": "sha512-GG2AQYWoLgL877gQIKeRPGO1xF9+eG1ujIb5soS5gPvLQ1y2o8FL90w2QWNdf9I361Mpp7726c+lj3U0qK1uGw==",
      "license": "MIT",
      "dependencies": {
        "@types/unist": "^2.0.0",
        "character-entities-legacy": "^3.0.0",
        "character-reference-invalid": "^2.0.0",
        "decode-named-character-reference": "^1.0.0",
        "is-alphanumerical": "^2.0.0",
        "is-decimal": "^2.0.0",
        "is-hexadecimal": "^2.0.0"
      },
      "funding": {
        "type": "github",
        "url": "https://github.com/sponsors/wooorm"
      }
    },
    "node_modules/parse-entities/node_modules/@types/unist": {
      "version": "2.0.11",
      "resolved": "https://registry.npmjs.org/@types/unist/-/unist-2.0.11.tgz",
      "integrity": "sha512-CmBKiL6NNo/OqgmMn95Fk9Whlp2mtvIv+KNpQKN2F4SjvrEesubTRWGYSg+BnWZOnlCaSTU1sMpsBOzgbYhnsA==",
      "license": "MIT"
    },
    "node_modules/path-exists": {
      "version": "4.0.0",
      "resolved": "https://registry.npmjs.org/path-exists/-/path-exists-4.0.0.tgz",
      "integrity": "sha512-ak9Qy5Q7jYb2Wwcey5Fpvg2KoAc/ZIhLSLOSBmRmygPsGwkVVt0fZa0qrtMz+m6tJTAHfZQ8FnmB4MG4LWy7/w==",
      "dev": true,
      "license": "MIT",
      "engines": {
        "node": ">=8"
      }
    },
    "node_modules/path-key": {
      "version": "3.1.1",
      "resolved": "https://registry.npmjs.org/path-key/-/path-key-3.1.1.tgz",
      "integrity": "sha512-ojmeN0qd+y0jszEtoY48r0Peq5dwMEkIlCOu6Q5f41lfkswXuKtYrhgoTpLnyIcHm24Uhqx+5Tqm2InSwLhE6Q==",
      "dev": true,
      "license": "MIT",
      "engines": {
        "node": ">=8"
      }
    },
    "node_modules/path-parse": {
      "version": "1.0.7",
      "resolved": "https://registry.npmjs.org/path-parse/-/path-parse-1.0.7.tgz",
      "integrity": "sha512-LDJzPVEEEPR+y48z93A0Ed0yXb8pAByGWo/k5YYdYgpY2/2EsOsksJrq7lOHxryrVOn1ejG6oAp8ahvOIQD8sw==",
      "license": "MIT"
    },
    "node_modules/performance-now": {
      "version": "2.1.0",
      "resolved": "https://registry.npmjs.org/performance-now/-/performance-now-2.1.0.tgz",
      "integrity": "sha512-7EAHlyLHI56VEIdK57uwHdHKIaAGbnXPiw0yWbarQZOKaKpvUIgW0jWRVLiatnM+XXlSwsanIBH/hzGMJulMow==",
      "license": "MIT",
      "optional": true
    },
    "node_modules/picocolors": {
      "version": "1.1.1",
      "resolved": "https://registry.npmjs.org/picocolors/-/picocolors-1.1.1.tgz",
      "integrity": "sha512-xceH2snhtb5M9liqDsmEw56le376mTZkEX/jEb/RxNFyegNul7eNslCXP9FDj/Lcu0X8KEyMceP2ntpaHrDEVA==",
      "license": "ISC"
    },
    "node_modules/picomatch": {
      "version": "2.3.2",
      "resolved": "https://registry.npmjs.org/picomatch/-/picomatch-2.3.2.tgz",
      "integrity": "sha512-V7+vQEJ06Z+c5tSye8S+nHUfI51xoXIXjHQ99cQtKUkQqqO1kO/KCJUfZXuB47h/YBlDhah2H3hdUGXn8ie0oA==",
      "license": "MIT",
      "engines": {
        "node": ">=8.6"
      },
      "funding": {
        "url": "https://github.com/sponsors/jonschlinkert"
      }
    },
    "node_modules/pify": {
      "version": "2.3.0",
      "resolved": "https://registry.npmjs.org/pify/-/pify-2.3.0.tgz",
      "integrity": "sha512-udgsAY+fTnvv7kI7aaxbqwWNb0AHiB0qBO89PZKPkoTmGOgdbrHDKD+0B2X4uTfJ/FT1R09r9gTsjUjNJotuog==",
      "license": "MIT",
      "engines": {
        "node": ">=0.10.0"
      }
    },
    "node_modules/pirates": {
      "version": "4.0.7",
      "resolved": "https://registry.npmjs.org/pirates/-/pirates-4.0.7.tgz",
      "integrity": "sha512-TfySrs/5nm8fQJDcBDuUng3VOUKsd7S+zqvbOTiGXHfxX4wK31ard+hoNuvkicM/2YFzlpDgABOevKSsB4G/FA==",
      "license": "MIT",
      "engines": {
        "node": ">= 6"
      }
    },
    "node_modules/possible-typed-array-names": {
      "version": "1.1.0",
      "resolved": "https://registry.npmjs.org/possible-typed-array-names/-/possible-typed-array-names-1.1.0.tgz",
      "integrity": "sha512-/+5VFTchJDoVj3bhoqi6UeymcD00DAwb1nJwamzPvHEszJ4FpF6SNNbUbOS8yI56qHzdV8eK0qEfOSiodkTdxg==",
      "dev": true,
      "license": "MIT",
      "engines": {
        "node": ">= 0.4"
      }
    },
    "node_modules/postcss": {
      "version": "8.5.15",
      "resolved": "https://registry.npmjs.org/postcss/-/postcss-8.5.15.tgz",
      "integrity": "sha512-FfR8sjd4em2T6fb3I2MwAJU7HWVMr9zba+enmQeeWFfCbm+UOC/0X4DS8XtpUTMwWMGbjKYP7xjfNekzyGmB3A==",
      "funding": [
        {
          "type": "opencollective",
          "url": "https://opencollective.com/postcss/"
        },
        {
          "type": "tidelift",
          "url": "https://tidelift.com/funding/github/npm/postcss"
        },
        {
          "type": "github",
          "url": "https://github.com/sponsors/ai"
        }
      ],
      "license": "MIT",
      "dependencies": {
        "nanoid": "^3.3.12",
        "picocolors": "^1.1.1",
        "source-map-js": "^1.2.1"
      },
      "engines": {
        "node": "^10 || ^12 || >=14"
      }
    },
    "node_modules/postcss-import": {
      "version": "15.1.0",
      "resolved": "https://registry.npmjs.org/postcss-import/-/postcss-import-15.1.0.tgz",
      "integrity": "sha512-hpr+J05B2FVYUAXHeK1YyI267J/dDDhMU6B6civm8hSY1jYJnBXxzKDKDswzJmtLHryrjhnDjqqp/49t8FALew==",
      "license": "MIT",
      "dependencies": {
        "postcss-value-parser": "^4.0.0",
        "read-cache": "^1.0.0",
        "resolve": "^1.1.7"
      },
      "engines": {
        "node": ">=14.0.0"
      },
      "peerDependencies": {
        "postcss": "^8.0.0"
      }
    },
    "node_modules/postcss-import/node_modules/resolve": {
      "version": "1.22.11",
      "resolved": "https://registry.npmjs.org/resolve/-/resolve-1.22.11.tgz",
      "integrity": "sha512-RfqAvLnMl313r7c9oclB1HhUEAezcpLjz95wFH4LVuhk9JF/r22qmVP9AMmOU4vMX7Q8pN8jwNg/CSpdFnMjTQ==",
      "license": "MIT",
      "dependencies": {
        "is-core-module": "^2.16.1",
        "path-parse": "^1.0.7",
        "supports-preserve-symlinks-flag": "^1.0.0"
      },
      "bin": {
        "resolve": "bin/resolve"
      },
      "engines": {
        "node": ">= 0.4"
      },
      "funding": {
        "url": "https://github.com/sponsors/ljharb"
      }
    },
    "node_modules/postcss-js": {
      "version": "4.1.0",
      "resolved": "https://registry.npmjs.org/postcss-js/-/postcss-js-4.1.0.tgz",
      "integrity": "sha512-oIAOTqgIo7q2EOwbhb8UalYePMvYoIeRY2YKntdpFQXNosSu3vLrniGgmH9OKs/qAkfoj5oB3le/7mINW1LCfw==",
      "funding": [
        {
          "type": "opencollective",
          "url": "https://opencollective.com/postcss/"
        },
        {
          "type": "github",
          "url": "https://github.com/sponsors/ai"
        }
      ],
      "license": "MIT",
      "dependencies": {
        "camelcase-css": "^2.0.1"
      },
      "engines": {
        "node": "^12 || ^14 || >= 16"
      },
      "peerDependencies": {
        "postcss": "^8.4.21"
      }
    },
    "node_modules/postcss-load-config": {
      "version": "6.0.1",
      "resolved": "https://registry.npmjs.org/postcss-load-config/-/postcss-load-config-6.0.1.tgz",
      "integrity": "sha512-oPtTM4oerL+UXmx+93ytZVN82RrlY/wPUV8IeDxFrzIjXOLF1pN+EmKPLbubvKHT2HC20xXsCAH2Z+CKV6Oz/g==",
      "funding": [
        {
          "type": "opencollective",
          "url": "https://opencollective.com/postcss/"
        },
        {
          "type": "github",
          "url": "https://github.com/sponsors/ai"
        }
      ],
      "license": "MIT",
      "dependencies": {
        "lilconfig": "^3.1.1"
      },
      "engines": {
        "node": ">= 18"
      },
      "peerDependencies": {
        "jiti": ">=1.21.0",
        "postcss": ">=8.0.9",
        "tsx": "^4.8.1",
        "yaml": "^2.4.2"
      },
      "peerDependenciesMeta": {
        "jiti": {
          "optional": true
        },
        "postcss": {
          "optional": true
        },
        "tsx": {
          "optional": true
        },
        "yaml": {
          "optional": true
        }
      }
    },
    "node_modules/postcss-nested": {
      "version": "6.2.0",
      "resolved": "https://registry.npmjs.org/postcss-nested/-/postcss-nested-6.2.0.tgz",
      "integrity": "sha512-HQbt28KulC5AJzG+cZtj9kvKB93CFCdLvog1WFLf1D+xmMvPGlBstkpTEZfK5+AN9hfJocyBFCNiqyS48bpgzQ==",
      "funding": [
        {
          "type": "opencollective",
          "url": "https://opencollective.com/postcss/"
        },
        {
          "type": "github",
          "url": "https://github.com/sponsors/ai"
        }
      ],
      "license": "MIT",
      "dependencies": {
        "postcss-selector-parser": "^6.1.1"
      },
      "engines": {
        "node": ">=12.0"
      },
      "peerDependencies": {
        "postcss": "^8.2.14"
      }
    },
    "node_modules/postcss-selector-parser": {
      "version": "6.1.2",
      "resolved": "https://registry.npmjs.org/postcss-selector-parser/-/postcss-selector-parser-6.1.2.tgz",
      "integrity": "sha512-Q8qQfPiZ+THO/3ZrOrO0cJJKfpYCagtMUkXbnEfmgUjwXg6z/WBeOyS9APBBPCTSiDV+s4SwQGu8yFsiMRIudg==",
      "license": "MIT",
      "dependencies": {
        "cssesc": "^3.0.0",
        "util-deprecate": "^1.0.2"
      },
      "engines": {
        "node": ">=4"
      }
    },
    "node_modules/postcss-value-parser": {
      "version": "4.2.0",
      "resolved": "https://registry.npmjs.org/postcss-value-parser/-/postcss-value-parser-4.2.0.tgz",
      "integrity": "sha512-1NNCs6uurfkVbeXG4S8JFT9t19m45ICnif8zWLd5oPSZ50QnwMfK+H3jv408d4jw/7Bttv5axS5IiHoLaVNHeQ==",
      "license": "MIT"
    },
    "node_modules/prelude-ls": {
      "version": "1.2.1",
      "resolved": "https://registry.npmjs.org/prelude-ls/-/prelude-ls-1.2.1.tgz",
      "integrity": "sha512-vkcDPrRZo1QZLbn5RLGPpg/WmIQ65qoWWhcGKf/b5eplkkarX0m9z8ppCat4mlOqUsWpyNuYgO3VRyrYHSzX5g==",
      "dev": true,
      "license": "MIT",
      "engines": {
        "node": ">= 0.8.0"
      }
    },
    "node_modules/prop-types": {
      "version": "15.8.1",
      "resolved": "https://registry.npmjs.org/prop-types/-/prop-types-15.8.1.tgz",
      "integrity": "sha512-oj87CgZICdulUohogVAR7AjlC0327U4el4L6eAvOqCeudMDVU0NThNaV+b9Df4dXgSP1gXMTnPdhfe/2qDH5cg==",
      "license": "MIT",
      "dependencies": {
        "loose-envify": "^1.4.0",
        "object-assign": "^4.1.1",
        "react-is": "^16.13.1"
      }
    },
    "node_modules/property-information": {
      "version": "7.1.0",
      "resolved": "https://registry.npmjs.org/property-information/-/property-information-7.1.0.tgz",
      "integrity": "sha512-TwEZ+X+yCJmYfL7TPUOcvBZ4QfoT5YenQiJuX//0th53DE6w0xxLEtfK3iyryQFddXuvkIk51EEgrJQ0WJkOmQ==",
      "license": "MIT",
      "funding": {
        "type": "github",
        "url": "https://github.com/sponsors/wooorm"
      }
    },
    "node_modules/proxy-from-env": {
      "version": "2.1.0",
      "resolved": "https://registry.npmjs.org/proxy-from-env/-/proxy-from-env-2.1.0.tgz",
      "integrity": "sha512-cJ+oHTW1VAEa8cJslgmUZrc+sjRKgAKl3Zyse6+PV38hZe/V6Z14TbCuXcan9F9ghlz4QrFr2c92TNF82UkYHA==",
      "license": "MIT",
      "engines": {
        "node": ">=10"
      }
    },
    "node_modules/punycode": {
      "version": "2.3.1",
      "resolved": "https://registry.npmjs.org/punycode/-/punycode-2.3.1.tgz",
      "integrity": "sha512-vYt7UD1U9Wg6138shLtLOvdAu+8DsC/ilFtEVHcH+wydcSpNE20AfSOduf6MkRFahL5FY7X1oU7nKVZFtfq8Fg==",
      "dev": true,
      "license": "MIT",
      "engines": {
        "node": ">=6"
      }
    },
    "node_modules/queue-microtask": {
      "version": "1.2.3",
      "resolved": "https://registry.npmjs.org/queue-microtask/-/queue-microtask-1.2.3.tgz",
      "integrity": "sha512-NuaNSa6flKT5JaSYQzJok04JzTL1CA6aGhv5rfLW3PgqA+M2ChpZQnAC8h8i4ZFkBS8X5RqkDBHA7r4hej3K9A==",
      "funding": [
        {
          "type": "github",
          "url": "https://github.com/sponsors/feross"
        },
        {
          "type": "patreon",
          "url": "https://www.patreon.com/feross"
        },
        {
          "type": "consulting",
          "url": "https://feross.org/support"
        }
      ],
      "license": "MIT"
    },
    "node_modules/quill": {
      "version": "1.3.7",
      "resolved": "https://registry.npmjs.org/quill/-/quill-1.3.7.tgz",
      "integrity": "sha512-hG/DVzh/TiknWtE6QmWAF/pxoZKYxfe3J/d/+ShUWkDvvkZQVTPeVmUJVu1uE6DDooC4fWTiCLh84ul89oNz5g==",
      "license": "BSD-3-Clause",
      "dependencies": {
        "clone": "^2.1.1",
        "deep-equal": "^1.0.1",
        "eventemitter3": "^2.0.3",
        "extend": "^3.0.2",
        "parchment": "^1.1.4",
        "quill-delta": "^3.6.2"
      }
    },
    "node_modules/quill-delta": {
      "version": "3.6.3",
      "resolved": "https://registry.npmjs.org/quill-delta/-/quill-delta-3.6.3.tgz",
      "integrity": "sha512-wdIGBlcX13tCHOXGMVnnTVFtGRLoP0imqxM696fIPwIf5ODIYUHIvHbZcyvGlZFiFhK5XzDC2lpjbxRhnM05Tg==",
      "license": "MIT",
      "dependencies": {
        "deep-equal": "^1.0.1",
        "extend": "^3.0.2",
        "fast-diff": "1.1.2"
      },
      "engines": {
        "node": ">=0.10"
      }
    },
    "node_modules/raf": {
      "version": "3.4.1",
      "resolved": "https://registry.npmjs.org/raf/-/raf-3.4.1.tgz",
      "integrity": "sha512-Sq4CW4QhwOHE8ucn6J34MqtZCeWFP2aQSmrlroYgqAV1PjStIhJXxYuTgUIfkEk7zTLjmIjLmU5q+fbD1NnOJA==",
      "license": "MIT",
      "optional": true,
      "dependencies": {
        "performance-now": "^2.1.0"
      }
    },
    "node_modules/raf-schd": {
      "version": "4.0.3",
      "resolved": "https://registry.npmjs.org/raf-schd/-/raf-schd-4.0.3.tgz",
      "integrity": "sha512-tQkJl2GRWh83ui2DiPTJz9wEiMN20syf+5oKfB03yYP7ioZcJwsIK8FjrtLwH1m7C7e+Tt2yYBlrOpdT+dyeIQ==",
      "license": "MIT"
    },
    "node_modules/react": {
      "version": "18.3.1",
      "resolved": "https://registry.npmjs.org/react/-/react-18.3.1.tgz",
      "integrity": "sha512-wS+hAgJShR0KhEvPJArfuPVN1+Hz1t0Y6n5jLrGQbkb4urgPE/0Rve+1kMB1v/oWgHgm4WIcV+i7F2pTVj+2iQ==",
      "license": "MIT",
      "dependencies": {
        "loose-envify": "^1.1.0"
      },
      "engines": {
        "node": ">=0.10.0"
      }
    },
    "node_modules/react-day-picker": {
      "version": "8.10.1",
      "resolved": "https://registry.npmjs.org/react-day-picker/-/react-day-picker-8.10.1.tgz",
      "integrity": "sha512-TMx7fNbhLk15eqcMt+7Z7S2KF7mfTId/XJDjKE8f+IUcFn0l08/kI4FiYTL/0yuOLmEcbR4Fwe3GJf/NiiMnPA==",
      "license": "MIT",
      "funding": {
        "type": "individual",
        "url": "https://github.com/sponsors/gpbl"
      },
      "peerDependencies": {
        "date-fns": "^2.28.0 || ^3.0.0",
        "react": "^16.8.0 || ^17.0.0 || ^18.0.0"
      }
    },
    "node_modules/react-dom": {
      "version": "18.3.1",
      "resolved": "https://registry.npmjs.org/react-dom/-/react-dom-18.3.1.tgz",
      "integrity": "sha512-5m4nQKp+rZRb09LNH59GM4BxTh9251/ylbKIbpe7TpGxfJ+9kv6BLkLBXIjjspbgbnIBNqlI23tRnTWT0snUIw==",
      "license": "MIT",
      "dependencies": {
        "loose-envify": "^1.1.0",
        "scheduler": "^0.23.2"
      },
      "peerDependencies": {
        "react": "^18.3.1"
      }
    },
    "node_modules/react-hook-form": {
      "version": "7.71.1",
      "resolved": "https://registry.npmjs.org/react-hook-form/-/react-hook-form-7.71.1.tgz",
      "integrity": "sha512-9SUJKCGKo8HUSsCO+y0CtqkqI5nNuaDqTxyqPsZPqIwudpj4rCrAz/jZV+jn57bx5gtZKOh3neQu94DXMc+w5w==",
      "license": "MIT",
      "engines": {
        "node": ">=18.0.0"
      },
      "funding": {
        "type": "opencollective",
        "url": "https://opencollective.com/react-hook-form"
      },
      "peerDependencies": {
        "react": "^16.8.0 || ^17 || ^18 || ^19"
      }
    },
    "node_modules/react-hot-toast": {
      "version": "2.6.0",
      "resolved": "https://registry.npmjs.org/react-hot-toast/-/react-hot-toast-2.6.0.tgz",
      "integrity": "sha512-bH+2EBMZ4sdyou/DPrfgIouFpcRLCJ+HoCA32UoAYHn6T3Ur5yfcDCeSr5mwldl6pFOsiocmrXMuoCJ1vV8bWg==",
      "license": "MIT",
      "dependencies": {
        "csstype": "^3.1.3",
        "goober": "^2.1.16"
      },
      "engines": {
        "node": ">=10"
      },
      "peerDependencies": {
        "react": ">=16",
        "react-dom": ">=16"
      }
    },
    "node_modules/react-is": {
      "version": "16.13.1",
      "resolved": "https://registry.npmjs.org/react-is/-/react-is-16.13.1.tgz",
      "integrity": "sha512-24e6ynE2H+OKt4kqsOvNd8kBpV65zoxbA4BVsEOB3ARVWQki/DHzaUoC5KuON/BiccDaCCTZBuOcfZs70kR8bQ==",
      "license": "MIT"
    },
    "node_modules/react-leaflet": {
      "version": "4.2.1",
      "resolved": "https://registry.npmjs.org/react-leaflet/-/react-leaflet-4.2.1.tgz",
      "integrity": "sha512-p9chkvhcKrWn/H/1FFeVSqLdReGwn2qmiobOQGO3BifX+/vV/39qhY8dGqbdcPh1e6jxh/QHriLXr7a4eLFK4Q==",
      "license": "Hippocratic-2.1",
      "dependencies": {
        "@react-leaflet/core": "^2.1.0"
      },
      "peerDependencies": {
        "leaflet": "^1.9.0",
        "react": "^18.0.0",
        "react-dom": "^18.0.0"
      }
    },
    "node_modules/react-markdown": {
      "version": "9.1.0",
      "resolved": "https://registry.npmjs.org/react-markdown/-/react-markdown-9.1.0.tgz",
      "integrity": "sha512-xaijuJB0kzGiUdG7nc2MOMDUDBWPyGAjZtUrow9XxUeua8IqeP+VlIfAZ3bphpcLTnSZXz6z9jcVC/TCwbfgdw==",
      "license": "MIT",
      "dependencies": {
        "@types/hast": "^3.0.0",
        "@types/mdast": "^4.0.0",
        "devlop": "^1.0.0",
        "hast-util-to-jsx-runtime": "^2.0.0",
        "html-url-attributes": "^3.0.0",
        "mdast-util-to-hast": "^13.0.0",
        "remark-parse": "^11.0.0",
        "remark-rehype": "^11.0.0",
        "unified": "^11.0.0",
        "unist-util-visit": "^5.0.0",
        "vfile": "^6.0.0"
      },
      "funding": {
        "type": "opencollective",
        "url": "https://opencollective.com/unified"
      },
      "peerDependencies": {
        "@types/react": ">=18",
        "react": ">=18"
      }
    },
    "node_modules/react-quill": {
      "version": "2.0.0",
      "resolved": "https://registry.npmjs.org/react-quill/-/react-quill-2.0.0.tgz",
      "integrity": "sha512-4qQtv1FtCfLgoD3PXAur5RyxuUbPXQGOHgTlFie3jtxp43mXDtzCKaOgQ3mLyZfi1PUlyjycfivKelFhy13QUg==",
      "license": "MIT",
      "dependencies": {
        "@types/quill": "^1.3.10",
        "lodash": "^4.17.4",
        "quill": "^1.3.7"
      },
      "peerDependencies": {
        "react": "^16 || ^17 || ^18",
        "react-dom": "^16 || ^17 || ^18"
      }
    },
    "node_modules/react-redux": {
      "version": "9.2.0",
      "resolved": "https://registry.npmjs.org/react-redux/-/react-redux-9.2.0.tgz",
      "integrity": "sha512-ROY9fvHhwOD9ySfrF0wmvu//bKCQ6AeZZq1nJNtbDC+kk5DuSuNX/n6YWYF/SYy7bSba4D4FSz8DJeKY/S/r+g==",
      "license": "MIT",
      "dependencies": {
        "@types/use-sync-external-store": "^0.0.6",
        "use-sync-external-store": "^1.4.0"
      },
      "peerDependencies": {
        "@types/react": "^18.2.25 || ^19",
        "react": "^18.0 || ^19",
        "redux": "^5.0.0"
      },
      "peerDependenciesMeta": {
        "@types/react": {
          "optional": true
        },
        "redux": {
          "optional": true
        }
      }
    },
    "node_modules/react-refresh": {
      "version": "0.17.0",
      "resolved": "https://registry.npmjs.org/react-refresh/-/react-refresh-0.17.0.tgz",
      "integrity": "sha512-z6F7K9bV85EfseRCp2bzrpyQ0Gkw1uLoCel9XBVWPg/TjRj94SkJzUTGfOa4bs7iJvBWtQG0Wq7wnI0syw3EBQ==",
      "dev": true,
      "license": "MIT",
      "engines": {
        "node": ">=0.10.0"
      }
    },
    "node_modules/react-remove-scroll": {
      "version": "2.7.2",
      "resolved": "https://registry.npmjs.org/react-remove-scroll/-/react-remove-scroll-2.7.2.tgz",
      "integrity": "sha512-Iqb9NjCCTt6Hf+vOdNIZGdTiH1QSqr27H/Ek9sv/a97gfueI/5h1s3yRi1nngzMUaOOToin5dI1dXKdXiF+u0Q==",
      "license": "MIT",
      "dependencies": {
        "react-remove-scroll-bar": "^2.3.7",
        "react-style-singleton": "^2.2.3",
        "tslib": "^2.1.0",
        "use-callback-ref": "^1.3.3",
        "use-sidecar": "^1.1.3"
      },
      "engines": {
        "node": ">=10"
      },
      "peerDependencies": {
        "@types/react": "*",
        "react": "^16.8.0 || ^17.0.0 || ^18.0.0 || ^19.0.0 || ^19.0.0-rc"
      },
      "peerDependenciesMeta": {
        "@types/react": {
          "optional": true
        }
      }
    },
    "node_modules/react-remove-scroll-bar": {
      "version": "2.3.8",
      "resolved": "https://registry.npmjs.org/react-remove-scroll-bar/-/react-remove-scroll-bar-2.3.8.tgz",
      "integrity": "sha512-9r+yi9+mgU33AKcj6IbT9oRCO78WriSj6t/cF8DWBZJ9aOGPOTEDvdUDz1FwKim7QXWwmHqtdHnRJfhAxEG46Q==",
      "license": "MIT",
      "dependencies": {
        "react-style-singleton": "^2.2.2",
        "tslib": "^2.0.0"
      },
      "engines": {
        "node": ">=10"
      },
      "peerDependencies": {
        "@types/react": "*",
        "react": "^16.8.0 || ^17.0.0 || ^18.0.0 || ^19.0.0"
      },
      "peerDependenciesMeta": {
        "@types/react": {
          "optional": true
        }
      }
    },
    "node_modules/react-resizable-panels": {
      "version": "2.1.9",
      "resolved": "https://registry.npmjs.org/react-resizable-panels/-/react-resizable-panels-2.1.9.tgz",
      "integrity": "sha512-z77+X08YDIrgAes4jl8xhnUu1LNIRp4+E7cv4xHmLOxxUPO/ML7PSrE813b90vj7xvQ1lcf7g2uA9GeMZonjhQ==",
      "license": "MIT",
      "peerDependencies": {
        "react": "^16.14.0 || ^17.0.0 || ^18.0.0 || ^19.0.0 || ^19.0.0-rc",
        "react-dom": "^16.14.0 || ^17.0.0 || ^18.0.0 || ^19.0.0 || ^19.0.0-rc"
      }
    },
    "node_modules/react-router": {
      "version": "6.30.4",
      "resolved": "https://registry.npmjs.org/react-router/-/react-router-6.30.4.tgz",
      "integrity": "sha512-SVUsDe+DybHM/WmYKIVYhZh1o5Dcuf16yM6WjG02Q9XVFMZIJyHYhwrr6bFBXZkVP6z69kNkMyBCujt8FaFLJA==",
      "license": "MIT",
      "dependencies": {
        "@remix-run/router": "1.23.3"
      },
      "engines": {
        "node": ">=14.0.0"
      },
      "peerDependencies": {
        "react": ">=16.8"
      }
    },
    "node_modules/react-router-dom": {
      "version": "6.30.4",
      "resolved": "https://registry.npmjs.org/react-router-dom/-/react-router-dom-6.30.4.tgz",
      "integrity": "sha512-q4HvNl+mmDdkS0g+MqiBZNteQJCuimWoOyHMy4T/RQLAn9Z29+E91QXRaxOujeMl2HTzRSS0KFPd7lxX3PjV0Q==",
      "license": "MIT",
      "dependencies": {
        "@remix-run/router": "1.23.3",
        "react-router": "6.30.4"
      },
      "engines": {
        "node": ">=14.0.0"
      },
      "peerDependencies": {
        "react": ">=16.8",
        "react-dom": ">=16.8"
      }
    },
    "node_modules/react-smooth": {
      "version": "4.0.4",
      "resolved": "https://registry.npmjs.org/react-smooth/-/react-smooth-4.0.4.tgz",
      "integrity": "sha512-gnGKTpYwqL0Iii09gHobNolvX4Kiq4PKx6eWBCYYix+8cdw+cGo3do906l1NBPKkSWx1DghC1dlWG9L2uGd61Q==",
      "license": "MIT",
      "dependencies": {
        "fast-equals": "^5.0.1",
        "prop-types": "^15.8.1",
        "react-transition-group": "^4.4.5"
      },
      "peerDependencies": {
        "react": "^16.8.0 || ^17.0.0 || ^18.0.0 || ^19.0.0",
        "react-dom": "^16.8.0 || ^17.0.0 || ^18.0.0 || ^19.0.0"
      }
    },
    "node_modules/react-style-singleton": {
      "version": "2.2.3",
      "resolved": "https://registry.npmjs.org/react-style-singleton/-/react-style-singleton-2.2.3.tgz",
      "integrity": "sha512-b6jSvxvVnyptAiLjbkWLE/lOnR4lfTtDAl+eUC7RZy+QQWc6wRzIV2CE6xBuMmDxc2qIihtDCZD5NPOFl7fRBQ==",
      "license": "MIT",
      "dependencies": {
        "get-nonce": "^1.0.0",
        "tslib": "^2.0.0"
      },
      "engines": {
        "node": ">=10"
      },
      "peerDependencies": {
        "@types/react": "*",
        "react": "^16.8.0 || ^17.0.0 || ^18.0.0 || ^19.0.0 || ^19.0.0-rc"
      },
      "peerDependenciesMeta": {
        "@types/react": {
          "optional": true
        }
      }
    },
    "node_modules/react-transition-group": {
      "version": "4.4.5",
      "resolved": "https://registry.npmjs.org/react-transition-group/-/react-transition-group-4.4.5.tgz",
      "integrity": "sha512-pZcd1MCJoiKiBR2NRxeCRg13uCXbydPnmB4EOeRrY7480qNWO8IIgQG6zlDkm6uRMsURXPuKq0GWtiM59a5Q6g==",
      "license": "BSD-3-Clause",
      "dependencies": {
        "@babel/runtime": "^7.5.5",
        "dom-helpers": "^5.0.1",
        "loose-envify": "^1.4.0",
        "prop-types": "^15.6.2"
      },
      "peerDependencies": {
        "react": ">=16.6.0",
        "react-dom": ">=16.6.0"
      }
    },
    "node_modules/read-cache": {
      "version": "1.0.0",
      "resolved": "https://registry.npmjs.org/read-cache/-/read-cache-1.0.0.tgz",
      "integrity": "sha512-Owdv/Ft7IjOgm/i0xvNDZ1LrRANRfew4b2prF3OWMQLxLfu3bS8FVhCsrSCMK4lR56Y9ya+AThoTpDCTxCmpRA==",
      "license": "MIT",
      "dependencies": {
        "pify": "^2.3.0"
      }
    },
    "node_modules/readdirp": {
      "version": "3.6.0",
      "resolved": "https://registry.npmjs.org/readdirp/-/readdirp-3.6.0.tgz",
      "integrity": "sha512-hOS089on8RduqdbhvQ5Z37A0ESjsqz6qnRcffsMU3495FuTdqSm+7bhJ29JvIOsBDEEnan5DPu9t3To9VRlMzA==",
      "license": "MIT",
      "dependencies": {
        "picomatch": "^2.2.1"
      },
      "engines": {
        "node": ">=8.10.0"
      }
    },
    "node_modules/recharts": {
      "version": "2.15.4",
      "resolved": "https://registry.npmjs.org/recharts/-/recharts-2.15.4.tgz",
      "integrity": "sha512-UT/q6fwS3c1dHbXv2uFgYJ9BMFHu3fwnd7AYZaEQhXuYQ4hgsxLvsUXzGdKeZrW5xopzDCvuA2N41WJ88I7zIw==",
      "license": "MIT",
      "dependencies": {
        "clsx": "^2.0.0",
        "eventemitter3": "^4.0.1",
        "lodash": "^4.17.21",
        "react-is": "^18.3.1",
        "react-smooth": "^4.0.4",
        "recharts-scale": "^0.4.4",
        "tiny-invariant": "^1.3.1",
        "victory-vendor": "^36.6.8"
      },
      "engines": {
        "node": ">=14"
      },
      "peerDependencies": {
        "react": "^16.0.0 || ^17.0.0 || ^18.0.0 || ^19.0.0",
        "react-dom": "^16.0.0 || ^17.0.0 || ^18.0.0 || ^19.0.0"
      }
    },
    "node_modules/recharts-scale": {
      "version": "0.4.5",
      "resolved": "https://registry.npmjs.org/recharts-scale/-/recharts-scale-0.4.5.tgz",
      "integrity": "sha512-kivNFO+0OcUNu7jQquLXAxz1FIwZj8nrj+YkOKc5694NbjCvcT6aSZiIzNzd2Kul4o4rTto8QVR9lMNtxD4G1w==",
      "license": "MIT",
      "dependencies": {
        "decimal.js-light": "^2.4.1"
      }
    },
    "node_modules/recharts/node_modules/eventemitter3": {
      "version": "4.0.7",
      "resolved": "https://registry.npmjs.org/eventemitter3/-/eventemitter3-4.0.7.tgz",
      "integrity": "sha512-8guHBZCwKnFhYdHr2ysuRWErTwhoN2X8XELRlrRwpmfeY2jjuUN4taQMsULKUVo1K4DvZl+0pgfyoysHxvmvEw==",
      "license": "MIT"
    },
    "node_modules/recharts/node_modules/react-is": {
      "version": "18.3.1",
      "resolved": "https://registry.npmjs.org/react-is/-/react-is-18.3.1.tgz",
      "integrity": "sha512-/LLMVyas0ljjAtoYiPqYiL8VWXzUUdThrmU5+n20DZv+a+ClRoevUzw5JxU+Ieh5/c87ytoTBV9G1FiKfNJdmg==",
      "license": "MIT"
    },
    "node_modules/redux": {
      "version": "5.0.1",
      "resolved": "https://registry.npmjs.org/redux/-/redux-5.0.1.tgz",
      "integrity": "sha512-M9/ELqF6fy8FwmkpnF0S3YKOqMyoWJ4+CS5Efg2ct3oY9daQvd/Pc71FpGZsVsbl3Cpb+IIcjBDUnnyBdQbq4w==",
      "license": "MIT"
    },
    "node_modules/reflect.getprototypeof": {
      "version": "1.0.10",
      "resolved": "https://registry.npmjs.org/reflect.getprototypeof/-/reflect.getprototypeof-1.0.10.tgz",
      "integrity": "sha512-00o4I+DVrefhv+nX0ulyi3biSHCPDe+yLv5o/p6d/UVlirijB8E16FtfwSAi4g3tcqrQ4lRAqQSoFEZJehYEcw==",
      "dev": true,
      "license": "MIT",
      "dependencies": {
        "call-bind": "^1.0.8",
        "define-properties": "^1.2.1",
        "es-abstract": "^1.23.9",
        "es-errors": "^1.3.0",
        "es-object-atoms": "^1.0.0",
        "get-intrinsic": "^1.2.7",
        "get-proto": "^1.0.1",
        "which-builtin-type": "^1.2.1"
      },
      "engines": {
        "node": ">= 0.4"
      },
      "funding": {
        "url": "https://github.com/sponsors/ljharb"
      }
    },
    "node_modules/regenerator-runtime": {
      "version": "0.13.11",
      "resolved": "https://registry.npmjs.org/regenerator-runtime/-/regenerator-runtime-0.13.11.tgz",
      "integrity": "sha512-kY1AZVr2Ra+t+piVaJ4gxaFaReZVH40AKNo7UCX6W+dEwBo/2oZJzqfuN1qLq1oL45o56cPaTXELwrTh8Fpggg==",
      "license": "MIT",
      "optional": true
    },
    "node_modules/regexp.prototype.flags": {
      "version": "1.5.4",
      "resolved": "https://registry.npmjs.org/regexp.prototype.flags/-/regexp.prototype.flags-1.5.4.tgz",
      "integrity": "sha512-dYqgNSZbDwkaJ2ceRd9ojCGjBq+mOm9LmtXnAnEGyHhN/5R7iDW2TRw3h+o/jCFxus3P2LfWIIiwowAjANm7IA==",
      "license": "MIT",
      "dependencies": {
        "call-bind": "^1.0.8",
        "define-properties": "^1.2.1",
        "es-errors": "^1.3.0",
        "get-proto": "^1.0.1",
        "gopd": "^1.2.0",
        "set-function-name": "^2.0.2"
      },
      "engines": {
        "node": ">= 0.4"
      },
      "funding": {
        "url": "https://github.com/sponsors/ljharb"
      }
    },
    "node_modules/remark-parse": {
      "version": "11.0.0",
      "resolved": "https://registry.npmjs.org/remark-parse/-/remark-parse-11.0.0.tgz",
      "integrity": "sha512-FCxlKLNGknS5ba/1lmpYijMUzX2esxW5xQqjWxw2eHFfS2MSdaHVINFmhjo+qN1WhZhNimq0dZATN9pH0IDrpA==",
      "license": "MIT",
      "dependencies": {
        "@types/mdast": "^4.0.0",
        "mdast-util-from-markdown": "^2.0.0",
        "micromark-util-types": "^2.0.0",
        "unified": "^11.0.0"
      },
      "funding": {
        "type": "opencollective",
        "url": "https://opencollective.com/unified"
      }
    },
    "node_modules/remark-rehype": {
      "version": "11.1.2",
      "resolved": "https://registry.npmjs.org/remark-rehype/-/remark-rehype-11.1.2.tgz",
      "integrity": "sha512-Dh7l57ianaEoIpzbp0PC9UKAdCSVklD8E5Rpw7ETfbTl3FqcOOgq5q2LVDhgGCkaBv7p24JXikPdvhhmHvKMsw==",
      "license": "MIT",
      "dependencies": {
        "@types/hast": "^3.0.0",
        "@types/mdast": "^4.0.0",
        "mdast-util-to-hast": "^13.0.0",
        "unified": "^11.0.0",
        "vfile": "^6.0.0"
      },
      "funding": {
        "type": "opencollective",
        "url": "https://opencollective.com/unified"
      }
    },
    "node_modules/resolve": {
      "version": "2.0.0-next.6",
      "resolved": "https://registry.npmjs.org/resolve/-/resolve-2.0.0-next.6.tgz",
      "integrity": "sha512-3JmVl5hMGtJ3kMmB3zi3DL25KfkCEyy3Tw7Gmw7z5w8M9WlwoPFnIvwChzu1+cF3iaK3sp18hhPz8ANeimdJfA==",
      "dev": true,
      "license": "MIT",
      "dependencies": {
        "es-errors": "^1.3.0",
        "is-core-module": "^2.16.1",
        "node-exports-info": "^1.6.0",
        "object-keys": "^1.1.1",
        "path-parse": "^1.0.7",
        "supports-preserve-symlinks-flag": "^1.0.0"
      },
      "bin": {
        "resolve": "bin/resolve"
      },
      "engines": {
        "node": ">= 0.4"
      },
      "funding": {
        "url": "https://github.com/sponsors/ljharb"
      }
    },
    "node_modules/resolve-from": {
      "version": "4.0.0",
      "resolved": "https://registry.npmjs.org/resolve-from/-/resolve-from-4.0.0.tgz",
      "integrity": "sha512-pb/MYmXstAkysRFx8piNI1tGFNQIFA3vkE3Gq4EuA1dF6gHp/+vgZqsCGJapvy8N3Q+4o7FwvquPJcnZ7RYy4g==",
      "dev": true,
      "license": "MIT",
      "engines": {
        "node": ">=4"
      }
    },
    "node_modules/reusify": {
      "version": "1.1.0",
      "resolved": "https://registry.npmjs.org/reusify/-/reusify-1.1.0.tgz",
      "integrity": "sha512-g6QUff04oZpHs0eG5p83rFLhHeV00ug/Yf9nZM6fLeUrPguBTkTQOdpAWWspMh55TZfVQDPaN3NQJfbVRAxdIw==",
      "license": "MIT",
      "engines": {
        "iojs": ">=1.0.0",
        "node": ">=0.10.0"
      }
    },
    "node_modules/rgbcolor": {
      "version": "1.0.1",
      "resolved": "https://registry.npmjs.org/rgbcolor/-/rgbcolor-1.0.1.tgz",
      "integrity": "sha512-9aZLIrhRaD97sgVhtJOW6ckOEh6/GnvQtdVNfdZ6s67+3/XwLS9lBcQYzEEhYVeUowN7pRzMLsyGhK2i/xvWbw==",
      "license": "MIT OR SEE LICENSE IN FEEL-FREE.md",
      "optional": true,
      "engines": {
        "node": ">= 0.8.15"
      }
    },
    "node_modules/rollup": {
      "version": "4.62.2",
      "resolved": "https://registry.npmjs.org/rollup/-/rollup-4.62.2.tgz",
      "integrity": "sha512-RFnrW4lhXA3s3eqHDZvN654g8OTjzRfqpIRJYczCGB6HzphckVAi/Qh4tbPUbRuDi7s1Llv8g/NspLkttY3gTA==",
      "dev": true,
      "license": "MIT",
      "dependencies": {
        "@types/estree": "1.0.9"
      },
      "bin": {
        "rollup": "dist/bin/rollup"
      },
      "engines": {
        "node": ">=18.0.0",
        "npm": ">=8.0.0"
      },
      "optionalDependencies": {
        "@rollup/rollup-android-arm-eabi": "4.62.2",
        "@rollup/rollup-android-arm64": "4.62.2",
        "@rollup/rollup-darwin-arm64": "4.62.2",
        "@rollup/rollup-darwin-x64": "4.62.2",
        "@rollup/rollup-freebsd-arm64": "4.62.2",
        "@rollup/rollup-freebsd-x64": "4.62.2",
        "@rollup/rollup-linux-arm-gnueabihf": "4.62.2",
        "@rollup/rollup-linux-arm-musleabihf": "4.62.2",
        "@rollup/rollup-linux-arm64-gnu": "4.62.2",
        "@rollup/rollup-linux-arm64-musl": "4.62.2",
        "@rollup/rollup-linux-loong64-gnu": "4.62.2",
        "@rollup/rollup-linux-loong64-musl": "4.62.2",
        "@rollup/rollup-linux-ppc64-gnu": "4.62.2",
        "@rollup/rollup-linux-ppc64-musl": "4.62.2",
        "@rollup/rollup-linux-riscv64-gnu": "4.62.2",
        "@rollup/rollup-linux-riscv64-musl": "4.62.2",
        "@rollup/rollup-linux-s390x-gnu": "4.62.2",
        "@rollup/rollup-linux-x64-gnu": "4.62.2",
        "@rollup/rollup-linux-x64-musl": "4.62.2",
        "@rollup/rollup-openbsd-x64": "4.62.2",
        "@rollup/rollup-openharmony-arm64": "4.62.2",
        "@rollup/rollup-win32-arm64-msvc": "4.62.2",
        "@rollup/rollup-win32-ia32-msvc": "4.62.2",
        "@rollup/rollup-win32-x64-gnu": "4.62.2",
        "@rollup/rollup-win32-x64-msvc": "4.62.2",
        "fsevents": "~2.3.2"
      }
    },
    "node_modules/run-parallel": {
      "version": "1.2.0",
      "resolved": "https://registry.npmjs.org/run-parallel/-/run-parallel-1.2.0.tgz",
      "integrity": "sha512-5l4VyZR86LZ/lDxZTR6jqL8AFE2S0IFLMP26AbjsLVADxHdhB/c0GUsH+y39UfCi3dzz8OlQuPmnaJOMoDHQBA==",
      "funding": [
        {
          "type": "github",
          "url": "https://github.com/sponsors/feross"
        },
        {
          "type": "patreon",
          "url": "https://www.patreon.com/feross"
        },
        {
          "type": "consulting",
          "url": "https://feross.org/support"
        }
      ],
      "license": "MIT",
      "dependencies": {
        "queue-microtask": "^1.2.2"
      }
    },
    "node_modules/safe-array-concat": {
      "version": "1.1.3",
      "resolved": "https://registry.npmjs.org/safe-array-concat/-/safe-array-concat-1.1.3.tgz",
      "integrity": "sha512-AURm5f0jYEOydBj7VQlVvDrjeFgthDdEF5H1dP+6mNpoXOMo1quQqJ4wvJDyRZ9+pO3kGWoOdmV08cSv2aJV6Q==",
      "dev": true,
      "license": "MIT",
      "dependencies": {
        "call-bind": "^1.0.8",
        "call-bound": "^1.0.2",
        "get-intrinsic": "^1.2.6",
        "has-symbols": "^1.1.0",
        "isarray": "^2.0.5"
      },
      "engines": {
        "node": ">=0.4"
      },
      "funding": {
        "url": "https://github.com/sponsors/ljharb"
      }
    },
    "node_modules/safe-push-apply": {
      "version": "1.0.0",
      "resolved": "https://registry.npmjs.org/safe-push-apply/-/safe-push-apply-1.0.0.tgz",
      "integrity": "sha512-iKE9w/Z7xCzUMIZqdBsp6pEQvwuEebH4vdpjcDWnyzaI6yl6O9FHvVpmGelvEHNsoY6wGblkxR6Zty/h00WiSA==",
      "dev": true,
      "license": "MIT",
      "dependencies": {
        "es-errors": "^1.3.0",
        "isarray": "^2.0.5"
      },
      "engines": {
        "node": ">= 0.4"
      },
      "funding": {
        "url": "https://github.com/sponsors/ljharb"
      }
    },
    "node_modules/safe-regex-test": {
      "version": "1.1.0",
      "resolved": "https://registry.npmjs.org/safe-regex-test/-/safe-regex-test-1.1.0.tgz",
      "integrity": "sha512-x/+Cz4YrimQxQccJf5mKEbIa1NzeCRNI5Ecl/ekmlYaampdNLPalVyIcCZNNH3MvmqBugV5TMYZXv0ljslUlaw==",
      "dev": true,
      "license": "MIT",
      "dependencies": {
        "call-bound": "^1.0.2",
        "es-errors": "^1.3.0",
        "is-regex": "^1.2.1"
      },
      "engines": {
        "node": ">= 0.4"
      },
      "funding": {
        "url": "https://github.com/sponsors/ljharb"
      }
    },
    "node_modules/scheduler": {
      "version": "0.23.2",
      "resolved": "https://registry.npmjs.org/scheduler/-/scheduler-0.23.2.tgz",
      "integrity": "sha512-UOShsPwz7NrMUqhR6t0hWjFduvOzbtv7toDH1/hIrfRNIDBnnBWd0CwJTGvTpngVlmwGCdP9/Zl/tVrDqcuYzQ==",
      "license": "MIT",
      "dependencies": {
        "loose-envify": "^1.1.0"
      }
    },
    "node_modules/semver": {
      "version": "6.3.1",
      "resolved": "https://registry.npmjs.org/semver/-/semver-6.3.1.tgz",
      "integrity": "sha512-BR7VvDCVHO+q2xBEWskxS6DJE1qRnb7DxzUrogb71CWoSficBxYsiAGd+Kl0mmq/MprG9yArRkyrQxTO6XjMzA==",
      "dev": true,
      "license": "ISC",
      "bin": {
        "semver": "bin/semver.js"
      }
    },
    "node_modules/set-function-length": {
      "version": "1.2.2",
      "resolved": "https://registry.npmjs.org/set-function-length/-/set-function-length-1.2.2.tgz",
      "integrity": "sha512-pgRc4hJ4/sNjWCSS9AmnS40x3bNMDTknHgL5UaMBTMyJnU90EgWh1Rz+MC9eFu4BuN/UwZjKQuY/1v3rM7HMfg==",
      "license": "MIT",
      "dependencies": {
        "define-data-property": "^1.1.4",
        "es-errors": "^1.3.0",
        "function-bind": "^1.1.2",
        "get-intrinsic": "^1.2.4",
        "gopd": "^1.0.1",
        "has-property-descriptors": "^1.0.2"
      },
      "engines": {
        "node": ">= 0.4"
      }
    },
    "node_modules/set-function-name": {
      "version": "2.0.2",
      "resolved": "https://registry.npmjs.org/set-function-name/-/set-function-name-2.0.2.tgz",
      "integrity": "sha512-7PGFlmtwsEADb0WYyvCMa1t+yke6daIG4Wirafur5kcf+MhUnPms1UeR0CKQdTZD81yESwMHbtn+TR+dMviakQ==",
      "license": "MIT",
      "dependencies": {
        "define-data-property": "^1.1.4",
        "es-errors": "^1.3.0",
        "functions-have-names": "^1.2.3",
        "has-property-descriptors": "^1.0.2"
      },
      "engines": {
        "node": ">= 0.4"
      }
    },
    "node_modules/set-proto": {
      "version": "1.0.0",
      "resolved": "https://registry.npmjs.org/set-proto/-/set-proto-1.0.0.tgz",
      "integrity": "sha512-RJRdvCo6IAnPdsvP/7m6bsQqNnn1FCBX5ZNtFL98MmFF/4xAIJTIg1YbHW5DC2W5SKZanrC6i4HsJqlajw/dZw==",
      "dev": true,
      "license": "MIT",
      "dependencies": {
        "dunder-proto": "^1.0.1",
        "es-errors": "^1.3.0",
        "es-object-atoms": "^1.0.0"
      },
      "engines": {
        "node": ">= 0.4"
      }
    },
    "node_modules/shebang-command": {
      "version": "2.0.0",
      "resolved": "https://registry.npmjs.org/shebang-command/-/shebang-command-2.0.0.tgz",
      "integrity": "sha512-kHxr2zZpYtdmrN1qDjrrX/Z1rR1kG8Dx+gkpK1G4eXmvXswmcE1hTWBWYUzlraYw1/yZp6YuDY77YtvbN0dmDA==",
      "dev": true,
      "license": "MIT",
      "dependencies": {
        "shebang-regex": "^3.0.0"
      },
      "engines": {
        "node": ">=8"
      }
    },
    "node_modules/shebang-regex": {
      "version": "3.0.0",
      "resolved": "https://registry.npmjs.org/shebang-regex/-/shebang-regex-3.0.0.tgz",
      "integrity": "sha512-7++dFhtcx3353uBaq8DDR4NuxBetBzC7ZQOhmTQInHEd6bSrXdiEyzCvG07Z44UYdLShWUyXt5M/yhz8ekcb1A==",
      "dev": true,
      "license": "MIT",
      "engines": {
        "node": ">=8"
      }
    },
    "node_modules/side-channel": {
      "version": "1.1.0",
      "resolved": "https://registry.npmjs.org/side-channel/-/side-channel-1.1.0.tgz",
      "integrity": "sha512-ZX99e6tRweoUXqR+VBrslhda51Nh5MTQwou5tnUDgbtyM0dBgmhEDtWGP/xbKn6hqfPRHujUNwz5fy/wbbhnpw==",
      "dev": true,
      "license": "MIT",
      "dependencies": {
        "es-errors": "^1.3.0",
        "object-inspect": "^1.13.3",
        "side-channel-list": "^1.0.0",
        "side-channel-map": "^1.0.1",
        "side-channel-weakmap": "^1.0.2"
      },
      "engines": {
        "node": ">= 0.4"
      },
      "funding": {
        "url": "https://github.com/sponsors/ljharb"
      }
    },
    "node_modules/side-channel-list": {
      "version": "1.0.0",
      "resolved": "https://registry.npmjs.org/side-channel-list/-/side-channel-list-1.0.0.tgz",
      "integrity": "sha512-FCLHtRD/gnpCiCHEiJLOwdmFP+wzCmDEkc9y7NsYxeF4u7Btsn1ZuwgwJGxImImHicJArLP4R0yX4c2KCrMrTA==",
      "dev": true,
      "license": "MIT",
      "dependencies": {
        "es-errors": "^1.3.0",
        "object-inspect": "^1.13.3"
      },
      "engines": {
        "node": ">= 0.4"
      },
      "funding": {
        "url": "https://github.com/sponsors/ljharb"
      }
    },
    "node_modules/side-channel-map": {
      "version": "1.0.1",
      "resolved": "https://registry.npmjs.org/side-channel-map/-/side-channel-map-1.0.1.tgz",
      "integrity": "sha512-VCjCNfgMsby3tTdo02nbjtM/ewra6jPHmpThenkTYh8pG9ucZ/1P8So4u4FGBek/BjpOVsDCMoLA/iuBKIFXRA==",
      "dev": true,
      "license": "MIT",
      "dependencies": {
        "call-bound": "^1.0.2",
        "es-errors": "^1.3.0",
        "get-intrinsic": "^1.2.5",
        "object-inspect": "^1.13.3"
      },
      "engines": {
        "node": ">= 0.4"
      },
      "funding": {
        "url": "https://github.com/sponsors/ljharb"
      }
    },
    "node_modules/side-channel-weakmap": {
      "version": "1.0.2",
      "resolved": "https://registry.npmjs.org/side-channel-weakmap/-/side-channel-weakmap-1.0.2.tgz",
      "integrity": "sha512-WPS/HvHQTYnHisLo9McqBHOJk2FkHO/tlpvldyrnem4aeQp4hai3gythswg6p01oSoTl58rcpiFAjF2br2Ak2A==",
      "dev": true,
      "license": "MIT",
      "dependencies": {
        "call-bound": "^1.0.2",
        "es-errors": "^1.3.0",
        "get-intrinsic": "^1.2.5",
        "object-inspect": "^1.13.3",
        "side-channel-map": "^1.0.1"
      },
      "engines": {
        "node": ">= 0.4"
      },
      "funding": {
        "url": "https://github.com/sponsors/ljharb"
      }
    },
    "node_modules/socket.io-client": {
      "version": "4.8.3",
      "resolved": "https://registry.npmjs.org/socket.io-client/-/socket.io-client-4.8.3.tgz",
      "integrity": "sha512-uP0bpjWrjQmUt5DTHq9RuoCBdFJF10cdX9X+a368j/Ft0wmaVgxlrjvK3kjvgCODOMMOz9lcaRzxmso0bTWZ/g==",
      "license": "MIT",
      "dependencies": {
        "@socket.io/component-emitter": "~3.1.0",
        "debug": "~4.4.1",
        "engine.io-client": "~6.6.1",
        "socket.io-parser": "~4.2.4"
      },
      "engines": {
        "node": ">=10.0.0"
      }
    },
    "node_modules/socket.io-parser": {
      "version": "4.2.6",
      "resolved": "https://registry.npmjs.org/socket.io-parser/-/socket.io-parser-4.2.6.tgz",
      "integrity": "sha512-asJqbVBDsBCJx0pTqw3WfesSY0iRX+2xzWEWzrpcH7L6fLzrhyF8WPI8UaeM4YCuDfpwA/cgsdugMsmtz8EJeg==",
      "license": "MIT",
      "dependencies": {
        "@socket.io/component-emitter": "~3.1.0",
        "debug": "~4.4.1"
      },
      "engines": {
        "node": ">=10.0.0"
      }
    },
    "node_modules/sonner": {
      "version": "2.0.7",
      "resolved": "https://registry.npmjs.org/sonner/-/sonner-2.0.7.tgz",
      "integrity": "sha512-W6ZN4p58k8aDKA4XPcx2hpIQXBRAgyiWVkYhT7CvK6D3iAu7xjvVyhQHg2/iaKJZ1XVJ4r7XuwGL+WGEK37i9w==",
      "license": "MIT",
      "peerDependencies": {
        "react": "^18.0.0 || ^19.0.0 || ^19.0.0-rc",
        "react-dom": "^18.0.0 || ^19.0.0 || ^19.0.0-rc"
      }
    },
    "node_modules/source-map-js": {
      "version": "1.2.1",
      "resolved": "https://registry.npmjs.org/source-map-js/-/source-map-js-1.2.1.tgz",
      "integrity": "sha512-UXWMKhLOwVKb728IUtQPXxfYU+usdybtUrK/8uGE8CQMvrhOpwvzDBwj0QhSL7MQc7vIsISBG8VQ8+IDQxpfQA==",
      "license": "BSD-3-Clause",
      "engines": {
        "node": ">=0.10.0"
      }
    },
    "node_modules/space-separated-tokens": {
      "version": "2.0.2",
      "resolved": "https://registry.npmjs.org/space-separated-tokens/-/space-separated-tokens-2.0.2.tgz",
      "integrity": "sha512-PEGlAwrG8yXGXRjW32fGbg66JAlOAwbObuqVoJpv/mRgoWDQfgH1wDPvtzWyUSNAXBGSk8h755YDbbcEy3SH2Q==",
      "license": "MIT",
      "funding": {
        "type": "github",
        "url": "https://github.com/sponsors/wooorm"
      }
    },
    "node_modules/stackblur-canvas": {
      "version": "2.7.0",
      "resolved": "https://registry.npmjs.org/stackblur-canvas/-/stackblur-canvas-2.7.0.tgz",
      "integrity": "sha512-yf7OENo23AGJhBriGx0QivY5JP6Y1HbrrDI6WLt6C5auYZXlQrheoY8hD4ibekFKz1HOfE48Ww8kMWMnJD/zcQ==",
      "license": "MIT",
      "optional": true,
      "engines": {
        "node": ">=0.1.14"
      }
    },
    "node_modules/stop-iteration-iterator": {
      "version": "1.1.0",
      "resolved": "https://registry.npmjs.org/stop-iteration-iterator/-/stop-iteration-iterator-1.1.0.tgz",
      "integrity": "sha512-eLoXW/DHyl62zxY4SCaIgnRhuMr6ri4juEYARS8E6sCEqzKpOiE521Ucofdx+KnDZl5xmvGYaaKCk5FEOxJCoQ==",
      "dev": true,
      "license": "MIT",
      "dependencies": {
        "es-errors": "^1.3.0",
        "internal-slot": "^1.1.0"
      },
      "engines": {
        "node": ">= 0.4"
      }
    },
    "node_modules/string.prototype.matchall": {
      "version": "4.0.12",
      "resolved": "https://registry.npmjs.org/string.prototype.matchall/-/string.prototype.matchall-4.0.12.tgz",
      "integrity": "sha512-6CC9uyBL+/48dYizRf7H7VAYCMCNTBeM78x/VTUe9bFEaxBepPJDa1Ow99LqI/1yF7kuy7Q3cQsYMrcjGUcskA==",
      "dev": true,
      "license": "MIT",
      "dependencies": {
        "call-bind": "^1.0.8",
        "call-bound": "^1.0.3",
        "define-properties": "^1.2.1",
        "es-abstract": "^1.23.6",
        "es-errors": "^1.3.0",
        "es-object-atoms": "^1.0.0",
        "get-intrinsic": "^1.2.6",
        "gopd": "^1.2.0",
        "has-symbols": "^1.1.0",
        "internal-slot": "^1.1.0",
        "regexp.prototype.flags": "^1.5.3",
        "set-function-name": "^2.0.2",
        "side-channel": "^1.1.0"
      },
      "engines": {
        "node": ">= 0.4"
      },
      "funding": {
        "url": "https://github.com/sponsors/ljharb"
      }
    },
    "node_modules/string.prototype.repeat": {
      "version": "1.0.0",
      "resolved": "https://registry.npmjs.org/string.prototype.repeat/-/string.prototype.repeat-1.0.0.tgz",
      "integrity": "sha512-0u/TldDbKD8bFCQ/4f5+mNRrXwZ8hg2w7ZR8wa16e8z9XpePWl3eGEcUD0OXpEH/VJH/2G3gjUtR3ZOiBe2S/w==",
      "dev": true,
      "license": "MIT",
      "dependencies": {
        "define-properties": "^1.1.3",
        "es-abstract": "^1.17.5"
      }
    },
    "node_modules/string.prototype.trim": {
      "version": "1.2.10",
      "resolved": "https://registry.npmjs.org/string.prototype.trim/-/string.prototype.trim-1.2.10.tgz",
      "integrity": "sha512-Rs66F0P/1kedk5lyYyH9uBzuiI/kNRmwJAR9quK6VOtIpZ2G+hMZd+HQbbv25MgCA6gEffoMZYxlTod4WcdrKA==",
      "dev": true,
      "license": "MIT",
      "dependencies": {
        "call-bind": "^1.0.8",
        "call-bound": "^1.0.2",
        "define-data-property": "^1.1.4",
        "define-properties": "^1.2.1",
        "es-abstract": "^1.23.5",
        "es-object-atoms": "^1.0.0",
        "has-property-descriptors": "^1.0.2"
      },
      "engines": {
        "node": ">= 0.4"
      },
      "funding": {
        "url": "https://github.com/sponsors/ljharb"
      }
    },
    "node_modules/string.prototype.trimend": {
      "version": "1.0.9",
      "resolved": "https://registry.npmjs.org/string.prototype.trimend/-/string.prototype.trimend-1.0.9.tgz",
      "integrity": "sha512-G7Ok5C6E/j4SGfyLCloXTrngQIQU3PWtXGst3yM7Bea9FRURf1S42ZHlZZtsNque2FN2PoUhfZXYLNWwEr4dLQ==",
      "dev": true,
      "license": "MIT",
      "dependencies": {
        "call-bind": "^1.0.8",
        "call-bound": "^1.0.2",
        "define-properties": "^1.2.1",
        "es-object-atoms": "^1.0.0"
      },
      "engines": {
        "node": ">= 0.4"
      },
      "funding": {
        "url": "https://github.com/sponsors/ljharb"
      }
    },
    "node_modules/string.prototype.trimstart": {
      "version": "1.0.8",
      "resolved": "https://registry.npmjs.org/string.prototype.trimstart/-/string.prototype.trimstart-1.0.8.tgz",
      "integrity": "sha512-UXSH262CSZY1tfu3G3Secr6uGLCFVPMhIqHjlgCUtCCcgihYc/xKs9djMTMUOb2j1mVSeU8EU6NWc/iQKU6Gfg==",
      "dev": true,
      "license": "MIT",
      "dependencies": {
        "call-bind": "^1.0.7",
        "define-properties": "^1.2.1",
        "es-object-atoms": "^1.0.0"
      },
      "engines": {
        "node": ">= 0.4"
      },
      "funding": {
        "url": "https://github.com/sponsors/ljharb"
      }
    },
    "node_modules/stringify-entities": {
      "version": "4.0.4",
      "resolved": "https://registry.npmjs.org/stringify-entities/-/stringify-entities-4.0.4.tgz",
      "integrity": "sha512-IwfBptatlO+QCJUo19AqvrPNqlVMpW9YEL2LIVY+Rpv2qsjCGxaDLNRgeGsQWJhfItebuJhsGSLjaBbNSQ+ieg==",
      "license": "MIT",
      "dependencies": {
        "character-entities-html4": "^2.0.0",
        "character-entities-legacy": "^3.0.0"
      },
      "funding": {
        "type": "github",
        "url": "https://github.com/sponsors/wooorm"
      }
    },
    "node_modules/strip-json-comments": {
      "version": "3.1.1",
      "resolved": "https://registry.npmjs.org/strip-json-comments/-/strip-json-comments-3.1.1.tgz",
      "integrity": "sha512-6fPc+R4ihwqP6N/aIv2f1gMH8lOVtWQHoqC4yK6oSDVVocumAsfCqjkXnqiYMhmMwS/mEHLp7Vehlt3ql6lEig==",
      "dev": true,
      "license": "MIT",
      "engines": {
        "node": ">=8"
      },
      "funding": {
        "url": "https://github.com/sponsors/sindresorhus"
      }
    },
    "node_modules/style-to-js": {
      "version": "1.1.21",
      "resolved": "https://registry.npmjs.org/style-to-js/-/style-to-js-1.1.21.tgz",
      "integrity": "sha512-RjQetxJrrUJLQPHbLku6U/ocGtzyjbJMP9lCNK7Ag0CNh690nSH8woqWH9u16nMjYBAok+i7JO1NP2pOy8IsPQ==",
      "license": "MIT",
      "dependencies": {
        "style-to-object": "1.0.14"
      }
    },
    "node_modules/style-to-object": {
      "version": "1.0.14",
      "resolved": "https://registry.npmjs.org/style-to-object/-/style-to-object-1.0.14.tgz",
      "integrity": "sha512-LIN7rULI0jBscWQYaSswptyderlarFkjQ+t79nzty8tcIAceVomEVlLzH5VP4Cmsv6MtKhs7qaAiwlcp+Mgaxw==",
      "license": "MIT",
      "dependencies": {
        "inline-style-parser": "0.2.7"
      }
    },
    "node_modules/sucrase": {
      "version": "3.35.1",
      "resolved": "https://registry.npmjs.org/sucrase/-/sucrase-3.35.1.tgz",
      "integrity": "sha512-DhuTmvZWux4H1UOnWMB3sk0sbaCVOoQZjv8u1rDoTV0HTdGem9hkAZtl4JZy8P2z4Bg0nT+YMeOFyVr4zcG5Tw==",
      "license": "MIT",
      "dependencies": {
        "@jridgewell/gen-mapping": "^0.3.2",
        "commander": "^4.0.0",
        "lines-and-columns": "^1.1.6",
        "mz": "^2.7.0",
        "pirates": "^4.0.1",
        "tinyglobby": "^0.2.11",
        "ts-interface-checker": "^0.1.9"
      },
      "bin": {
        "sucrase": "bin/sucrase",
        "sucrase-node": "bin/sucrase-node"
      },
      "engines": {
        "node": ">=16 || 14 >=14.17"
      }
    },
    "node_modules/supports-color": {
      "version": "7.2.0",
      "resolved": "https://registry.npmjs.org/supports-color/-/supports-color-7.2.0.tgz",
      "integrity": "sha512-qpCAvRl9stuOHveKsn7HncJRvv501qIacKzQlO/+Lwxc9+0q2wLyv4Dfvt80/DPn2pqOBsJdDiogXGR9+OvwRw==",
      "dev": true,
      "license": "MIT",
      "dependencies": {
        "has-flag": "^4.0.0"
      },
      "engines": {
        "node": ">=8"
      }
    },
    "node_modules/supports-preserve-symlinks-flag": {
      "version": "1.0.0",
      "resolved": "https://registry.npmjs.org/supports-preserve-symlinks-flag/-/supports-preserve-symlinks-flag-1.0.0.tgz",
      "integrity": "sha512-ot0WnXS9fgdkgIcePe6RHNk1WA8+muPa6cSjeR3V8K27q9BB1rTE3R1p7Hv0z1ZyAc8s6Vvv8DIyWf681MAt0w==",
      "license": "MIT",
      "engines": {
        "node": ">= 0.4"
      },
      "funding": {
        "url": "https://github.com/sponsors/ljharb"
      }
    },
    "node_modules/svg-pathdata": {
      "version": "6.0.3",
      "resolved": "https://registry.npmjs.org/svg-pathdata/-/svg-pathdata-6.0.3.tgz",
      "integrity": "sha512-qsjeeq5YjBZ5eMdFuUa4ZosMLxgr5RZ+F+Y1OrDhuOCEInRMA3x74XdBtggJcj9kOeInz0WE+LgCPDkZFlBYJw==",
      "license": "MIT",
      "optional": true,
      "engines": {
        "node": ">=12.0.0"
      }
    },
    "node_modules/tailwind-merge": {
      "version": "3.5.0",
      "resolved": "https://registry.npmjs.org/tailwind-merge/-/tailwind-merge-3.5.0.tgz",
      "integrity": "sha512-I8K9wewnVDkL1NTGoqWmVEIlUcB9gFriAEkXkfCjX5ib8ezGxtR3xD7iZIxrfArjEsH7F1CHD4RFUtxefdqV/A==",
      "license": "MIT",
      "funding": {
        "type": "github",
        "url": "https://github.com/sponsors/dcastil"
      }
    },
    "node_modules/tailwindcss": {
      "version": "3.4.19",
      "resolved": "https://registry.npmjs.org/tailwindcss/-/tailwindcss-3.4.19.tgz",
      "integrity": "sha512-3ofp+LL8E+pK/JuPLPggVAIaEuhvIz4qNcf3nA1Xn2o/7fb7s/TYpHhwGDv1ZU3PkBluUVaF8PyCHcm48cKLWQ==",
      "license": "MIT",
      "dependencies": {
        "@alloc/quick-lru": "^5.2.0",
        "arg": "^5.0.2",
        "chokidar": "^3.6.0",
        "didyoumean": "^1.2.2",
        "dlv": "^1.1.3",
        "fast-glob": "^3.3.2",
        "glob-parent": "^6.0.2",
        "is-glob": "^4.0.3",
        "jiti": "^1.21.7",
        "lilconfig": "^3.1.3",
        "micromatch": "^4.0.8",
        "normalize-path": "^3.0.0",
        "object-hash": "^3.0.0",
        "picocolors": "^1.1.1",
        "postcss": "^8.4.47",
        "postcss-import": "^15.1.0",
        "postcss-js": "^4.0.1",
        "postcss-load-config": "^4.0.2 || ^5.0 || ^6.0",
        "postcss-nested": "^6.2.0",
        "postcss-selector-parser": "^6.1.2",
        "resolve": "^1.22.8",
        "sucrase": "^3.35.0"
      },
      "bin": {
        "tailwind": "lib/cli.js",
        "tailwindcss": "lib/cli.js"
      },
      "engines": {
        "node": ">=14.0.0"
      }
    },
    "node_modules/tailwindcss-animate": {
      "version": "1.0.7",
      "resolved": "https://registry.npmjs.org/tailwindcss-animate/-/tailwindcss-animate-1.0.7.tgz",
      "integrity": "sha512-bl6mpH3T7I3UFxuvDEXLxy/VuFxBk5bbzplh7tXI68mwMokNYd1t9qPBHlnyTwfa4JGC4zP516I1hYYtQ/vspA==",
      "license": "MIT",
      "peerDependencies": {
        "tailwindcss": ">=3.0.0 || insiders"
      }
    },
    "node_modules/tailwindcss/node_modules/resolve": {
      "version": "1.22.11",
      "resolved": "https://registry.npmjs.org/resolve/-/resolve-1.22.11.tgz",
      "integrity": "sha512-RfqAvLnMl313r7c9oclB1HhUEAezcpLjz95wFH4LVuhk9JF/r22qmVP9AMmOU4vMX7Q8pN8jwNg/CSpdFnMjTQ==",
      "license": "MIT",
      "dependencies": {
        "is-core-module": "^2.16.1",
        "path-parse": "^1.0.7",
        "supports-preserve-symlinks-flag": "^1.0.0"
      },
      "bin": {
        "resolve": "bin/resolve"
      },
      "engines": {
        "node": ">= 0.4"
      },
      "funding": {
        "url": "https://github.com/sponsors/ljharb"
      }
    },
    "node_modules/text-segmentation": {
      "version": "1.0.3",
      "resolved": "https://registry.npmjs.org/text-segmentation/-/text-segmentation-1.0.3.tgz",
      "integrity": "sha512-iOiPUo/BGnZ6+54OsWxZidGCsdU8YbE4PSpdPinp7DeMtUJNJBoJ/ouUSTJjHkh1KntHaltHl/gDs2FC4i5+Nw==",
      "license": "MIT",
      "dependencies": {
        "utrie": "^1.0.2"
      }
    },
    "node_modules/thenify": {
      "version": "3.3.1",
      "resolved": "https://registry.npmjs.org/thenify/-/thenify-3.3.1.tgz",
      "integrity": "sha512-RVZSIV5IG10Hk3enotrhvz0T9em6cyHBLkH/YAZuKqd8hRkKhSfCGIcP2KUY0EPxndzANBmNllzWPwak+bheSw==",
      "license": "MIT",
      "dependencies": {
        "any-promise": "^1.0.0"
      }
    },
    "node_modules/thenify-all": {
      "version": "1.6.0",
      "resolved": "https://registry.npmjs.org/thenify-all/-/thenify-all-1.6.0.tgz",
      "integrity": "sha512-RNxQH/qI8/t3thXJDwcstUO4zeqo64+Uy/+sNVRBx4Xn2OX+OZ9oP+iJnNFqplFra2ZUVeKCSa2oVWi3T4uVmA==",
      "license": "MIT",
      "dependencies": {
        "thenify": ">= 3.1.0 < 4"
      },
      "engines": {
        "node": ">=0.8"
      }
    },
    "node_modules/three": {
      "version": "0.171.0",
      "resolved": "https://registry.npmjs.org/three/-/three-0.171.0.tgz",
      "integrity": "sha512-Y/lAXPaKZPcEdkKjh0JOAHVv8OOnv/NDJqm0wjfCzyQmfKxV7zvkwsnBgPBKTzJHToSOhRGQAGbPJObT59B/PQ==",
      "license": "MIT"
    },
    "node_modules/tiny-invariant": {
      "version": "1.3.3",
      "resolved": "https://registry.npmjs.org/tiny-invariant/-/tiny-invariant-1.3.3.tgz",
      "integrity": "sha512-+FbBPE1o9QAYvviau/qC5SE3caw21q3xkvWKBtja5vgqOWIHHJ3ioaq1VPfn/Szqctz2bU/oYeKd9/z5BL+PVg==",
      "license": "MIT"
    },
    "node_modules/tinyglobby": {
      "version": "0.2.15",
      "resolved": "https://registry.npmjs.org/tinyglobby/-/tinyglobby-0.2.15.tgz",
      "integrity": "sha512-j2Zq4NyQYG5XMST4cbs02Ak8iJUdxRM0XI5QyxXuZOzKOINmWurp3smXu3y5wDcJrptwpSjgXHzIQxR0omXljQ==",
      "license": "MIT",
      "dependencies": {
        "fdir": "^6.5.0",
        "picomatch": "^4.0.3"
      },
      "engines": {
        "node": ">=12.0.0"
      },
      "funding": {
        "url": "https://github.com/sponsors/SuperchupuDev"
      }
    },
    "node_modules/tinyglobby/node_modules/fdir": {
      "version": "6.5.0",
      "resolved": "https://registry.npmjs.org/fdir/-/fdir-6.5.0.tgz",
      "integrity": "sha512-tIbYtZbucOs0BRGqPJkshJUYdL+SDH7dVM8gjy+ERp3WAUjLEFJE+02kanyHtwjWOnwrKYBiwAmM0p4kLJAnXg==",
      "license": "MIT",
      "engines": {
        "node": ">=12.0.0"
      },
      "peerDependencies": {
        "picomatch": "^3 || ^4"
      },
      "peerDependenciesMeta": {
        "picomatch": {
          "optional": true
        }
      }
    },
    "node_modules/tinyglobby/node_modules/picomatch": {
      "version": "4.0.4",
      "resolved": "https://registry.npmjs.org/picomatch/-/picomatch-4.0.4.tgz",
      "integrity": "sha512-QP88BAKvMam/3NxH6vj2o21R6MjxZUAd6nlwAS/pnGvN9IVLocLHxGYIzFhg6fUQ+5th6P4dv4eW9jX3DSIj7A==",
      "license": "MIT",
      "engines": {
        "node": ">=12"
      },
      "funding": {
        "url": "https://github.com/sponsors/jonschlinkert"
      }
    },
    "node_modules/to-regex-range": {
      "version": "5.0.1",
      "resolved": "https://registry.npmjs.org/to-regex-range/-/to-regex-range-5.0.1.tgz",
      "integrity": "sha512-65P7iz6X5yEr1cwcgvQxbbIw7Uk3gOy5dIdtZ4rDveLqhrdJP+Li/Hx6tyK0NEb+2GCyneCMJiGqrADCSNk8sQ==",
      "license": "MIT",
      "dependencies": {
        "is-number": "^7.0.0"
      },
      "engines": {
        "node": ">=8.0"
      }
    },
    "node_modules/trim-lines": {
      "version": "3.0.1",
      "resolved": "https://registry.npmjs.org/trim-lines/-/trim-lines-3.0.1.tgz",
      "integrity": "sha512-kRj8B+YHZCc9kQYdWfJB2/oUl9rA99qbowYYBtr4ui4mZyAQ2JpvVBd/6U2YloATfqBhBTSMhTpgBHtU0Mf3Rg==",
      "license": "MIT",
      "funding": {
        "type": "github",
        "url": "https://github.com/sponsors/wooorm"
      }
    },
    "node_modules/trough": {
      "version": "2.2.0",
      "resolved": "https://registry.npmjs.org/trough/-/trough-2.2.0.tgz",
      "integrity": "sha512-tmMpK00BjZiUyVyvrBK7knerNgmgvcV/KLVyuma/SC+TQN167GrMRciANTz09+k3zW8L8t60jWO1GpfkZdjTaw==",
      "license": "MIT",
      "funding": {
        "type": "github",
        "url": "https://github.com/sponsors/wooorm"
      }
    },
    "node_modules/ts-interface-checker": {
      "version": "0.1.13",
      "resolved": "https://registry.npmjs.org/ts-interface-checker/-/ts-interface-checker-0.1.13.tgz",
      "integrity": "sha512-Y/arvbn+rrz3JCKl9C4kVNfTfSm2/mEp5FSz5EsZSANGPSlQrpRI5M4PKF+mJnE52jOO90PnPSc3Ur3bTQw0gA==",
      "license": "Apache-2.0"
    },
    "node_modules/tslib": {
      "version": "2.8.1",
      "resolved": "https://registry.npmjs.org/tslib/-/tslib-2.8.1.tgz",
      "integrity": "sha512-oJFu94HQb+KVduSUQL7wnpmqnfmLsOA/nAh6b6EH0wCEoK0/mPeXU6c3wKDV83MkOuHPRHtSXKKU99IBazS/2w==",
      "license": "0BSD"
    },
    "node_modules/type-check": {
      "version": "0.4.0",
      "resolved": "https://registry.npmjs.org/type-check/-/type-check-0.4.0.tgz",
      "integrity": "sha512-XleUoc9uwGXqjWwXaUTZAmzMcFZ5858QA2vvx1Ur5xIcixXIP+8LnFDgRplU30us6teqdlskFfu+ae4K79Ooew==",
      "dev": true,
      "license": "MIT",
      "dependencies": {
        "prelude-ls": "^1.2.1"
      },
      "engines": {
        "node": ">= 0.8.0"
      }
    },
    "node_modules/typed-array-buffer": {
      "version": "1.0.3",
      "resolved": "https://registry.npmjs.org/typed-array-buffer/-/typed-array-buffer-1.0.3.tgz",
      "integrity": "sha512-nAYYwfY3qnzX30IkA6AQZjVbtK6duGontcQm1WSG1MD94YLqK0515GNApXkoxKOWMusVssAHWLh9SeaoefYFGw==",
      "dev": true,
      "license": "MIT",
      "dependencies": {
        "call-bound": "^1.0.3",
        "es-errors": "^1.3.0",
        "is-typed-array": "^1.1.14"
      },
      "engines": {
        "node": ">= 0.4"
      }
    },
    "node_modules/typed-array-byte-length": {
      "version": "1.0.3",
      "resolved": "https://registry.npmjs.org/typed-array-byte-length/-/typed-array-byte-length-1.0.3.tgz",
      "integrity": "sha512-BaXgOuIxz8n8pIq3e7Atg/7s+DpiYrxn4vdot3w9KbnBhcRQq6o3xemQdIfynqSeXeDrF32x+WvfzmOjPiY9lg==",
      "dev": true,
      "license": "MIT",
      "dependencies": {
        "call-bind": "^1.0.8",
        "for-each": "^0.3.3",
        "gopd": "^1.2.0",
        "has-proto": "^1.2.0",
        "is-typed-array": "^1.1.14"
      },
      "engines": {
        "node": ">= 0.4"
      },
      "funding": {
        "url": "https://github.com/sponsors/ljharb"
      }
    },
    "node_modules/typed-array-byte-offset": {
      "version": "1.0.4",
      "resolved": "https://registry.npmjs.org/typed-array-byte-offset/-/typed-array-byte-offset-1.0.4.tgz",
      "integrity": "sha512-bTlAFB/FBYMcuX81gbL4OcpH5PmlFHqlCCpAl8AlEzMz5k53oNDvN8p1PNOWLEmI2x4orp3raOFB51tv9X+MFQ==",
      "dev": true,
      "license": "MIT",
      "dependencies": {
        "available-typed-arrays": "^1.0.7",
        "call-bind": "^1.0.8",
        "for-each": "^0.3.3",
        "gopd": "^1.2.0",
        "has-proto": "^1.2.0",
        "is-typed-array": "^1.1.15",
        "reflect.getprototypeof": "^1.0.9"
      },
      "engines": {
        "node": ">= 0.4"
      },
      "funding": {
        "url": "https://github.com/sponsors/ljharb"
      }
    },
    "node_modules/typed-array-length": {
      "version": "1.0.7",
      "resolved": "https://registry.npmjs.org/typed-array-length/-/typed-array-length-1.0.7.tgz",
      "integrity": "sha512-3KS2b+kL7fsuk/eJZ7EQdnEmQoaho/r6KUef7hxvltNA5DR8NAUM+8wJMbJyZ4G9/7i3v5zPBIMN5aybAh2/Jg==",
      "dev": true,
      "license": "MIT",
      "dependencies": {
        "call-bind": "^1.0.7",
        "for-each": "^0.3.3",
        "gopd": "^1.0.1",
        "is-typed-array": "^1.1.13",
        "possible-typed-array-names": "^1.0.0",
        "reflect.getprototypeof": "^1.0.6"
      },
      "engines": {
        "node": ">= 0.4"
      },
      "funding": {
        "url": "https://github.com/sponsors/ljharb"
      }
    },
    "node_modules/typescript": {
      "version": "5.9.3",
      "resolved": "https://registry.npmjs.org/typescript/-/typescript-5.9.3.tgz",
      "integrity": "sha512-jl1vZzPDinLr9eUt3J/t7V6FgNEw9QjvBPdysz9KfQDD41fQrC2Y4vKQdiaUpFT4bXlb1RHhLpp8wtm6M5TgSw==",
      "dev": true,
      "license": "Apache-2.0",
      "bin": {
        "tsc": "bin/tsc",
        "tsserver": "bin/tsserver"
      },
      "engines": {
        "node": ">=14.17"
      }
    },
    "node_modules/unbox-primitive": {
      "version": "1.1.0",
      "resolved": "https://registry.npmjs.org/unbox-primitive/-/unbox-primitive-1.1.0.tgz",
      "integrity": "sha512-nWJ91DjeOkej/TA8pXQ3myruKpKEYgqvpw9lz4OPHj/NWFNluYrjbz9j01CJ8yKQd2g4jFoOkINCTW2I5LEEyw==",
      "dev": true,
      "license": "MIT",
      "dependencies": {
        "call-bound": "^1.0.3",
        "has-bigints": "^1.0.2",
        "has-symbols": "^1.1.0",
        "which-boxed-primitive": "^1.1.1"
      },
      "engines": {
        "node": ">= 0.4"
      },
      "funding": {
        "url": "https://github.com/sponsors/ljharb"
      }
    },
    "node_modules/undici-types": {
      "version": "6.21.0",
      "resolved": "https://registry.npmjs.org/undici-types/-/undici-types-6.21.0.tgz",
      "integrity": "sha512-iwDZqg0QAGrg9Rav5H4n0M64c3mkR59cJ6wQp+7C4nI0gsmExaedaYLNO44eT4AtBBwjbTiGPMlt2Md0T9H9JQ==",
      "dev": true,
      "license": "MIT"
    },
    "node_modules/unified": {
      "version": "11.0.5",
      "resolved": "https://registry.npmjs.org/unified/-/unified-11.0.5.tgz",
      "integrity": "sha512-xKvGhPWw3k84Qjh8bI3ZeJjqnyadK+GEFtazSfZv/rKeTkTjOJho6mFqh2SM96iIcZokxiOpg78GazTSg8+KHA==",
      "license": "MIT",
      "dependencies": {
        "@types/unist": "^3.0.0",
        "bail": "^2.0.0",
        "devlop": "^1.0.0",
        "extend": "^3.0.0",
        "is-plain-obj": "^4.0.0",
        "trough": "^2.0.0",
        "vfile": "^6.0.0"
      },
      "funding": {
        "type": "opencollective",
        "url": "https://opencollective.com/unified"
      }
    },
    "node_modules/unist-util-is": {
      "version": "6.0.1",
      "resolved": "https://registry.npmjs.org/unist-util-is/-/unist-util-is-6.0.1.tgz",
      "integrity": "sha512-LsiILbtBETkDz8I9p1dQ0uyRUWuaQzd/cuEeS1hoRSyW5E5XGmTzlwY1OrNzzakGowI9Dr/I8HVaw4hTtnxy8g==",
      "license": "MIT",
      "dependencies": {
        "@types/unist": "^3.0.0"
      },
      "funding": {
        "type": "opencollective",
        "url": "https://opencollective.com/unified"
      }
    },
    "node_modules/unist-util-position": {
      "version": "5.0.0",
      "resolved": "https://registry.npmjs.org/unist-util-position/-/unist-util-position-5.0.0.tgz",
      "integrity": "sha512-fucsC7HjXvkB5R3kTCO7kUjRdrS0BJt3M/FPxmHMBOm8JQi2BsHAHFsy27E0EolP8rp0NzXsJ+jNPyDWvOJZPA==",
      "license": "MIT",
      "dependencies": {
        "@types/unist": "^3.0.0"
      },
      "funding": {
        "type": "opencollective",
        "url": "https://opencollective.com/unified"
      }
    },
    "node_modules/unist-util-stringify-position": {
      "version": "4.0.0",
      "resolved": "https://registry.npmjs.org/unist-util-stringify-position/-/unist-util-stringify-position-4.0.0.tgz",
      "integrity": "sha512-0ASV06AAoKCDkS2+xw5RXJywruurpbC4JZSm7nr7MOt1ojAzvyyaO+UxZf18j8FCF6kmzCZKcAgN/yu2gm2XgQ==",
      "license": "MIT",
      "dependencies": {
        "@types/unist": "^3.0.0"
      },
      "funding": {
        "type": "opencollective",
        "url": "https://opencollective.com/unified"
      }
    },
    "node_modules/unist-util-visit": {
      "version": "5.1.0",
      "resolved": "https://registry.npmjs.org/unist-util-visit/-/unist-util-visit-5.1.0.tgz",
      "integrity": "sha512-m+vIdyeCOpdr/QeQCu2EzxX/ohgS8KbnPDgFni4dQsfSCtpz8UqDyY5GjRru8PDKuYn7Fq19j1CQ+nJSsGKOzg==",
      "license": "MIT",
      "dependencies": {
        "@types/unist": "^3.0.0",
        "unist-util-is": "^6.0.0",
        "unist-util-visit-parents": "^6.0.0"
      },
      "funding": {
        "type": "opencollective",
        "url": "https://opencollective.com/unified"
      }
    },
    "node_modules/unist-util-visit-parents": {
      "version": "6.0.2",
      "resolved": "https://registry.npmjs.org/unist-util-visit-parents/-/unist-util-visit-parents-6.0.2.tgz",
      "integrity": "sha512-goh1s1TBrqSqukSc8wrjwWhL0hiJxgA8m4kFxGlQ+8FYQ3C/m11FcTs4YYem7V664AhHVvgoQLk890Ssdsr2IQ==",
      "license": "MIT",
      "dependencies": {
        "@types/unist": "^3.0.0",
        "unist-util-is": "^6.0.0"
      },
      "funding": {
        "type": "opencollective",
        "url": "https://opencollective.com/unified"
      }
    },
    "node_modules/update-browserslist-db": {
      "version": "1.2.3",
      "resolved": "https://registry.npmjs.org/update-browserslist-db/-/update-browserslist-db-1.2.3.tgz",
      "integrity": "sha512-Js0m9cx+qOgDxo0eMiFGEueWztz+d4+M3rGlmKPT+T4IS/jP4ylw3Nwpu6cpTTP8R1MAC1kF4VbdLt3ARf209w==",
      "dev": true,
      "funding": [
        {
          "type": "opencollective",
          "url": "https://opencollective.com/browserslist"
        },
        {
          "type": "tidelift",
          "url": "https://tidelift.com/funding/github/npm/browserslist"
        },
        {
          "type": "github",
          "url": "https://github.com/sponsors/ai"
        }
      ],
      "license": "MIT",
      "dependencies": {
        "escalade": "^3.2.0",
        "picocolors": "^1.1.1"
      },
      "bin": {
        "update-browserslist-db": "cli.js"
      },
      "peerDependencies": {
        "browserslist": ">= 4.21.0"
      }
    },
    "node_modules/uri-js": {
      "version": "4.4.1",
      "resolved": "https://registry.npmjs.org/uri-js/-/uri-js-4.4.1.tgz",
      "integrity": "sha512-7rKUyy33Q1yc98pQ1DAmLtwX109F7TIfWlW1Ydo8Wl1ii1SeHieeh0HHfPeL2fMXK6z0s8ecKs9frCuLJvndBg==",
      "dev": true,
      "license": "BSD-2-Clause",
      "dependencies": {
        "punycode": "^2.1.0"
      }
    },
    "node_modules/use-callback-ref": {
      "version": "1.3.3",
      "resolved": "https://registry.npmjs.org/use-callback-ref/-/use-callback-ref-1.3.3.tgz",
      "integrity": "sha512-jQL3lRnocaFtu3V00JToYz/4QkNWswxijDaCVNZRiRTO3HQDLsdu1ZtmIUvV4yPp+rvWm5j0y0TG/S61cuijTg==",
      "license": "MIT",
      "dependencies": {
        "tslib": "^2.0.0"
      },
      "engines": {
        "node": ">=10"
      },
      "peerDependencies": {
        "@types/react": "*",
        "react": "^16.8.0 || ^17.0.0 || ^18.0.0 || ^19.0.0 || ^19.0.0-rc"
      },
      "peerDependenciesMeta": {
        "@types/react": {
          "optional": true
        }
      }
    },
    "node_modules/use-memo-one": {
      "version": "1.1.3",
      "resolved": "https://registry.npmjs.org/use-memo-one/-/use-memo-one-1.1.3.tgz",
      "integrity": "sha512-g66/K7ZQGYrI6dy8GLpVcMsBp4s17xNkYJVSMvTEevGy3nDxHOfE6z8BVE22+5G5x7t3+bhzrlTDB7ObrEE0cQ==",
      "license": "MIT",
      "peerDependencies": {
        "react": "^16.8.0 || ^17.0.0 || ^18.0.0"
      }
    },
    "node_modules/use-sidecar": {
      "version": "1.1.3",
      "resolved": "https://registry.npmjs.org/use-sidecar/-/use-sidecar-1.1.3.tgz",
      "integrity": "sha512-Fedw0aZvkhynoPYlA5WXrMCAMm+nSWdZt6lzJQ7Ok8S6Q+VsHmHpRWndVRJ8Be0ZbkfPc5LRYH+5XrzXcEeLRQ==",
      "license": "MIT",
      "dependencies": {
        "detect-node-es": "^1.1.0",
        "tslib": "^2.0.0"
      },
      "engines": {
        "node": ">=10"
      },
      "peerDependencies": {
        "@types/react": "*",
        "react": "^16.8.0 || ^17.0.0 || ^18.0.0 || ^19.0.0 || ^19.0.0-rc"
      },
      "peerDependenciesMeta": {
        "@types/react": {
          "optional": true
        }
      }
    },
    "node_modules/use-sync-external-store": {
      "version": "1.6.0",
      "resolved": "https://registry.npmjs.org/use-sync-external-store/-/use-sync-external-store-1.6.0.tgz",
      "integrity": "sha512-Pp6GSwGP/NrPIrxVFAIkOQeyw8lFenOHijQWkUTrDvrF4ALqylP2C/KCkeS9dpUM3KvYRQhna5vt7IL95+ZQ9w==",
      "license": "MIT",
      "peerDependencies": {
        "react": "^16.8.0 || ^17.0.0 || ^18.0.0 || ^19.0.0"
      }
    },
    "node_modules/util-deprecate": {
      "version": "1.0.2",
      "resolved": "https://registry.npmjs.org/util-deprecate/-/util-deprecate-1.0.2.tgz",
      "integrity": "sha512-EPD5q1uXyFxJpCrLnCc1nHnq3gOa6DZBocAIiI2TaSCA7VCJ1UJDMagCzIkXNsUYfD1daK//LTEQ8xiIbrHtcw==",
      "license": "MIT"
    },
    "node_modules/utrie": {
      "version": "1.0.2",
      "resolved": "https://registry.npmjs.org/utrie/-/utrie-1.0.2.tgz",
      "integrity": "sha512-1MLa5ouZiOmQzUbjbu9VmjLzn1QLXBhwpUa7kdLUQK+KQ5KA9I1vk5U4YHe/X2Ch7PYnJfWuWT+VbuxbGwljhw==",
      "license": "MIT",
      "dependencies": {
        "base64-arraybuffer": "^1.0.2"
      }
    },
    "node_modules/uuid": {
      "version": "13.0.2",
      "resolved": "https://registry.npmjs.org/uuid/-/uuid-13.0.2.tgz",
      "integrity": "sha512-vzi9uRZ926x4XV73S/4qQaTwPXM2JBj6/6lI/byHH1jOpCzb0zDbfytgA9LcN/hzb2l7WQSQnxITOVx5un/wGw==",
      "funding": [
        "https://github.com/sponsors/broofa",
        "https://github.com/sponsors/ctavan"
      ],
      "license": "MIT",
      "bin": {
        "uuid": "dist-node/bin/uuid"
      }
    },
    "node_modules/vaul": {
      "version": "1.1.2",
      "resolved": "https://registry.npmjs.org/vaul/-/vaul-1.1.2.tgz",
      "integrity": "sha512-ZFkClGpWyI2WUQjdLJ/BaGuV6AVQiJ3uELGk3OYtP+B6yCO7Cmn9vPFXVJkRaGkOJu3m8bQMgtyzNHixULceQA==",
      "license": "MIT",
      "dependencies": {
        "@radix-ui/react-dialog": "^1.1.1"
      },
      "peerDependencies": {
        "react": "^16.8 || ^17.0 || ^18.0 || ^19.0.0 || ^19.0.0-rc",
        "react-dom": "^16.8 || ^17.0 || ^18.0 || ^19.0.0 || ^19.0.0-rc"
      }
    },
    "node_modules/vfile": {
      "version": "6.0.3",
      "resolved": "https://registry.npmjs.org/vfile/-/vfile-6.0.3.tgz",
      "integrity": "sha512-KzIbH/9tXat2u30jf+smMwFCsno4wHVdNmzFyL+T/L3UGqqk6JKfVqOFOZEpZSHADH1k40ab6NUIXZq422ov3Q==",
      "license": "MIT",
      "dependencies": {
        "@types/unist": "^3.0.0",
        "vfile-message": "^4.0.0"
      },
      "funding": {
        "type": "opencollective",
        "url": "https://opencollective.com/unified"
      }
    },
    "node_modules/vfile-message": {
      "version": "4.0.3",
      "resolved": "https://registry.npmjs.org/vfile-message/-/vfile-message-4.0.3.tgz",
      "integrity": "sha512-QTHzsGd1EhbZs4AsQ20JX1rC3cOlt/IWJruk893DfLRr57lcnOeMaWG4K0JrRta4mIJZKth2Au3mM3u03/JWKw==",
      "license": "MIT",
      "dependencies": {
        "@types/unist": "^3.0.0",
        "unist-util-stringify-position": "^4.0.0"
      },
      "funding": {
        "type": "opencollective",
        "url": "https://opencollective.com/unified"
      }
    },
    "node_modules/victory-vendor": {
      "version": "36.9.2",
      "resolved": "https://registry.npmjs.org/victory-vendor/-/victory-vendor-36.9.2.tgz",
      "integrity": "sha512-PnpQQMuxlwYdocC8fIJqVXvkeViHYzotI+NJrCuav0ZYFoq912ZHBk3mCeuj+5/VpodOjPe1z0Fk2ihgzlXqjQ==",
      "license": "MIT AND ISC",
      "dependencies": {
        "@types/d3-array": "^3.0.3",
        "@types/d3-ease": "^3.0.0",
        "@types/d3-interpolate": "^3.0.1",
        "@types/d3-scale": "^4.0.2",
        "@types/d3-shape": "^3.1.0",
        "@types/d3-time": "^3.0.0",
        "@types/d3-timer": "^3.0.0",
        "d3-array": "^3.1.6",
        "d3-ease": "^3.0.1",
        "d3-interpolate": "^3.0.1",
        "d3-scale": "^4.0.2",
        "d3-shape": "^3.1.0",
        "d3-time": "^3.0.0",
        "d3-timer": "^3.0.1"
      }
    },
    "node_modules/vite": {
      "version": "6.4.3",
      "resolved": "https://registry.npmjs.org/vite/-/vite-6.4.3.tgz",
      "integrity": "sha512-NTKlcQjlAK7MlQoyb6LgaqHc8sso/pVyUJYWMws3jg21uTJw/LddqIFPcPqP6PzpgbIcZyKI85sFE4HBrQDA8A==",
      "dev": true,
      "license": "MIT",
      "dependencies": {
        "esbuild": "^0.25.0",
        "fdir": "^6.4.4",
        "picomatch": "^4.0.2",
        "postcss": "^8.5.3",
        "rollup": "^4.34.9",
        "tinyglobby": "^0.2.13"
      },
      "bin": {
        "vite": "bin/vite.js"
      },
      "engines": {
        "node": "^18.0.0 || ^20.0.0 || >=22.0.0"
      },
      "funding": {
        "url": "https://github.com/vitejs/vite?sponsor=1"
      },
      "optionalDependencies": {
        "fsevents": "~2.3.3"
      },
      "peerDependencies": {
        "@types/node": "^18.0.0 || ^20.0.0 || >=22.0.0",
        "jiti": ">=1.21.0",
        "less": "*",
        "lightningcss": "^1.21.0",
        "sass": "*",
        "sass-embedded": "*",
        "stylus": "*",
        "sugarss": "*",
        "terser": "^5.16.0",
        "tsx": "^4.8.1",
        "yaml": "^2.4.2"
      },
      "peerDependenciesMeta": {
        "@types/node": {
          "optional": true
        },
        "jiti": {
          "optional": true
        },
        "less": {
          "optional": true
        },
        "lightningcss": {
          "optional": true
        },
        "sass": {
          "optional": true
        },
        "sass-embedded": {
          "optional": true
        },
        "stylus": {
          "optional": true
        },
        "sugarss": {
          "optional": true
        },
        "terser": {
          "optional": true
        },
        "tsx": {
          "optional": true
        },
        "yaml": {
          "optional": true
        }
      }
    },
    "node_modules/vite/node_modules/fdir": {
      "version": "6.5.0",
      "resolved": "https://registry.npmjs.org/fdir/-/fdir-6.5.0.tgz",
      "integrity": "sha512-tIbYtZbucOs0BRGqPJkshJUYdL+SDH7dVM8gjy+ERp3WAUjLEFJE+02kanyHtwjWOnwrKYBiwAmM0p4kLJAnXg==",
      "dev": true,
      "license": "MIT",
      "engines": {
        "node": ">=12.0.0"
      },
      "peerDependencies": {
        "picomatch": "^3 || ^4"
      },
      "peerDependenciesMeta": {
        "picomatch": {
          "optional": true
        }
      }
    },
    "node_modules/vite/node_modules/picomatch": {
      "version": "4.0.4",
      "resolved": "https://registry.npmjs.org/picomatch/-/picomatch-4.0.4.tgz",
      "integrity": "sha512-QP88BAKvMam/3NxH6vj2o21R6MjxZUAd6nlwAS/pnGvN9IVLocLHxGYIzFhg6fUQ+5th6P4dv4eW9jX3DSIj7A==",
      "dev": true,
      "license": "MIT",
      "engines": {
        "node": ">=12"
      },
      "funding": {
        "url": "https://github.com/sponsors/jonschlinkert"
      }
    },
    "node_modules/which": {
      "version": "2.0.2",
      "resolved": "https://registry.npmjs.org/which/-/which-2.0.2.tgz",
      "integrity": "sha512-BLI3Tl1TW3Pvl70l3yq3Y64i+awpwXqsGBYWkkqMtnbXgrMD+yj7rhW0kuEDxzJaYXGjEW5ogapKNMEKNMjibA==",
      "dev": true,
      "license": "ISC",
      "dependencies": {
        "isexe": "^2.0.0"
      },
      "bin": {
        "node-which": "bin/node-which"
      },
      "engines": {
        "node": ">= 8"
      }
    },
    "node_modules/which-boxed-primitive": {
      "version": "1.1.1",
      "resolved": "https://registry.npmjs.org/which-boxed-primitive/-/which-boxed-primitive-1.1.1.tgz",
      "integrity": "sha512-TbX3mj8n0odCBFVlY8AxkqcHASw3L60jIuF8jFP78az3C2YhmGvqbHBpAjTRH2/xqYunrJ9g1jSyjCjpoWzIAA==",
      "dev": true,
      "license": "MIT",
      "dependencies": {
        "is-bigint": "^1.1.0",
        "is-boolean-object": "^1.2.1",
        "is-number-object": "^1.1.1",
        "is-string": "^1.1.1",
        "is-symbol": "^1.1.1"
      },
      "engines": {
        "node": ">= 0.4"
      },
      "funding": {
        "url": "https://github.com/sponsors/ljharb"
      }
    },
    "node_modules/which-builtin-type": {
      "version": "1.2.1",
      "resolved": "https://registry.npmjs.org/which-builtin-type/-/which-builtin-type-1.2.1.tgz",
      "integrity": "sha512-6iBczoX+kDQ7a3+YJBnh3T+KZRxM/iYNPXicqk66/Qfm1b93iu+yOImkg0zHbj5LNOcNv1TEADiZ0xa34B4q6Q==",
      "dev": true,
      "license": "MIT",
      "dependencies": {
        "call-bound": "^1.0.2",
        "function.prototype.name": "^1.1.6",
        "has-tostringtag": "^1.0.2",
        "is-async-function": "^2.0.0",
        "is-date-object": "^1.1.0",
        "is-finalizationregistry": "^1.1.0",
        "is-generator-function": "^1.0.10",
        "is-regex": "^1.2.1",
        "is-weakref": "^1.0.2",
        "isarray": "^2.0.5",
        "which-boxed-primitive": "^1.1.0",
        "which-collection": "^1.0.2",
        "which-typed-array": "^1.1.16"
      },
      "engines": {
        "node": ">= 0.4"
      },
      "funding": {
        "url": "https://github.com/sponsors/ljharb"
      }
    },
    "node_modules/which-collection": {
      "version": "1.0.2",
      "resolved": "https://registry.npmjs.org/which-collection/-/which-collection-1.0.2.tgz",
      "integrity": "sha512-K4jVyjnBdgvc86Y6BkaLZEN933SwYOuBFkdmBu9ZfkcAbdVbpITnDmjvZ/aQjRXQrv5EPkTnD1s39GiiqbngCw==",
      "dev": true,
      "license": "MIT",
      "dependencies": {
        "is-map": "^2.0.3",
        "is-set": "^2.0.3",
        "is-weakmap": "^2.0.2",
        "is-weakset": "^2.0.3"
      },
      "engines": {
        "node": ">= 0.4"
      },
      "funding": {
        "url": "https://github.com/sponsors/ljharb"
      }
    },
    "node_modules/which-typed-array": {
      "version": "1.1.20",
      "resolved": "https://registry.npmjs.org/which-typed-array/-/which-typed-array-1.1.20.tgz",
      "integrity": "sha512-LYfpUkmqwl0h9A2HL09Mms427Q1RZWuOHsukfVcKRq9q95iQxdw0ix1JQrqbcDR9PH1QDwf5Qo8OZb5lksZ8Xg==",
      "dev": true,
      "license": "MIT",
      "dependencies": {
        "available-typed-arrays": "^1.0.7",
        "call-bind": "^1.0.8",
        "call-bound": "^1.0.4",
        "for-each": "^0.3.5",
        "get-proto": "^1.0.1",
        "gopd": "^1.2.0",
        "has-tostringtag": "^1.0.2"
      },
      "engines": {
        "node": ">= 0.4"
      },
      "funding": {
        "url": "https://github.com/sponsors/ljharb"
      }
    },
    "node_modules/word-wrap": {
      "version": "1.2.5",
      "resolved": "https://registry.npmjs.org/word-wrap/-/word-wrap-1.2.5.tgz",
      "integrity": "sha512-BN22B5eaMMI9UMtjrGd5g5eCYPpCPDUy0FJXbYsaT5zYxjFOckS53SQDE3pWkVoWpHXVb3BrYcEN4Twa55B5cA==",
      "dev": true,
      "license": "MIT",
      "engines": {
        "node": ">=0.10.0"
      }
    },
    "node_modules/ws": {
      "version": "8.21.0",
      "resolved": "https://registry.npmjs.org/ws/-/ws-8.21.0.tgz",
      "integrity": "sha512-Vsp28b7DRcimFQvrqu2Wek3z1iYxDCWqHYB8Qsnk/S4RfaCQzPGPyBNuVjJV3cd6UiKtUtp6sNM77gWvzcCH+g==",
      "license": "MIT",
      "engines": {
        "node": ">=10.0.0"
      },
      "peerDependencies": {
        "bufferutil": "^4.0.1",
        "utf-8-validate": ">=5.0.2"
      },
      "peerDependenciesMeta": {
        "bufferutil": {
          "optional": true
        },
        "utf-8-validate": {
          "optional": true
        }
      }
    },
    "node_modules/xmlhttprequest-ssl": {
      "version": "2.1.2",
      "resolved": "https://registry.npmjs.org/xmlhttprequest-ssl/-/xmlhttprequest-ssl-2.1.2.tgz",
      "integrity": "sha512-TEU+nJVUUnA4CYJFLvK5X9AOeH4KvDvhIfm0vV1GaQRtchnG0hgK5p8hw/xjv8cunWYCsiPCSDzObPyhEwq3KQ==",
      "engines": {
        "node": ">=0.4.0"
      }
    },
    "node_modules/yallist": {
      "version": "3.1.1",
      "resolved": "https://registry.npmjs.org/yallist/-/yallist-3.1.1.tgz",
      "integrity": "sha512-a4UGQaWPH59mOXUYnAG2ewncQS4i4F43Tv3JoAM+s2VDAmS9NsK8GpDMLrCHPksFT7h3K6TOoUNn2pb7RoXx4g==",
      "dev": true,
      "license": "ISC"
    },
    "node_modules/yocto-queue": {
      "version": "0.1.0",
      "resolved": "https://registry.npmjs.org/yocto-queue/-/yocto-queue-0.1.0.tgz",
      "integrity": "sha512-rVksvsnNCdJ/ohGc6xgPwyN8eheCxsiLM8mxuE/t/mOVqJewPuO1miLpTHQiRgTKCLexL4MeAFVagts7HmNZ2Q==",
      "dev": true,
      "license": "MIT",
      "engines": {
        "node": ">=10"
      },
      "funding": {
        "url": "https://github.com/sponsors/sindresorhus"
      }
    },
    "node_modules/zod": {
      "version": "3.25.76",
      "resolved": "https://registry.npmjs.org/zod/-/zod-3.25.76.tgz",
      "integrity": "sha512-gzUt/qt81nXsFGKIFcC3YnfEAx5NkunCfnDlvuBSSFS02bcXu4Lmea0AFIUwbLWxWPx3d9p8S5QoaujKcNQxcQ==",
      "license": "MIT",
      "funding": {
        "url": "https://github.com/sponsors/colinhacks"
      }
    },
    "node_modules/zwitch": {
      "version": "2.0.4",
      "resolved": "https://registry.npmjs.org/zwitch/-/zwitch-2.0.4.tgz",
      "integrity": "sha512-bXE4cR/kVZhKZX/RjPEflHaKVhUVl85noU3v6b8apfQEc1x4A+zBxjZ4lN8LqGd6WZ3dl98pY4o717VFmoPp+A==",
      "license": "MIT",
      "funding": {
        "type": "github",
        "url": "https://github.com/sponsors/wooorm"
      }
    }
  }
}

```

---

## File: `jsconfig.json`

```text
{
  "compilerOptions": {
    "baseUrl": ".",
    "paths": {
      "@/*": ["./src/*"]
    },
    "jsx": "react-jsx",
    "module": "esnext",
    "moduleResolution": "bundler",
    "lib": ["esnext", "dom"],
    "target": "esnext",
    "checkJs": true,
    "skipLibCheck": true,
    "allowSyntheticDefaultImports": true,
    "esModuleInterop": true,
    "resolveJsonModule": true,
    "types": []
  },
  "include": ["src/components/**/*.js", "src/pages/**/*.jsx", "src/Layout.jsx"],
  "exclude": ["node_modules", "dist", "src/vite-plugins", "src/components/ui", "src/api", "src/lib"]
} 
```

---

## File: `CLAUDE.md`

```text
# See AGENTS.md

Follow the instructions in `AGENTS.md`.

```

---

## File: `index.html`

```text
<!doctype html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <link rel="icon" type="image/svg+xml" href="https://base44.com/logo_v2.svg" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <link rel="manifest" href="/manifest.json" />
    <title>Base44 APP</title>
  </head>
  <body>
    <div id="root"></div>
    <script type="module" src="/src/main.jsx"></script>
  </body>
</html>

```

---

## File: `.npmrc`

```text
# Supply-chain cooldown: never install a version published in the last 7 days.
# Maps internally to `before = now - 7 days`, so npm picks the newest version
# that is at least a week old. Applies to `npm install` and `npm audit fix`.
# A freshly-compromised release is most likely to be live (and not yet pulled)
# within its first days, so we skip that window.
min-release-age=7

```

---

## File: `package.json`

```text
{
  "name": "base44-app",
  "private": true,
  "version": "0.0.0",
  "type": "module",
  "scripts": {
    "dev": "vite",
    "build": "vite build",
    "lint": "eslint . --quiet",
    "lint:fix": "eslint . --fix",
    "typecheck": "tsc -p ./jsconfig.json",
    "preview": "vite preview"
  },
  "dependencies": {
    "@base44/sdk": "^0.8.40",
    "@base44/vite-plugin": "^1.0.30",
    "@hello-pangea/dnd": "^17.0.0",
    "@hookform/resolvers": "^4.1.2",
    "@radix-ui/react-accordion": "^1.2.3",
    "@radix-ui/react-alert-dialog": "^1.1.6",
    "@radix-ui/react-aspect-ratio": "^1.1.2",
    "@radix-ui/react-avatar": "^1.1.3",
    "@radix-ui/react-checkbox": "^1.1.4",
    "@radix-ui/react-collapsible": "^1.1.3",
    "@radix-ui/react-context-menu": "^2.2.6",
    "@radix-ui/react-dialog": "^1.1.6",
    "@radix-ui/react-dropdown-menu": "^2.1.6",
    "@radix-ui/react-hover-card": "^1.1.6",
    "@radix-ui/react-label": "^2.1.2",
    "@radix-ui/react-menubar": "^1.1.6",
    "@radix-ui/react-navigation-menu": "^1.2.5",
    "@radix-ui/react-popover": "^1.1.6",
    "@radix-ui/react-progress": "^1.1.2",
    "@radix-ui/react-radio-group": "^1.2.3",
    "@radix-ui/react-scroll-area": "^1.2.3",
    "@radix-ui/react-select": "^2.1.6",
    "@radix-ui/react-separator": "^1.1.2",
    "@radix-ui/react-slider": "^1.2.3",
    "@radix-ui/react-slot": "^1.1.2",
    "@radix-ui/react-switch": "^1.1.3",
    "@radix-ui/react-tabs": "^1.1.3",
    "@radix-ui/react-toast": "^1.2.2",
    "@radix-ui/react-toggle": "^1.1.2",
    "@radix-ui/react-toggle-group": "^1.1.2",
    "@radix-ui/react-tooltip": "^1.1.8",
    "@stripe/react-stripe-js": "^3.0.0",
    "@stripe/stripe-js": "^5.2.0",
    "@tanstack/react-query": "^5.84.1",
    "canvas-confetti": "^1.9.4",
    "class-variance-authority": "^0.7.1",
    "clsx": "^2.1.1",
    "cmdk": "^1.0.0",
    "date-fns": "^3.6.0",
    "embla-carousel-react": "^8.5.2",
    "framer-motion": "^11.16.4",
    "html2canvas": "^1.4.1",
    "input-otp": "^1.4.2",
    "jspdf": "^4.2.1",
    "lodash": "^4.17.21",
    "lucide-react": "^0.475.0",
    "moment": "^2.30.1",
    "next-themes": "^0.4.4",
    "react": "^18.2.0",
    "react-day-picker": "^8.10.1",
    "react-dom": "^18.2.0",
    "react-hook-form": "^7.54.2",
    "react-hot-toast": "^2.6.0",
    "react-leaflet": "^4.2.1",
    "react-markdown": "^9.0.1",
    "react-quill": "^2.0.0",
    "react-resizable-panels": "^2.1.7",
    "react-router-dom": "^6.26.0",
    "recharts": "^2.15.4",
    "sonner": "^2.0.1",
    "tailwind-merge": "^3.0.2",
    "tailwindcss-animate": "^1.0.7",
    "three": "^0.171.0",
    "vaul": "^1.1.2",
    "zod": "^3.24.2"
  },
  "devDependencies": {
    "@eslint/js": "^9.19.0",
    "@types/node": "^22.13.5",
    "@types/react": "^18.2.66",
    "@types/react-dom": "^18.2.22",
    "@vitejs/plugin-react": "^4.3.4",
    "autoprefixer": "^10.4.20",
    "baseline-browser-mapping": "^2.8.32",
    "eslint": "^9.19.0",
    "eslint-plugin-react": "^7.37.4",
    "eslint-plugin-react-hooks": "^5.0.0",
    "eslint-plugin-react-refresh": "^0.4.18",
    "eslint-plugin-unused-imports": "^4.3.0",
    "globals": "^15.14.0",
    "postcss": "^8.5.3",
    "tailwindcss": "^3.4.17",
    "typescript": "^5.8.2",
    "vite": "^6.1.0"
  }
}

```

---

## File: `src/index.css`

```text
@import url('https://fonts.googleapis.com/css2?family=Orbitron:wght@400;500;600;700;800&family=Exo+2:ital,wght@0,300;0,400;0,500;0,600;0,700;1,400&family=Share+Tech+Mono&display=swap');

@tailwind base;
@tailwind components;
@tailwind utilities;

@layer base {
  :root {
    --background: 222 47% 4%;
    --foreground: 190 25% 90%;
    --card: 222 40% 7%;
    --card-foreground: 190 25% 90%;
    --popover: 222 42% 6%;
    --popover-foreground: 190 25% 90%;
    --primary: 38 95% 55%;
    --primary-foreground: 222 47% 5%;
    --secondary: 220 30% 12%;
    --secondary-foreground: 190 25% 90%;
    --muted: 220 30% 12%;
    --muted-foreground: 215 15% 58%;
    --accent: 187 90% 42%;
    --accent-foreground: 222 47% 5%;
    --destructive: 0 84.2% 60.2%;
    --destructive-foreground: 0 0% 98%;
    --border: 218 28% 16%;
    --input: 218 28% 16%;
    --ring: 187 90% 50%;
    --chart-1: 12 76% 61%;
    --chart-2: 173 58% 39%;
    --chart-3: 197 37% 24%;
    --chart-4: 43 74% 66%;
    --chart-5: 27 87% 67%;
    --radius: 0.5rem;
    --font-heading: 'Orbitron', ui-sans-serif, system-ui, sans-serif;
    --font-body: 'Exo 2', ui-sans-serif, system-ui, sans-serif;
    --font-display: 'Orbitron', ui-sans-serif, system-ui, sans-serif;
    --font-mono: 'Share Tech Mono', ui-monospace, SFMono-Regular, Menlo, Monaco, Consolas, "Liberation Mono", "Courier New", monospace;
    --sidebar-background: 0 0% 98%;
    --sidebar-foreground: 240 5.3% 26.1%;
    --sidebar-primary: 240 5.9% 10%;
    --sidebar-primary-foreground: 0 0% 98%;
    --sidebar-accent: 240 4.8% 95.9%;
    --sidebar-accent-foreground: 240 5.9% 10%;
    --sidebar-border: 220 13% 91%;
    --sidebar-ring: 217.2 91.2% 59.8%;
  }

  .dark {
    --background: 222 47% 4%;
    --foreground: 190 25% 90%;
    --card: 222 40% 7%;
    --card-foreground: 190 25% 90%;
    --popover: 222 42% 6%;
    --popover-foreground: 190 25% 90%;
    --primary: 38 95% 55%;
    --primary-foreground: 222 47% 5%;
    --secondary: 220 30% 12%;
    --secondary-foreground: 190 25% 90%;
    --muted: 220 30% 12%;
    --muted-foreground: 215 15% 58%;
    --accent: 187 90% 42%;
    --accent-foreground: 222 47% 5%;
    --destructive: 0 62.8% 30.6%;
    --destructive-foreground: 0 0% 98%;
    --border: 218 28% 16%;
    --input: 218 28% 16%;
    --ring: 187 90% 50%;
    --chart-1: 220 70% 50%;
    --chart-2: 160 60% 45%;
    --chart-3: 30 80% 55%;
    --chart-4: 280 65% 60%;
    --chart-5: 340 75% 55%;
    --sidebar-background: 240 5.9% 10%;
    --sidebar-foreground: 240 4.8% 95.9%;
    --sidebar-primary: 224.3 76.3% 48%;
    --sidebar-primary-foreground: 0 0% 100%;
    --sidebar-accent: 240 3.7% 15.9%;
    --sidebar-accent-foreground: 240 4.8% 95.9%;
    --sidebar-border: 240 3.7% 15.9%;
    --sidebar-ring: 217.2 91.2% 59.8%;
  }
}



@layer base {
  * {
    @apply border-border outline-ring/50;
  }

  body {
    @apply bg-background text-foreground font-body;
  }
}
```

---

## File: `src/App.jsx`

```text
import { Toaster } from "@/components/ui/toaster"
import { QueryClientProvider } from '@tanstack/react-query'
import { queryClientInstance } from '@/lib/query-client'
import { BrowserRouter as Router, Route, Routes } from 'react-router-dom';
import PageNotFound from './lib/PageNotFound';
import { AuthProvider, useAuth } from '@/lib/AuthContext';
import UserNotRegisteredError from '@/components/UserNotRegisteredError';
import ScrollToTop from './components/ScrollToTop';
// Add page imports here
import { Navigate } from 'react-router-dom';
import ProtectedRoute from '@/components/ProtectedRoute';
import Login from './pages/Login';
import Register from './pages/Register';
import ForgotPassword from './pages/ForgotPassword';
import ResetPassword from './pages/ResetPassword';
import Board from './pages/Board';
import PieceDetail from './pages/PieceDetail';
import InstallGuide from './pages/InstallGuide';
import ControlDeck from './pages/ControlDeck';
import CheatSheet from './pages/CheatSheet';
import ReviewBay from './pages/ReviewBay';
import ForgeLink from './pages/ForgeLink';

const AuthenticatedApp = () => {
  const { isLoadingAuth, isLoadingPublicSettings, authError, navigateToLogin } = useAuth();

  // Show loading spinner while checking app public settings or auth
  if (isLoadingPublicSettings || isLoadingAuth) {
    return (
      <div className="fixed inset-0 flex items-center justify-center">
        <div className="w-8 h-8 border-4 border-slate-200 border-t-slate-800 rounded-full animate-spin"></div>
      </div>
    );
  }

  // Handle authentication errors
  if (authError) {
    if (authError.type === 'user_not_registered') {
      return <UserNotRegisteredError />;
    } else if (authError.type === 'auth_required') {
      // Redirect to login automatically
      navigateToLogin();
      return null;
    }
  }

  // Render the main app
  return (
    <Routes>
      {/* Add your page Route elements here */}
      <Route path="/login" element={<Login />} />
      <Route path="/register" element={<Register />} />
      <Route path="/forgot-password" element={<ForgotPassword />} />
      <Route path="/reset-password" element={<ResetPassword />} />
      <Route element={<ProtectedRoute unauthenticatedElement={<Navigate to="/login" replace />} />}>
        <Route path="/" element={<Board />} />
        <Route path="/piece/:id" element={<PieceDetail />} />
        <Route path="/install" element={<InstallGuide />} />
        <Route path="/deck" element={<ControlDeck />} />
        <Route path="/cheatsheet" element={<CheatSheet />} />
        <Route path="/review" element={<ReviewBay />} />
        <Route path="/forge" element={<ForgeLink />} />
      </Route>
      <Route path="*" element={<PageNotFound />} />
    </Routes>
  );
};


function App() {

  return (
    <AuthProvider>
      <QueryClientProvider client={queryClientInstance}>
        <Router>
          <ScrollToTop />
          <AuthenticatedApp />
        </Router>
        <Toaster />
      </QueryClientProvider>
    </AuthProvider>
  )
}

export default App
```

---

## File: `src/main.jsx`

```text
import React from 'react'
import ReactDOM from 'react-dom/client'
import App from '@/App.jsx'
import '@/index.css'

ReactDOM.createRoot(document.getElementById('root')).render(
  <App />
)

```

---

## File: `src/components/GoogleIcon.jsx`

```text
import React from "react";

export default function GoogleIcon({ className = "w-5 h-5" }) {
  return (
    <svg className={className} viewBox="0 0 24 24" aria-hidden="true">
      <path d="M22.56 12.25c0-.78-.07-1.53-.2-2.25H12v4.26h5.92a5.06 5.06 0 01-2.2 3.32v2.77h3.57c2.08-1.92 3.28-4.74 3.28-8.1z" fill="#4285F4" />
      <path d="M12 23c2.97 0 5.46-.98 7.28-2.66l-3.57-2.77c-.98.66-2.23 1.06-3.71 1.06-2.86 0-5.29-1.93-6.16-4.53H2.18v2.84C3.99 20.53 7.7 23 12 23z" fill="#34A853" />
      <path d="M5.84 14.09c-.22-.66-.35-1.36-.35-2.09s.13-1.43.35-2.09V7.07H2.18C1.43 8.55 1 10.22 1 12s.43 3.45 1.18 4.93l2.85-2.22.81-.62z" fill="#FBBC05" />
      <path d="M12 5.38c1.62 0 3.06.56 4.21 1.64l3.15-3.15C17.45 2.09 14.97 1 12 1 7.7 1 3.99 3.47 2.18 7.07l3.66 2.84c.87-2.6 3.3-4.53 6.16-4.53z" fill="#EA4335" />
    </svg>
  );
}

```

---

## File: `src/components/UserNotRegisteredError.jsx`

```text
import React from 'react';

const UserNotRegisteredError = () => {
  return (
    <div className="flex flex-col items-center justify-center min-h-screen bg-gradient-to-b from-white to-slate-50">
      <div className="max-w-md w-full p-8 bg-white rounded-lg shadow-lg border border-slate-100">
        <div className="text-center">
          <div className="inline-flex items-center justify-center w-16 h-16 mb-6 rounded-full bg-orange-100">
            <svg className="w-8 h-8 text-orange-600" fill="none" stroke="currentColor" viewBox="0 0 24 24">
              <path strokeLinecap="round" strokeLinejoin="round" strokeWidth="2" d="M12 9v2m0 4h.01m-6.938 4h13.856c1.54 0 2.502-1.667 1.732-3L13.732 4c-.77-1.333-2.694-1.333-3.464 0L3.34 16c-.77 1.333.192 3 1.732 3z" />
            </svg>
          </div>
          <h1 className="text-3xl font-bold text-slate-900 mb-4">Access Restricted</h1>
          <p className="text-slate-600 mb-8">
            You are not registered to use this application. Please contact the app administrator to request access.
          </p>
          <div className="p-4 bg-slate-50 rounded-md text-sm text-slate-600">
            <p>If you believe this is an error, you can:</p>
            <ul className="list-disc list-inside mt-2 space-y-1">
              <li>Verify you are logged in with the correct account</li>
              <li>Contact the app administrator for access</li>
              <li>Try logging out and back in again</li>
            </ul>
          </div>
        </div>
      </div>
    </div>
  );
};

export default UserNotRegisteredError;

```

---

## File: `src/components/ProtectedRoute.jsx`

```text
import { useEffect } from 'react';
import { Outlet } from 'react-router-dom';
import { useAuth } from '@/lib/AuthContext';
import UserNotRegisteredError from '@/components/UserNotRegisteredError';

const DefaultFallback = () => (
  <div className="fixed inset-0 flex items-center justify-center">
    <div className="w-8 h-8 border-4 border-slate-200 border-t-slate-800 rounded-full animate-spin"></div>
  </div>
);

export default function ProtectedRoute({ fallback = <DefaultFallback />, unauthenticatedElement }) {
  const { isAuthenticated, isLoadingAuth, authChecked, authError, checkUserAuth } = useAuth();

  useEffect(() => {
    if (!authChecked && !isLoadingAuth) {
      checkUserAuth();
    }
  }, [authChecked, isLoadingAuth, checkUserAuth]);

  if (isLoadingAuth || !authChecked) {
    return fallback;
  }

  if (authError) {
    if (authError.type === 'user_not_registered') {
      return <UserNotRegisteredError />;
    }
    return unauthenticatedElement;
  }

  if (!isAuthenticated) {
    return unauthenticatedElement;
  }

  return <Outlet />;
}

```

---

## File: `src/components/AuthLayout.jsx`

```text
import React from "react";

export default function AuthLayout({ icon: Icon, title, subtitle, footer, children }) {
  return (
    <div className="min-h-screen flex items-center justify-center bg-background px-4">
      <div className="w-full max-w-md">
        <div className="text-center mb-10">
          <div className="inline-flex items-center justify-center w-14 h-14 rounded-2xl bg-primary mb-4">
            <Icon className="w-7 h-7 text-primary-foreground" aria-hidden="true" />
          </div>
          <h1 className="text-3xl font-bold tracking-tight text-foreground">{title}</h1>
          {subtitle && <p className="text-muted-foreground mt-2">{subtitle}</p>}
        </div>
        <div className="bg-card rounded-2xl shadow-sm border border-border p-8">
          {children}
        </div>
        {footer && (
          <p className="text-center text-sm text-muted-foreground mt-6">{footer}</p>
        )}
      </div>
    </div>
  );
}

```

---

## File: `src/components/ScrollToTop.jsx`

```text
import { useEffect } from "react";
import { useLocation, useNavigationType } from "react-router-dom";

const getHashId = (hash) => {
  const rawId = hash.slice(1);

  try {
    return decodeURIComponent(rawId);
  } catch {
    return rawId;
  }
};

export default function ScrollToTop() {
  const { pathname, hash } = useLocation();
  const navigationType = useNavigationType();

  useEffect(() => {
    if (navigationType === "POP") return;

    if (hash) {
      const id = getHashId(hash);
      const timer = window.setTimeout(() => {
        document.getElementById(id)?.scrollIntoView({ behavior: "smooth" });
      }, 50);
      return () => window.clearTimeout(timer);
    }

    window.scrollTo({ top: 0, left: 0, behavior: "instant" });
  }, [pathname, hash, navigationType]);

  return null;
}

```

---

## File: `src/components/sockets/ConnectionCard.jsx`

```text
import React, { useState } from "react";
import { base44 } from "@/api/base44Client";
import { getBridgeConfig, saveBridgeConfig, bridgeFetch } from "@/lib/forgeBridge";
import { getConnSecrets, hasConnSecrets, deleteConnSecrets } from "@/lib/connectionVault";
import { kindOf } from "@/components/sockets/socketKinds";
import { Plug, Pin, Trash2, Loader2, KeyRound } from "lucide-react";

const DOT = { ok: "bg-emerald-400", fail: "bg-red-500", unknown: "bg-zinc-600" };

export default function ConnectionCard({ conn, onChanged, onBridged }) {
  const [busy, setBusy] = useState(false);
  const k = kindOf(conn.kind);
  const Icon = k.icon;

  const bridge = async () => {
    setBusy(true);
    const prev = getBridgeConfig();
    const secrets = getConnSecrets(conn.id);
    // Sockets without their own vaulted keys reuse the current live credentials
    saveBridgeConfig({
      url: conn.url,
      token: secrets.token || prev.token,
      cfId: secrets.cfId || prev.cfId,
      cfSecret: secrets.cfSecret || prev.cfSecret,
    });
    let status = "ok", detail = "Bridged and health check passed";
    try {
      const health = await bridgeFetch("/health");
      detail = `Bridged · booted: ${health.booted ? "yes" : "no"}`;
    } catch (e) {
      status = "fail";
      detail = e.message;
      saveBridgeConfig(prev); // don't clobber a working connection with a dead one
    }
    await Promise.all([
      base44.entities.BridgeConnection.update(conn.id, {
        last_status: status,
        last_connected: new Date().toISOString(),
        times_connected: (conn.times_connected || 0) + (status === "ok" ? 1 : 0),
      }),
      base44.entities.ConnectionEvent.create({ connection_id: conn.id, connection_name: conn.name, kind: conn.kind, status, detail }),
    ]);
    setBusy(false);
    onChanged();
    if (status === "ok") onBridged?.();
  };

  const togglePin = async () => {
    await base44.entities.BridgeConnection.update(conn.id, { pinned: !conn.pinned });
    onChanged();
  };

  const remove = async () => {
    deleteConnSecrets(conn.id);
    await base44.entities.BridgeConnection.delete(conn.id);
    onChanged();
  };

  return (
    <div className={`rounded-xl border ${k.border} bg-zinc-900/60 p-4`}>
      <div className="flex items-start justify-between gap-2 mb-2">
        <div className="flex items-center gap-2 min-w-0">
          <Icon className={`h-4 w-4 shrink-0 ${k.text}`} />
          <span className="text-sm text-zinc-100 truncate">{conn.name}</span>
          {hasConnSecrets(conn.id) && <KeyRound className="h-3 w-3 shrink-0 text-amber-400" title="Keys in this browser's vault" />}
        </div>
        <div className="flex items-center gap-1.5 shrink-0">
          <span className={`h-2 w-2 rounded-full ${DOT[conn.last_status] || DOT.unknown}`} />
          <button onClick={togglePin} className={conn.pinned ? "text-amber-400" : "text-zinc-600 hover:text-zinc-400"}>
            <Pin className="h-3.5 w-3.5" />
          </button>
          <button onClick={remove} className="text-zinc-600 hover:text-red-400">
            <Trash2 className="h-3.5 w-3.5" />
          </button>
        </div>
      </div>
      <p className="text-[11px] font-mono text-zinc-500 truncate mb-1">{conn.url}</p>
      {conn.notes && <p className="text-xs text-zinc-500 mb-2 line-clamp-2">{conn.notes}</p>}
      <div className="flex items-center justify-between gap-2 mt-2">
        <span className="text-[10px] font-mono text-zinc-600">
          {conn.times_connected ? `${conn.times_connected}× bridged` : "never bridged"}
          {conn.last_connected ? ` · last ${new Date(conn.last_connected).toLocaleString()}` : ""}
        </span>
        <button
          onClick={bridge}
          disabled={busy}
          className={`inline-flex items-center gap-1.5 rounded-full border ${k.border} ${k.bg} px-3 py-1 text-[11px] font-mono uppercase tracking-wider ${k.text} hover:opacity-80 transition-opacity disabled:opacity-40`}
        >
          {busy ? <Loader2 className="h-3 w-3 animate-spin" /> : <Plug className="h-3 w-3" />} Bridge in
        </button>
      </div>
    </div>
  );
}
```

---

## File: `src/components/sockets/HistoryLog.jsx`

```text
import React from "react";
import { History } from "lucide-react";
import { kindOf } from "@/components/sockets/socketKinds";

export default function HistoryLog({ events }) {
  return (
    <div>
      <div className="flex items-center gap-2 mb-3 text-xs font-mono uppercase tracking-widest text-zinc-500">
        <History className="h-3.5 w-3.5" /> Connection memory
      </div>
      {!events?.length ? (
        <p className="text-zinc-600 font-mono text-xs py-4">No bridge history yet — every connect attempt lands here.</p>
      ) : (
        <div className="space-y-1.5 max-h-72 overflow-y-auto pr-1">
          {events.map((e) => {
            const k = kindOf(e.kind);
            const Icon = k.icon;
            return (
              <div key={e.id} className="flex items-center gap-3 rounded-lg border border-zinc-800/80 bg-zinc-900/40 px-3 py-2">
                <Icon className={`h-3.5 w-3.5 shrink-0 ${k.text}`} />
                <span className={`h-1.5 w-1.5 shrink-0 rounded-full ${e.status === "ok" ? "bg-emerald-400" : "bg-red-500"}`} />
                <span className="text-xs text-zinc-300 truncate">{e.connection_name}</span>
                <span className="text-[10px] font-mono text-zinc-600 truncate flex-1">{e.detail}</span>
                <span className="text-[10px] font-mono text-zinc-600 shrink-0">{new Date(e.created_date).toLocaleString()}</span>
              </div>
            );
          })}
        </div>
      )}
    </div>
  );
}
```

---

## File: `src/components/sockets/SocketDock.jsx`

```text
import React, { useEffect, useState } from "react";
import { base44 } from "@/api/base44Client";
import { saveConnSecrets } from "@/lib/connectionVault";
import { getBridgeConfig } from "@/lib/forgeBridge";
import { Download } from "lucide-react";
import AddConnectionDialog from "@/components/sockets/AddConnectionDialog";
import ConnectionCard from "@/components/sockets/ConnectionCard";
import HistoryLog from "@/components/sockets/HistoryLog";

export default function SocketDock({ onBridged }) {
  const [connections, setConnections] = useState(null);
  const [events, setEvents] = useState([]);

  const load = async () => {
    const [conns, evts] = await Promise.all([
      base44.entities.BridgeConnection.list("-updated_date", 100),
      base44.entities.ConnectionEvent.list("-created_date", 40),
    ]);
    setConnections(conns.sort((a, b) => (b.pinned ? 1 : 0) - (a.pinned ? 1 : 0)));
    setEvents(evts);
  };

  useEffect(() => { load(); }, []);

  const create = async ({ token, cfId, cfSecret, ...meta }) => {
    const record = await base44.entities.BridgeConnection.create(meta);
    if (token || cfId || cfSecret) saveConnSecrets(record.id, { token, cfId, cfSecret });
    load();
  };

  const captureLive = async () => {
    const cfg = getBridgeConfig();
    if (!cfg.url) return;
    let host = cfg.url;
    try { host = new URL(cfg.url).hostname; } catch { /* keep raw */ }
    const record = await base44.entities.BridgeConnection.create({
      name: `Live · ${host}`,
      kind: "forge",
      url: cfg.url,
      notes: "Captured from the active bridge connection.",
      last_status: "ok",
      last_connected: new Date().toISOString(),
      times_connected: 1,
      pinned: true,
    });
    saveConnSecrets(record.id, { token: cfg.token, cfId: cfg.cfId, cfSecret: cfg.cfSecret });
    load();
  };

  return (
    <div className="space-y-8">
      <div className="flex flex-wrap items-center justify-between gap-3">
        <p className="text-xs font-mono text-zinc-500 max-w-xl">
          Socket keychain — register any endpoint (WSL, GitHub bridge, Cloudflare tunnel, GPU offloader…) once,
          then bridge back in with one press. Endpoints live in your database; keys stay in this browser's vault.
        </p>
        <div className="flex items-center gap-2">
          <button
            onClick={captureLive}
            className="inline-flex items-center gap-2 rounded-full border border-emerald-500/40 bg-emerald-500/10 px-4 py-2 text-xs font-mono uppercase tracking-wider text-emerald-400 hover:bg-emerald-500/20 transition-colors"
          >
            <Download className="h-3.5 w-3.5" /> Capture live connection
          </button>
          <AddConnectionDialog onCreate={create} />
        </div>
      </div>

      {!connections ? (
        <div className="flex justify-center py-16">
          <div className="w-8 h-8 border-2 border-zinc-800 border-t-cyan-400 rounded-full animate-spin" />
        </div>
      ) : connections.length === 0 ? (
        <p className="text-zinc-600 text-center py-16 font-mono text-sm">Empty dock — register your first socket.</p>
      ) : (
        <div className="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-4">
          {connections.map((c) => (
            <ConnectionCard key={c.id} conn={c} onChanged={load} onBridged={onBridged} />
          ))}
        </div>
      )}

      <HistoryLog events={events} />
    </div>
  );
}
```

---

## File: `src/components/sockets/socketKinds.js`

```text
import { Terminal, Flame, Github, Cloud, Cpu, Database, Plug } from "lucide-react";

export const SOCKET_KINDS = {
  wsl: { label: "WSL / OS", icon: Terminal, text: "text-emerald-400", border: "border-emerald-500/40", bg: "bg-emerald-500/10" },
  forge: { label: "Forge", icon: Flame, text: "text-amber-400", border: "border-amber-500/40", bg: "bg-amber-500/10" },
  github: { label: "GitHub", icon: Github, text: "text-violet-400", border: "border-violet-500/40", bg: "bg-violet-500/10" },
  cloudflare: { label: "Cloudflare", icon: Cloud, text: "text-orange-400", border: "border-orange-500/40", bg: "bg-orange-500/10" },
  gpu: { label: "GPU Offloader", icon: Cpu, text: "text-cyan-400", border: "border-cyan-500/40", bg: "bg-cyan-500/10" },
  database: { label: "Database", icon: Database, text: "text-sky-400", border: "border-sky-500/40", bg: "bg-sky-500/10" },
  custom: { label: "Custom", icon: Plug, text: "text-zinc-300", border: "border-zinc-600/60", bg: "bg-zinc-700/20" },
};

export const kindOf = (kind) => SOCKET_KINDS[kind] || SOCKET_KINDS.custom;
```

---

## File: `src/components/sockets/AddConnectionDialog.jsx`

```text
import React, { useState } from "react";
import { Dialog, DialogContent, DialogHeader, DialogTitle, DialogTrigger } from "@/components/ui/dialog";
import { Button } from "@/components/ui/button";
import { Input } from "@/components/ui/input";
import { Textarea } from "@/components/ui/textarea";
import { Select, SelectContent, SelectItem, SelectTrigger, SelectValue } from "@/components/ui/select";
import { Plus } from "lucide-react";
import { SOCKET_KINDS } from "@/components/sockets/socketKinds";

const fieldCls = "bg-zinc-900 border-zinc-800 text-zinc-100";
const EMPTY = { name: "", kind: "wsl", url: "", notes: "", token: "", cfId: "", cfSecret: "" };

export default function AddConnectionDialog({ onCreate }) {
  const [open, setOpen] = useState(false);
  const [form, setForm] = useState(EMPTY);
  const set = (k, v) => setForm((f) => ({ ...f, [k]: v }));

  const submit = async () => {
    if (!form.name.trim() || !form.url.trim()) return;
    await onCreate(form);
    setOpen(false);
    setForm(EMPTY);
  };

  return (
    <Dialog open={open} onOpenChange={setOpen}>
      <DialogTrigger asChild>
        <Button className="bg-accent hover:bg-accent/80 text-accent-foreground font-semibold gap-2">
          <Plus className="h-4 w-4" /> New socket
        </Button>
      </DialogTrigger>
      <DialogContent className="bg-zinc-950 border-zinc-800 text-zinc-100">
        <DialogHeader><DialogTitle className="font-heading">Register a socket</DialogTitle></DialogHeader>
        <div className="space-y-3">
          <div className="grid grid-cols-2 gap-3">
            <div>
              <label className="text-xs font-mono text-zinc-500 uppercase">Name</label>
              <Input className={fieldCls} placeholder="e.g. GPU Offloader" value={form.name} onChange={(e) => set("name", e.target.value)} />
            </div>
            <div>
              <label className="text-xs font-mono text-zinc-500 uppercase">Kind</label>
              <Select value={form.kind} onValueChange={(v) => set("kind", v)}>
                <SelectTrigger className={fieldCls}><SelectValue /></SelectTrigger>
                <SelectContent>
                  {Object.entries(SOCKET_KINDS).map(([k, v]) => <SelectItem key={k} value={k}>{v.label}</SelectItem>)}
                </SelectContent>
              </Select>
            </div>
          </div>
          <div>
            <label className="text-xs font-mono text-zinc-500 uppercase">Endpoint URL</label>
            <Input className={fieldCls} placeholder="https://…" value={form.url} onChange={(e) => set("url", e.target.value)} />
          </div>
          <div className="grid grid-cols-3 gap-3">
            <Input className={fieldCls} type="password" placeholder="Token (optional)" value={form.token} onChange={(e) => set("token", e.target.value)} />
            <Input className={fieldCls} placeholder="CF Client ID" value={form.cfId} onChange={(e) => set("cfId", e.target.value)} />
            <Input className={fieldCls} type="password" placeholder="CF Secret" value={form.cfSecret} onChange={(e) => set("cfSecret", e.target.value)} />
          </div>
          <p className="text-[10px] font-mono text-zinc-600">Keys stay in this browser's vault only — never stored in the database.</p>
          <div>
            <label className="text-xs font-mono text-zinc-500 uppercase">Notes</label>
            <Textarea className={fieldCls} rows={2} placeholder="What lives on the other end?" value={form.notes} onChange={(e) => set("notes", e.target.value)} />
          </div>
          <Button onClick={submit} className="w-full bg-accent hover:bg-accent/80 text-accent-foreground font-semibold">Register socket</Button>
        </div>
      </DialogContent>
    </Dialog>
  );
}
```

---

## File: `src/components/deck/NeonToggle.jsx`

```text
import React from "react";
import { NEON } from "@/components/deck/deckColors";

export default function NeonToggle({ control, onChange }) {
  const c = NEON[control.color] || NEON.cyan;
  const on = (control.value ?? 0) >= 1;
  return (
    <button
      onClick={() => onChange(on ? 0 : 1)}
      className={`w-full rounded-xl border p-4 text-left transition-all duration-200 ${
        on ? `${c.border} ${c.bg} ${c.glow}` : "border-zinc-800 bg-zinc-900/70"
      }`}
    >
      <div className="flex items-center justify-between">
        <span className="text-xs font-mono uppercase tracking-widest text-zinc-400">{control.name}</span>
        <span className={`relative inline-flex h-6 w-11 items-center rounded-full transition-colors ${on ? c.fill : "bg-zinc-700"}`}>
          <span className={`inline-block h-4 w-4 rounded-full bg-zinc-950 transition-transform ${on ? "translate-x-6" : "translate-x-1"}`} />
        </span>
      </div>
      <p className={`mt-2 font-mono text-sm ${on ? c.text : "text-zinc-600"}`}>{on ? "ENGAGED" : "OFF"}</p>
    </button>
  );
}
```

---

## File: `src/components/deck/NeonButton.jsx`

```text
import React, { useState } from "react";
import { Zap } from "lucide-react";
import { NEON } from "@/components/deck/deckColors";

export default function NeonButton({ control, onChange }) {
  const c = NEON[control.color] || NEON.cyan;
  const [flash, setFlash] = useState(false);

  const fire = () => {
    onChange((control.value ?? 0) + 1);
    setFlash(true);
    setTimeout(() => setFlash(false), 400);
  };

  return (
    <button
      onClick={fire}
      className={`w-full rounded-xl border ${c.border} p-4 text-left transition-all duration-150 active:scale-[0.97] ${
        flash ? `${c.bg} ${c.glow} ring-2 ${c.ring}` : "bg-zinc-900/70 hover:bg-zinc-900"
      }`}
    >
      <div className="flex items-center justify-between">
        <span className="text-xs font-mono uppercase tracking-widest text-zinc-400">{control.name}</span>
        <Zap className={`h-4 w-4 ${c.text}`} />
      </div>
      <p className={`mt-2 font-mono text-sm ${c.text}`}>FIRE · sent {control.value ?? 0}×</p>
    </button>
  );
}
```

---

## File: `src/components/deck/NeonSlider.jsx`

```text
import React, { useState, useEffect } from "react";
import { Slider } from "@/components/ui/slider";
import { NEON } from "@/components/deck/deckColors";

export default function NeonSlider({ control, onChange }) {
  const c = NEON[control.color] || NEON.cyan;
  const [local, setLocal] = useState(control.value ?? 0);
  useEffect(() => setLocal(control.value ?? 0), [control.value]);

  return (
    <div className={`rounded-xl border ${c.border} bg-zinc-900/70 p-4 ${c.glow}`}>
      <div className="flex items-center justify-between mb-3">
        <span className="text-xs font-mono uppercase tracking-widest text-zinc-400">{control.name}</span>
        <span className={`font-mono text-lg ${c.text}`}>{local}</span>
      </div>
      <Slider
        value={[local]}
        min={control.min ?? 0}
        max={control.max ?? 100}
        step={control.step ?? 1}
        onValueChange={([v]) => setLocal(v)}
        onValueCommit={([v]) => onChange(v)}
        className="[&_[role=slider]]:h-5 [&_[role=slider]]:w-5 [&_[role=slider]]:border-2 [&_[role=slider]]:bg-zinc-950"
      />
      <div className="flex justify-between mt-1.5 text-[10px] font-mono text-zinc-600">
        <span>{control.min ?? 0}</span>
        <span>{control.max ?? 100}</span>
      </div>
    </div>
  );
}
```

---

## File: `src/components/deck/deckColors.js`

```text
export const NEON = {
  cyan: {
    text: "text-cyan-400",
    border: "border-cyan-500/40",
    bg: "bg-cyan-500/10",
    fill: "bg-cyan-400",
    glow: "shadow-[0_0_20px_-4px_rgba(34,211,238,0.6)]",
    ring: "ring-cyan-400/50",
  },
  magenta: {
    text: "text-fuchsia-400",
    border: "border-fuchsia-500/40",
    bg: "bg-fuchsia-500/10",
    fill: "bg-fuchsia-400",
    glow: "shadow-[0_0_20px_-4px_rgba(232,121,249,0.6)]",
    ring: "ring-fuchsia-400/50",
  },
  amber: {
    text: "text-amber-400",
    border: "border-amber-500/40",
    bg: "bg-amber-500/10",
    fill: "bg-amber-400",
    glow: "shadow-[0_0_20px_-4px_rgba(251,191,36,0.6)]",
    ring: "ring-amber-400/50",
  },
  green: {
    text: "text-emerald-400",
    border: "border-emerald-500/40",
    bg: "bg-emerald-500/10",
    fill: "bg-emerald-400",
    glow: "shadow-[0_0_20px_-4px_rgba(52,211,153,0.6)]",
    ring: "ring-emerald-400/50",
  },
  violet: {
    text: "text-violet-400",
    border: "border-violet-500/40",
    bg: "bg-violet-500/10",
    fill: "bg-violet-400",
    glow: "shadow-[0_0_20px_-4px_rgba(167,139,250,0.6)]",
    ring: "ring-violet-400/50",
  },
};
```

---

## File: `src/components/deck/AddControlDialog.jsx`

```text
import React, { useState } from "react";
import { Dialog, DialogContent, DialogHeader, DialogTitle, DialogTrigger } from "@/components/ui/dialog";
import { Button } from "@/components/ui/button";
import { Input } from "@/components/ui/input";
import { Select, SelectContent, SelectItem, SelectTrigger, SelectValue } from "@/components/ui/select";
import { Plus } from "lucide-react";
import { NEON } from "@/components/deck/deckColors";

const fieldCls = "bg-zinc-900 border-zinc-800 text-zinc-100";

export default function AddControlDialog({ onCreate }) {
  const [open, setOpen] = useState(false);
  const [form, setForm] = useState({ name: "", kind: "toggle", section: "Fabric", color: "cyan", min: 0, max: 100, step: 1 });
  const set = (k, v) => setForm((f) => ({ ...f, [k]: v }));

  const submit = async () => {
    if (!form.name.trim()) return;
    await onCreate({ ...form, min: Number(form.min), max: Number(form.max), step: Number(form.step), value: 0 });
    setOpen(false);
    setForm({ name: "", kind: "toggle", section: "Fabric", color: "cyan", min: 0, max: 100, step: 1 });
  };

  return (
    <Dialog open={open} onOpenChange={setOpen}>
      <DialogTrigger asChild>
        <Button className="bg-cyan-600 hover:bg-cyan-500 text-zinc-950 font-semibold gap-2">
          <Plus className="h-4 w-4" /> New control
        </Button>
      </DialogTrigger>
      <DialogContent className="bg-zinc-950 border-zinc-800 text-zinc-100">
        <DialogHeader><DialogTitle className="font-heading">Snap on a new control</DialogTitle></DialogHeader>
        <div className="space-y-3">
          <div>
            <label className="text-xs font-mono text-zinc-500 uppercase">Name</label>
            <Input className={fieldCls} placeholder="e.g. Tap Sensitivity" value={form.name} onChange={(e) => set("name", e.target.value)} />
          </div>
          <div className="grid grid-cols-3 gap-3">
            <div>
              <label className="text-xs font-mono text-zinc-500 uppercase">Type</label>
              <Select value={form.kind} onValueChange={(v) => set("kind", v)}>
                <SelectTrigger className={fieldCls}><SelectValue /></SelectTrigger>
                <SelectContent>
                  <SelectItem value="slider">Slider</SelectItem>
                  <SelectItem value="toggle">Toggle</SelectItem>
                  <SelectItem value="button">Button</SelectItem>
                </SelectContent>
              </Select>
            </div>
            <div>
              <label className="text-xs font-mono text-zinc-500 uppercase">Section</label>
              <Input className={fieldCls} value={form.section} onChange={(e) => set("section", e.target.value)} />
            </div>
            <div>
              <label className="text-xs font-mono text-zinc-500 uppercase">Neon</label>
              <Select value={form.color} onValueChange={(v) => set("color", v)}>
                <SelectTrigger className={fieldCls}><SelectValue /></SelectTrigger>
                <SelectContent>
                  {Object.keys(NEON).map((k) => <SelectItem key={k} value={k}>{k}</SelectItem>)}
                </SelectContent>
              </Select>
            </div>
          </div>
          {form.kind === "slider" && (
            <div className="grid grid-cols-3 gap-3">
              {["min", "max", "step"].map((k) => (
                <div key={k}>
                  <label className="text-xs font-mono text-zinc-500 uppercase">{k}</label>
                  <Input type="number" className={fieldCls} value={form[k]} onChange={(e) => set(k, e.target.value)} />
                </div>
              ))}
            </div>
          )}
          <Button onClick={submit} className="w-full bg-cyan-600 hover:bg-cyan-500 text-zinc-950 font-semibold">Snap it on</Button>
        </div>
      </DialogContent>
    </Dialog>
  );
}
```

---

## File: `src/components/deck/useControls.js`

```text
import { useEffect, useState } from "react";
import { base44 } from "@/api/base44Client";

export default function useControls() {
  const [controls, setControls] = useState(null);

  useEffect(() => {
    base44.entities.ForgeControl.list("created_date", 200).then(setControls);
    const unsubscribe = base44.entities.ForgeControl.subscribe((event) => {
      setControls((prev) => {
        if (!prev) return prev;
        if (event.type === "create") return prev.some((c) => c.id === event.data.id) ? prev : [...prev, event.data];
        if (event.type === "update") return prev.map((c) => (c.id === event.data.id ? event.data : c));
        if (event.type === "delete") return prev.filter((c) => c.id !== event.data.id);
        return prev;
      });
    });
    return unsubscribe;
  }, []);

  const setValue = async (control, value) => {
    setControls((prev) => prev.map((c) => (c.id === control.id ? { ...c, value } : c)));
    await base44.entities.ForgeControl.update(control.id, { value });
  };

  const create = async (data) => base44.entities.ForgeControl.create(data);

  const remove = async (control) => {
    setControls((prev) => prev.filter((c) => c.id !== control.id));
    await base44.entities.ForgeControl.delete(control.id);
  };

  return { controls, setValue, create, remove };
}
```

---

## File: `src/components/deck/BoardControlStrip.jsx`

```text
import React, { useState } from "react";
import { Link } from "react-router-dom";
import { Radio, Trash2 } from "lucide-react";
import useControls from "@/components/deck/useControls";
import NeonSlider from "@/components/deck/NeonSlider";
import NeonToggle from "@/components/deck/NeonToggle";
import NeonButton from "@/components/deck/NeonButton";
import AddControlDialog from "@/components/deck/AddControlDialog";

export default function BoardControlStrip() {
  const { controls, setValue, create, remove } = useControls();
  const [removeMode, setRemoveMode] = useState(false);

  return (
    <section className="mb-10 rounded-2xl border border-accent/30 bg-card/60 p-5 shadow-[0_0_30px_-12px_hsl(var(--accent))]">
      <div className="flex flex-wrap items-center justify-between gap-3 mb-4">
        <div className="flex items-center gap-2 text-xs font-mono uppercase tracking-widest text-accent">
          <Radio className="h-4 w-4 animate-pulse" /> Bridge controls · live sync
        </div>
        <div className="flex items-center gap-2">
          <button
            onClick={() => setRemoveMode((v) => !v)}
            className={`rounded-full border px-3 py-1.5 text-xs font-mono uppercase tracking-wider transition-colors ${
              removeMode ? "border-red-500/60 bg-red-500/10 text-red-400" : "border-border text-muted-foreground hover:border-accent/40"
            }`}
          >
            {removeMode ? "Done" : "Remove"}
          </button>
          <AddControlDialog onCreate={create} />
          <Link to="/deck" className="text-xs font-mono uppercase tracking-wider text-muted-foreground hover:text-accent transition-colors">
            Full deck →
          </Link>
        </div>
      </div>
      {!controls ? (
        <p className="text-muted-foreground text-center py-8 font-mono text-sm">Powering up consoles…</p>
      ) : controls.length === 0 ? (
        <p className="text-muted-foreground text-center py-8 font-mono text-sm">No controls on the bridge yet — snap one on.</p>
      ) : (
        <div className="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-4 gap-3">
          {controls.map((c) => (
            <div key={c.id} className="relative">
              {removeMode && (
                <button
                  onClick={() => remove(c)}
                  className="absolute -top-2 -right-2 z-10 rounded-full bg-red-600 p-1.5 text-white hover:bg-red-500"
                >
                  <Trash2 className="h-3.5 w-3.5" />
                </button>
              )}
              {c.kind === "slider" && <NeonSlider control={c} onChange={(v) => setValue(c, v)} />}
              {c.kind === "toggle" && <NeonToggle control={c} onChange={(v) => setValue(c, v)} />}
              {c.kind === "button" && <NeonButton control={c} onChange={(v) => setValue(c, v)} />}
            </div>
          ))}
        </div>
      )}
    </section>
  );
}
```

---

## File: `src/components/forge/cheatSheet.js`

```text
export const CHEAT_SECTIONS = [
  {
    title: "The Laws (never break these)",
    color: "amber",
    items: [
      ["Deaf by default", "Sections cannot hear each other. Only the overseer's tap hears everything. 'Everyone knows everything' is impossible by design."],
      ["One door", "Every privileged action goes through the Gate — signed, verified, replay-guarded. Even the overseer can't act twice silently."],
      ["Nothing bare", "A raw model is a hostile binary until it's wrapped, sealed, and gated — the baptism."],
      ["Bonded, not fused", "The NPU brain bonds through the VectorConduit. Reclaiming a capsule never erases memory."],
      ["Nothing thrown away", "Retire → archive. The Wardrobe keeps every stripped suit and peeled concept."],
    ],
  },
  {
    title: "The Verbs (what the fabric can do)",
    color: "cyan",
    items: [
      ["Spawn", "Bring a new capsule/section to life inside the fabric."],
      ["Mount", "Attach storage or a resource to a sealed section."],
      ["Egress", "The only sanctioned way anything leaves a section."],
      ["NpuEval", "Send work to the brain seat for judgment."],
      ["Conform", "Seal a raw model into a wrap — the baptism verb."],
      ["Splice", "Cut and recombine substance — multiple models on one body, viewing and commanding each other."],
      ["Reclaim", "Strip a suit back to parts in the Wardrobe; memory survives."],
    ],
  },
  {
    title: "The Control Deck (how to drive it)",
    color: "magenta",
    items: [
      ["Sliders", "DJ-style live dials — drag and release to commit. Values sync in real time to everyone viewing, and to your Forge through the bridge."],
      ["Toggles", "Engage/disengage a mode — tap toggle, deaf mode, NPU seat, sandbox observe."],
      ["Buttons", "Fire a one-shot task — each press counts up, and your Forge treats a count change as a command."],
      ["New control", "Snap on your own slider/toggle/button, name it, pick a section and neon color. LEGO rule: nothing welded in — delete any control anytime."],
      ["The bridge", "Your Forge on the metal polls the deck (Install Guide step 08) and reacts to changes. The deck is codeless; the fabric does the work."],
    ],
  },
  {
    title: "The Rubric (grades)",
    color: "green",
    items: [
      ["🟢 GREEN", "Solid — built and tested."],
      ["🟡 YELLOW", "Needs a look."],
      ["🔴 RED", "Weak or missing."],
      ["🟣 PURPLE", "Revolutionary — seed-stage north star."],
      ["🟠 ORANGE", "Needs custom work."],
    ],
  },
  {
    title: "Order of Operations (don't skip)",
    color: "violet",
    items: [
      ["1. Green tests", "119/119 pass before anything else."],
      ["2. NPU visible", "intel_vpu + Level Zero + OpenVINO show 'NPU'."],
      ["3. Boot", "Kernel bootstrap main.py — the skeleton runs, not just imports."],
      ["4. Real seat", "Swap HeuristicSeat → OpenVINOSeat with bind_seat(). Hot, no reboot."],
      ["5. Bridge", "Connect the Forge to this deck and drive it codeless."],
      ["6. Service", "systemd unit — it survives reboots and breathes on its own."],
    ],
  },
];
```

---

## File: `src/components/forge/installSteps.js`

```text
export const INSTALL_STEPS = [
  {
    title: "Check your metal",
    note: "The Arrow Lake NPU needs kernel 6.8+ (the intel_vpu driver ships in-tree from there). Pop!_OS 22.04+ with a recent kernel qualifies. Verify:",
    blocks: [
      {
        lang: "bash",
        code: `uname -r                      # want 6.8 or newer
python3 --version             # want 3.11+
ls /dev/accel/accel0 2>/dev/null && echo "NPU device node present" || echo "NPU node missing (see Step 4)"
nvidia-smi                    # RTX 5080 sanity check`,
      },
    ],
  },
  {
    title: "Set up the project + environment",
    note: "Unpack forge_ng wherever you keep it (e.g. ~/forge), then create an isolated venv. Nothing global, nothing heavy.",
    blocks: [
      {
        lang: "bash",
        code: `cd ~/forge
python3 -m venv .venv
source .venv/bin/activate
pip install --upgrade pip
pip install pytest            # the fabric itself is stdlib-only by design`,
      },
    ],
  },
  {
    title: "Prove the fabric is green",
    note: "Before touching anything, confirm all 119 tests pass on your machine. If anything is red here, stop and fix it first.",
    blocks: [
      {
        lang: "bash",
        code: `cd ~/forge
source .venv/bin/activate
python -m pytest forge_ng/ -q
# expect: 119 passed`,
      },
    ],
  },
  {
    title: "Wire the NPU (Arrow Lake on Pop!_OS)",
    note: "The NPU stack is three layers: the intel_vpu kernel driver, the Level Zero NPU user-space driver, and OpenVINO as the runtime your NpuSeat binds to. If /dev/accel/accel0 was missing in Step 1, do this:",
    blocks: [
      {
        lang: "bash",
        code: `# 1. Kernel driver (in-tree since 6.8) — load + confirm
sudo modprobe intel_vpu
lsmod | grep intel_vpu
ls /dev/accel/               # want accel0

# 2. Give yourself access to the device node
sudo usermod -aG render $USER   # then log out/in

# 3. Level Zero NPU user-space driver
#    Grab the latest .deb from:
#    https://github.com/intel/linux-npu-driver/releases
sudo apt install ./intel-driver-compiler-npu_*.deb ./intel-level-zero-npu_*.deb
sudo apt install level-zero

# 4. OpenVINO runtime (in your venv)
source ~/forge/.venv/bin/activate
pip install openvino

# 5. Verify the NPU is visible to the runtime
python -c "import openvino as ov; print(ov.Core().available_devices)"
# want: ['CPU', 'GPU', 'NPU']`,
      },
    ],
  },
  {
    title: "Kernel bootstrap — make it BOOT, not just import",
    note: "This is the Skeleton's known gap. Drop this in as forge_ng/main.py and adapt the imports/constructor args to your exact signatures — it assembles the organs, binds a seat, and runs the living tick loop. HeuristicSeat keeps it alive even with no NPU.",
    blocks: [
      {
        lang: "python",
        code: `#!/usr/bin/env python3
"""forge_ng/main.py — kernel bootstrap: the Forge as a living process.

Adapt import paths / constructor args to your exact signatures.
Philosophy preserved: deaf by default, one door, nothing bare.
"""
import signal, sys, time

from forge_ng.fabric.bus import SubstanceBus
from forge_ng.fabric.gate import Gate
from forge_ng.fabric.overseer import Overseer
from forge_ng.fabric.conduit import VectorConduit, HeuristicSeat

TICK_HZ = 2  # light: 2 ticks/sec is plenty; raise only when the NPU seat is real


def build_seat():
    """Try the real NPU; fall back to HeuristicSeat. Never dies for lack of silicon."""
    try:
        import openvino as ov
        core = ov.Core()
        if "NPU" in core.available_devices:
            # TODO: swap in your OpenVINOSeat(NpuSeat) implementation here
            print("[forge] NPU detected — bind OpenVINOSeat when ready; using HeuristicSeat for now")
    except ImportError:
        pass
    return HeuristicSeat()


def main():
    bus = SubstanceBus()
    gate = Gate()
    overseer = Overseer(bus=bus, gate=gate)
    conduit = VectorConduit(overseer=overseer, seat=build_seat())

    running = {"on": True}
    signal.signal(signal.SIGTERM, lambda *_: running.update(on=False))
    signal.signal(signal.SIGINT, lambda *_: running.update(on=False))

    print("[forge] awake — deaf sections sealed, tap live, seat bound")
    while running["on"]:
        conduit.tick()          # FEED UP -> JUDGE -> COMMAND
        time.sleep(1 / TICK_HZ)

    print("[forge] graceful sleep — nothing thrown away")
    return 0


if __name__ == "__main__":
    sys.exit(main())`,
      },
      {
        lang: "bash",
        code: `# boot it
cd ~/forge && source .venv/bin/activate
python -m forge_ng.main`,
      },
    ],
  },
  {
    title: "Bind the real NPU seat",
    note: "Once Step 4 shows 'NPU' in available_devices, implement the NpuSeat protocol on OpenVINO and hot-swap it with bind_seat() — no reboot, LEGO-style. Skeleton to adapt:",
    blocks: [
      {
        lang: "python",
        code: `# forge_ng/fabric/npu_seat.py — real silicon behind the NpuSeat protocol
import openvino as ov


class OpenVINOSeat:
    """Implements the same protocol as HeuristicSeat, judged on the NPU.

    Keep it light: compile ONE small model once, reuse forever.
    A compact embedding/classifier model is the right size for the
    judge role — the 5080 stays free for heavy capsule work.
    """

    def __init__(self, model_path: str, device: str = "NPU"):
        core = ov.Core()
        self._compiled = core.compile_model(model_path, device)

    def judge(self, vectors):
        # Adapt to your seat protocol's exact signature:
        # run inference on the drained tap vectors, return verdicts
        infer = self._compiled.create_infer_request()
        return infer.infer({0: vectors})`,
      },
    ],
  },
  {
    title: "Run it as a service (survives reboot)",
    note: "A systemd user unit keeps the Forge alive as a real resident process — light, auto-restarting, no root.",
    blocks: [
      {
        lang: "bash",
        code: `mkdir -p ~/.config/systemd/user
cat > ~/.config/systemd/user/forge.service <<'EOF'
[Unit]
Description=THE FORGE - local AI fabric

[Service]
WorkingDirectory=%h/forge
ExecStart=%h/forge/.venv/bin/python -m forge_ng.main
Restart=on-failure
RestartSec=3

[Install]
WantedBy=default.target
EOF

systemctl --user daemon-reload
systemctl --user enable --now forge
systemctl --user status forge        # watch it breathe
journalctl --user -u forge -f        # live logs`,
      },
    ],
  },
  {
    title: "The bridge — drive the Forge from the Control Deck",
    note: "This app's Control Deck is your codeless operator console. Your Forge polls the deck's controls over the app's data API and reacts to changes — sliders become live dials, toggles flip modes, button press-counts fire tasks. Get your App ID and an API key from this app's dashboard (Settings → API), then drop this in as forge_ng/bridge.py and call bridge.poll() inside the tick loop.",
    blocks: [
      {
        lang: "python",
        code: `# forge_ng/bridge.py — deaf-section coupler to the Control Deck (read-only pull)
import json, urllib.request

APP_ID = "YOUR_APP_ID"        # from this app's dashboard
API_KEY = "YOUR_API_KEY"      # Settings -> API (keep it secret, keep it local)
URL = f"https://app.base44.com/api/apps/{APP_ID}/entities/ForgeControl"


class DeckBridge:
    """Polls the deck; reports only what CHANGED since last poll.
    The bridge never pushes — one-way pull keeps the attack surface at zero verbs.
    """

    def __init__(self):
        self._last = {}

    def poll(self):
        req = urllib.request.Request(URL, headers={"api_key": API_KEY})
        controls = json.loads(urllib.request.urlopen(req, timeout=5).read())
        changed = []
        for c in controls:
            key = c["id"]
            if self._last.get(key) != c.get("value"):
                self._last[key] = c.get("value")
                changed.append(c)   # {name, kind, section, value, ...}
        return changed


# in main.py's tick loop (poll every ~2s, not every tick):
#   for c in bridge.poll():
#       if c["kind"] == "toggle": overseer.set_mode(c["name"], bool(c["value"]))
#       if c["kind"] == "slider": overseer.set_dial(c["name"], c["value"])
#       if c["kind"] == "button": overseer.fire_task(c["name"])   # count changed = fire once`,
      },
    ],
  },
];
```

---

## File: `src/components/forge/PieceEditForm.jsx`

```text
import React, { useState } from "react";
import { Button } from "@/components/ui/button";
import { Input } from "@/components/ui/input";
import { Textarea } from "@/components/ui/textarea";
import { Select, SelectContent, SelectItem, SelectTrigger, SelectValue } from "@/components/ui/select";
import { GRADES } from "@/components/forge/gradeConfig";

const fieldCls = "bg-zinc-900 border-zinc-800 text-zinc-100 focus-visible:ring-amber-500/50";

export default function PieceEditForm({ piece, onSave, onCancel, saving }) {
  const [form, setForm] = useState({ ...piece });
  const set = (k, v) => setForm((f) => ({ ...f, [k]: v }));

  return (
    <div className="space-y-4">
      <div className="grid grid-cols-1 sm:grid-cols-3 gap-4">
        <div className="sm:col-span-2">
          <label className="text-xs font-mono text-zinc-500 uppercase">Name</label>
          <Input className={fieldCls} value={form.name || ""} onChange={(e) => set("name", e.target.value)} />
        </div>
        <div>
          <label className="text-xs font-mono text-zinc-500 uppercase">Grade</label>
          <Select value={form.grade} onValueChange={(v) => set("grade", v)}>
            <SelectTrigger className={fieldCls}><SelectValue /></SelectTrigger>
            <SelectContent>
              {Object.keys(GRADES).map((g) => (
                <SelectItem key={g} value={g}>{GRADES[g].label}</SelectItem>
              ))}
            </SelectContent>
          </Select>
        </div>
      </div>
      {[
        ["what_it_is", "What it is"],
        ["serves", "What part it serves"],
        ["gaps", "Weak spots / gaps"],
        ["next_brick", "Upgrade / next brick"],
      ].map(([k, label]) => (
        <div key={k}>
          <label className="text-xs font-mono text-zinc-500 uppercase">{label}</label>
          <Textarea className={fieldCls} rows={2} value={form[k] || ""} onChange={(e) => set(k, e.target.value)} />
        </div>
      ))}
      <div className="flex gap-3 pt-2">
        <Button onClick={() => onSave(form)} disabled={saving} className="bg-amber-600 hover:bg-amber-500 text-zinc-950 font-semibold">
          {saving ? "Saving…" : "Save"}
        </Button>
        <Button variant="ghost" onClick={onCancel} className="text-zinc-400 hover:text-zinc-100">Cancel</Button>
      </div>
    </div>
  );
}
```

---

## File: `src/components/forge/GradeBadge.jsx`

```text
import React from "react";
import { GRADES } from "@/components/forge/gradeConfig";

export default function GradeBadge({ grade, small }) {
  const g = GRADES[grade] || GRADES.YELLOW;
  return (
    <span
      className={`inline-flex items-center gap-1.5 rounded-full border ${g.border} ${g.bg} ${g.text} ${
        small ? "px-2 py-0.5 text-[10px]" : "px-3 py-1 text-xs"
      } font-mono tracking-wider uppercase`}
    >
      <span className={`h-1.5 w-1.5 rounded-full ${g.dot} animate-pulse`} />
      {grade}
    </span>
  );
}
```

---

## File: `src/components/forge/CodeBlock.jsx`

```text
import React, { useState } from "react";
import { Copy, Check } from "lucide-react";

export default function CodeBlock({ code, lang }) {
  const [copied, setCopied] = useState(false);
  const copy = async () => {
    await navigator.clipboard.writeText(code);
    setCopied(true);
    setTimeout(() => setCopied(false), 1500);
  };
  return (
    <div className="relative group rounded-lg border border-zinc-800 bg-black/60 overflow-hidden">
      <div className="flex items-center justify-between px-3 py-1.5 border-b border-zinc-800/80 bg-zinc-900/60">
        <span className="text-[10px] font-mono uppercase tracking-widest text-zinc-500">{lang || "bash"}</span>
        <button onClick={copy} className="flex items-center gap-1 text-[10px] font-mono text-zinc-500 hover:text-amber-400 transition-colors">
          {copied ? <Check className="h-3 w-3 text-emerald-400" /> : <Copy className="h-3 w-3" />}
          {copied ? "copied" : "copy"}
        </button>
      </div>
      <pre className="p-4 overflow-x-auto text-[13px] leading-relaxed font-mono text-zinc-300 whitespace-pre">{code}</pre>
    </div>
  );
}
```

---

## File: `src/components/forge/gradeConfig.js`

```text
export const GRADES = {
  GREEN: {
    label: "GREEN · Solid",
    dot: "bg-emerald-400",
    text: "text-emerald-400",
    border: "border-emerald-500/30",
    glow: "shadow-[0_0_24px_-8px_rgba(52,211,153,0.4)]",
    bg: "bg-emerald-500/10",
  },
  YELLOW: {
    label: "YELLOW · Needs a look",
    dot: "bg-yellow-400",
    text: "text-yellow-400",
    border: "border-yellow-500/30",
    glow: "shadow-[0_0_24px_-8px_rgba(250,204,21,0.4)]",
    bg: "bg-yellow-500/10",
  },
  RED: {
    label: "RED · Weak / missing",
    dot: "bg-red-500",
    text: "text-red-400",
    border: "border-red-500/30",
    glow: "shadow-[0_0_24px_-8px_rgba(239,68,68,0.4)]",
    bg: "bg-red-500/10",
  },
  PURPLE: {
    label: "PURPLE · Revolutionary",
    dot: "bg-violet-400",
    text: "text-violet-400",
    border: "border-violet-500/30",
    glow: "shadow-[0_0_24px_-8px_rgba(167,139,250,0.4)]",
    bg: "bg-violet-500/10",
  },
  ORANGE: {
    label: "ORANGE · Needs custom work",
    dot: "bg-orange-400",
    text: "text-orange-400",
    border: "border-orange-500/30",
    glow: "shadow-[0_0_24px_-8px_rgba(251,146,60,0.4)]",
    bg: "bg-orange-500/10",
  },
};

export const GRADE_ORDER = ["GREEN", "YELLOW", "ORANGE", "PURPLE", "RED"];
```

---

## File: `src/components/forge/PieceCard.jsx`

```text
import React from "react";
import { Link } from "react-router-dom";
import { motion } from "framer-motion";
import { Code2, Lightbulb } from "lucide-react";
import GradeBadge from "@/components/forge/GradeBadge";
import { GRADES } from "@/components/forge/gradeConfig";

export default function PieceCard({ piece, index }) {
  const g = GRADES[piece.grade] || GRADES.YELLOW;
  const TypeIcon = piece.piece_type === "Code" ? Code2 : Lightbulb;
  return (
    <motion.div
      initial={{ opacity: 0, y: 16 }}
      animate={{ opacity: 1, y: 0 }}
      transition={{ delay: index * 0.04, duration: 0.4 }}
    >
      <Link
        to={`/piece/${piece.id}`}
        className={`group block h-full rounded-xl border ${g.border} bg-zinc-900/60 p-5 transition-all duration-300 hover:bg-zinc-900 hover:-translate-y-1 hover:${g.glow}`}
      >
        <div className="flex items-start justify-between gap-3 mb-3">
          <div className="flex items-center gap-2 text-zinc-500">
            <span className="font-mono text-xs">{String(piece.order || 0).padStart(2, "0")}</span>
            <TypeIcon className="h-3.5 w-3.5" />
            <span className="text-[10px] uppercase tracking-widest">{piece.piece_type}</span>
          </div>
          <GradeBadge grade={piece.grade} small />
        </div>
        <h3 className="font-heading text-lg text-zinc-100 mb-1.5 group-hover:text-amber-300 transition-colors">
          {piece.name}
        </h3>
        <p className="text-sm text-zinc-400 leading-relaxed line-clamp-2">{piece.what_it_is}</p>
        {piece.next_brick && (
          <p className="mt-3 text-xs font-mono text-amber-500/80 line-clamp-1">→ {piece.next_brick}</p>
        )}
      </Link>
    </motion.div>
  );
}
```

---

## File: `src/components/review/ReviewCard.jsx`

```text
import React, { useState } from "react";
import { ChevronDown, FileCode2, Trash2, AlertTriangle, Wrench, ListChecks } from "lucide-react";
import GradeBadge from "@/components/forge/GradeBadge";
import { GRADES } from "@/components/forge/gradeConfig";

const DIMS = [
  ["code_grade", "Code"],
  ["structure_grade", "Structure"],
  ["security_grade", "Security"],
  ["install_grade", "Install"],
];

const ListBlock = ({ icon: Icon, label, items, tone }) =>
  !items?.length ? null : (
    <div>
      <h4 className={`flex items-center gap-2 text-[11px] font-mono uppercase tracking-widest mb-2 ${tone}`}>
        <Icon className="h-3.5 w-3.5" /> {label}
      </h4>
      <ul className="space-y-1.5">
        {items.map((it, i) => (
          <li key={i} className="text-sm text-zinc-300 leading-relaxed pl-4 relative">
            <span className="absolute left-0 text-zinc-600">·</span>{it}
          </li>
        ))}
      </ul>
    </div>
  );

export default function ReviewCard({ review, onDelete }) {
  const [open, setOpen] = useState(false);
  const g = GRADES[review.overall_grade] || GRADES.YELLOW;

  return (
    <div className={`rounded-xl border ${g.border} bg-zinc-900/60 overflow-hidden`}>
      <button onClick={() => setOpen((v) => !v)} className="w-full p-4 text-left">
        <div className="flex items-center justify-between gap-3">
          <div className="flex items-center gap-3 min-w-0">
            <FileCode2 className={`h-5 w-5 shrink-0 ${g.text}`} />
            <span className="font-mono text-sm text-zinc-100 truncate">{review.file_name}</span>
          </div>
          <div className="flex items-center gap-2 shrink-0">
            <GradeBadge grade={review.overall_grade} />
            <ChevronDown className={`h-4 w-4 text-zinc-500 transition-transform ${open ? "rotate-180" : ""}`} />
          </div>
        </div>
        <p className="mt-2 text-sm text-zinc-400 leading-relaxed">{review.summary}</p>
        <div className="mt-3 flex flex-wrap gap-2">
          {DIMS.map(([key, label]) => {
            const dg = GRADES[review[key]];
            return dg ? (
              <span key={key} className={`rounded-full border px-2.5 py-0.5 text-[10px] font-mono uppercase tracking-wider ${dg.border} ${dg.bg} ${dg.text}`}>
                {label}: {review[key]}
              </span>
            ) : null;
          })}
        </div>
      </button>

      {open && (
        <div className="border-t border-zinc-800/80 p-4 space-y-5">
          <div>
            <h4 className="text-[11px] font-mono uppercase tracking-widest text-zinc-500 mb-2">The Review</h4>
            <p className="text-sm text-zinc-300 leading-relaxed whitespace-pre-wrap">{review.review}</p>
          </div>
          <ListBlock icon={AlertTriangle} label="Preinstall issues — fix before it touches the fabric" items={review.preinstall_issues} tone="text-red-400" />
          <ListBlock icon={Wrench} label="How to use / integrate" items={review.how_tos} tone="text-cyan-400" />
          <ListBlock icon={ListChecks} label="Next bricks" items={review.next_bricks} tone="text-amber-400" />
          <button
            onClick={() => onDelete(review)}
            className="flex items-center gap-1.5 text-xs font-mono text-zinc-600 hover:text-red-400 transition-colors"
          >
            <Trash2 className="h-3.5 w-3.5" /> Remove review
          </button>
        </div>
      )}
    </div>
  );
}
```

---

## File: `src/components/review/reviewGrader.js`

```text
import { base44 } from "@/api/base44Client";

const GRADE_ENUM = ["GREEN", "YELLOW", "RED", "PURPLE", "ORANGE"];

const SCHEMA = {
  type: "object",
  properties: {
    overall_grade: { type: "string", enum: GRADE_ENUM },
    code_grade: { type: "string", enum: GRADE_ENUM },
    structure_grade: { type: "string", enum: GRADE_ENUM },
    security_grade: { type: "string", enum: GRADE_ENUM },
    install_grade: { type: "string", enum: GRADE_ENUM },
    summary: { type: "string" },
    review: { type: "string" },
    how_tos: { type: "array", items: { type: "string" } },
    preinstall_issues: { type: "array", items: { type: "string" } },
    next_bricks: { type: "array", items: { type: "string" } },
  },
  required: ["overall_grade", "code_grade", "structure_grade", "security_grade", "install_grade", "summary", "review"],
};

const MAX_CHARS = 60000;

export async function gradeFile(file) {
  const raw = await file.text();
  const content = raw.slice(0, MAX_CHARS);

  const result = await base44.integrations.Core.InvokeLLM({
    prompt: `You are the reviewing organ of THE FORGE — a modular, security-first local AI fabric. Its laws: deaf-by-default isolation, one door (a signing Gate) for every privileged action, nothing bare (raw models must be wrapped/sealed), bonded-not-fused, nothing thrown away.

Review the following file thoroughly. Grade each dimension with EXACTLY one of: GREEN (solid, tested-quality), YELLOW (works but needs a look), RED (weak, broken, or missing essentials), PURPLE (revolutionary idea, seed-stage), ORANGE (needs custom work to fit).

Dimensions:
- code_grade: correctness, error handling, clarity
- structure_grade: modularity, LEGO snap-on/off separation, interfaces
- security_grade: fit with the Forge laws (one door, no bare access, replay/injection safety)
- install_grade: PREINSTALL READINESS — dependencies, environment assumptions, anything that would break a fresh install on Pop!_OS Linux
- overall_grade: your holistic verdict

Also produce:
- summary: 2-3 sentences — a quick once-over so an operator instantly understands what this file is and does
- review: an honest, specific written review (strengths, weak spots, what part of the fabric it serves)
- how_tos: short practical "how to use / how to integrate" steps
- preinstall_issues: concrete issues to fix BEFORE installing (missing deps, hardcoded paths, version pins, permissions) — empty array if none
- next_bricks: the upgrade steps, in priority order

FILE NAME: ${file.name}
FILE CONTENT:
\`\`\`
${content}
\`\`\``,
    response_json_schema: SCHEMA,
  });

  return base44.entities.FileReview.create({
    file_name: file.name,
    overall_grade: result.overall_grade,
    code_grade: result.code_grade,
    structure_grade: result.structure_grade,
    security_grade: result.security_grade,
    install_grade: result.install_grade,
    summary: result.summary,
    review: result.review,
    how_tos: result.how_tos || [],
    preinstall_issues: result.preinstall_issues || [],
    next_bricks: result.next_bricks || [],
  });
}
```

---

## File: `src/components/review/DropZone.jsx`

```text
import React, { useRef, useState } from "react";
import { UploadCloud } from "lucide-react";

export default function DropZone({ onFiles, busy }) {
  const inputRef = useRef(null);
  const [over, setOver] = useState(false);

  const handle = (files) => {
    if (!busy && files?.length) onFiles([...files]);
  };

  return (
    <div
      onClick={() => !busy && inputRef.current?.click()}
      onDragOver={(e) => { e.preventDefault(); setOver(true); }}
      onDragLeave={() => setOver(false)}
      onDrop={(e) => { e.preventDefault(); setOver(false); handle(e.dataTransfer.files); }}
      className={`cursor-pointer rounded-2xl border-2 border-dashed p-10 text-center transition-all ${
        over
          ? "border-cyan-400 bg-cyan-500/10 shadow-[0_0_30px_-8px_rgba(34,211,238,0.5)]"
          : "border-zinc-700 bg-zinc-900/50 hover:border-zinc-500"
      } ${busy ? "opacity-60 cursor-wait" : ""}`}
    >
      <input
        ref={inputRef}
        type="file"
        multiple
        className="hidden"
        onChange={(e) => { handle(e.target.files); e.target.value = ""; }}
      />
      <UploadCloud className={`mx-auto h-10 w-10 mb-3 ${over ? "text-cyan-400" : "text-zinc-500"}`} />
      <p className="font-mono text-sm text-zinc-300">
        {busy ? "Reviewing… hold the door" : "Drop files here — or click to pick"}
      </p>
      <p className="text-xs text-zinc-600 mt-1 font-mono">
        code · configs · docs — each file gets a full once-over before it touches the fabric
      </p>
    </div>
  );
}
```

---

## File: `src/components/bridge/BridgeSettings.jsx`

```text
import React, { useState } from "react";
import { getBridgeConfig, saveBridgeConfig } from "@/lib/forgeBridge";
import { Plug } from "lucide-react";

export default function BridgeSettings({ onSaved }) {
  const [cfg, setCfg] = useState(getBridgeConfig());

  const save = () => {
    saveBridgeConfig(cfg);
    onSaved?.();
  };

  return (
    <div className="rounded-xl border border-zinc-800 bg-zinc-900/60 p-4 space-y-3">
      <div className="flex items-center gap-2 text-xs font-mono uppercase tracking-widest text-zinc-400">
        <Plug className="h-3.5 w-3.5 text-cyan-400" /> Bridge connection · stored only in this browser
      </div>
      <div className="grid grid-cols-1 md:grid-cols-2 gap-3">
        <input
          value={cfg.url}
          onChange={(e) => setCfg({ ...cfg, url: e.target.value })}
          placeholder="Forge bridge URL (e.g. https://forge.yourtunnel.com)"
          className="w-full rounded-lg bg-zinc-950 border border-zinc-800 px-3 py-2 text-sm font-mono text-zinc-200 placeholder:text-zinc-600 focus:border-cyan-500/60 outline-none"
        />
        <input
          value={cfg.token}
          onChange={(e) => setCfg({ ...cfg, token: e.target.value })}
          type="password"
          placeholder="Access token (optional)"
          className="w-full rounded-lg bg-zinc-950 border border-zinc-800 px-3 py-2 text-sm font-mono text-zinc-200 placeholder:text-zinc-600 focus:border-cyan-500/60 outline-none"
        />
        <input
          value={cfg.cfId || ""}
          onChange={(e) => setCfg({ ...cfg, cfId: e.target.value })}
          placeholder="CF Access Client ID (service token)"
          className="w-full rounded-lg bg-zinc-950 border border-zinc-800 px-3 py-2 text-sm font-mono text-zinc-200 placeholder:text-zinc-600 focus:border-cyan-500/60 outline-none"
        />
        <input
          value={cfg.cfSecret || ""}
          onChange={(e) => setCfg({ ...cfg, cfSecret: e.target.value })}
          type="password"
          placeholder="CF Access Client Secret"
          className="w-full rounded-lg bg-zinc-950 border border-zinc-800 px-3 py-2 text-sm font-mono text-zinc-200 placeholder:text-zinc-600 focus:border-cyan-500/60 outline-none"
        />
      </div>
      <button
        onClick={save}
        className="rounded-full border border-cyan-500/40 bg-cyan-500/10 px-4 py-1.5 text-xs font-mono uppercase tracking-wider text-cyan-400 hover:bg-cyan-500/20 transition-colors"
      >
        Save & connect
      </button>
    </div>
  );
}
```

---

## File: `src/components/bridge/TaskRow.jsx`

```text
import React from "react";
import { base44 } from "@/api/base44Client";
import { Trash2 } from "lucide-react";

export default function TaskRow({ task, onChanged }) {
  const toggle = async () => {
    await base44.entities.ForgeTask.update(task.id, { status: task.status === "done" ? "open" : "done" });
    onChanged();
  };
  const remove = async () => {
    await base44.entities.ForgeTask.delete(task.id);
    onChanged();
  };

  return (
    <div className={`flex items-start gap-3 rounded-lg border p-3 ${task.status === "done" ? "border-zinc-800/60 bg-zinc-900/30 opacity-60" : "border-zinc-800 bg-zinc-900/60"}`}>
      <input type="checkbox" checked={task.status === "done"} onChange={toggle} className="mt-1 accent-amber-400" />
      <div className="flex-1 min-w-0">
        <p className={`text-sm font-mono text-zinc-200 ${task.status === "done" ? "line-through" : ""}`}>{task.title}</p>
        {task.detail && <p className="text-xs font-mono text-zinc-500 mt-0.5">{task.detail}</p>}
        {task.source && <p className="text-[10px] font-mono text-zinc-600 mt-1 uppercase tracking-wider">{task.source}</p>}
      </div>
      <button onClick={remove} className="text-zinc-600 hover:text-red-400 transition-colors" aria-label="Delete task">
        <Trash2 className="h-3.5 w-3.5" />
      </button>
    </div>
  );
}
```

---

## File: `src/components/bridge/ConcoctPanel.jsx`

```text
import React, { useState } from "react";
import { bridgeFetch } from "@/lib/forgeBridge";
import { FlaskConical, Gavel } from "lucide-react";

const EXAMPLE = `{
  "id": "draft-001",
  "kind": "shape",
  "spec": {}
}`;

export default function ConcoctPanel() {
  const [shapeText, setShapeText] = useState(EXAMPLE);
  const [busy, setBusy] = useState(false);
  const [result, setResult] = useState(null);

  const preview = async () => {
    let shape;
    try {
      shape = JSON.parse(shapeText);
    } catch {
      setResult({ error: "Draft isn't valid JSON — fix it before sending." });
      return;
    }
    setBusy(true);
    setResult(null);
    try {
      const res = await bridgeFetch("/concoct/preview", { method: "POST", body: JSON.stringify({ shape }) });
      setResult(res);
    } catch (error) {
      setResult({ error: error.message });
    }
    setBusy(false);
  };

  return (
    <div className="space-y-4 max-w-2xl">
      <p className="text-xs font-mono text-zinc-500">
        Drop a drafted shape into the Concoctinator arena — observe-mode only. It gets fitted and judged, never promoted.
      </p>
      <textarea
        value={shapeText}
        onChange={(e) => setShapeText(e.target.value)}
        rows={8}
        spellCheck={false}
        className="w-full rounded-lg bg-zinc-950 border border-zinc-800 px-3 py-2 text-sm font-mono text-zinc-200 focus:border-violet-500/60 outline-none"
      />
      <button
        onClick={preview}
        disabled={busy}
        className="inline-flex items-center gap-2 rounded-full border border-violet-500/40 bg-violet-500/10 px-5 py-2 text-sm font-mono uppercase tracking-wider text-violet-400 hover:bg-violet-500/20 transition-colors disabled:opacity-40"
      >
        <FlaskConical className="h-4 w-4" /> {busy ? "Judging…" : "Preview draft"}
      </button>
      {result && (
        result.error ? (
          <div className="rounded-xl border border-amber-500/30 bg-amber-500/5 p-4 text-xs font-mono text-amber-300 break-all">
            {result.error}
          </div>
        ) : (
          <div className="rounded-xl border border-violet-500/40 bg-violet-500/5 p-4">
            <div className="flex items-center gap-2 mb-2 text-sm font-mono uppercase tracking-wider text-violet-400">
              <Gavel className="h-4 w-4" /> Judgment · promoted: {String(result.promoted)}
            </div>
            <pre className="text-xs font-mono text-zinc-400 whitespace-pre-wrap break-all">{JSON.stringify(result.judgment, null, 2)}</pre>
          </div>
        )
      )}
    </div>
  );
}
```

---

## File: `src/components/bridge/HealthPanel.jsx`

```text
import React, { useEffect, useState } from "react";
import { bridgeFetch } from "@/lib/forgeBridge";
import PanelShell from "./PanelShell";
import { HeartPulse } from "lucide-react";

export default function HealthPanel() {
  const [state, setState] = useState({ loading: true });

  const load = async () => {
    try {
      const [health, sections] = await Promise.all([bridgeFetch("/health"), bridgeFetch("/sections")]);
      setState({ health, sections });
    } catch (error) {
      setState({ error });
    }
  };

  useEffect(() => {
    load();
    const t = setInterval(load, 10000);
    return () => clearInterval(t);
  }, []);

  const { health, sections, loading, error } = state;
  const secList = Array.isArray(sections) ? sections : sections?.sections || [];

  return (
    <PanelShell loading={loading} error={error}>
      {health && (
        <div className="space-y-4">
          <div className="flex flex-wrap gap-3">
            <Stat label="Booted" value={health.booted ? "YES" : "NO"} good={health.booted} />
            <Stat label="Contract" value={health.contract_version || "?"} good={Boolean(health.contract_version)} />
            <Stat label="Uptime" value={`${Math.floor((health.uptime_s || 0) / 60)}m`} good />
            <Stat label="Organs" value={(health.organs || []).length} good />
          </div>
          <div className="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-3">
            {secList.map((s, i) => (
              <div key={i} className="rounded-lg border border-zinc-800 bg-zinc-900/60 p-3">
                <div className="flex items-center gap-2 mb-1">
                  <HeartPulse className="h-3.5 w-3.5 text-emerald-400" />
                  <span className="text-sm font-mono text-zinc-200">{s.id || s.name || String(s)}</span>
                </div>
                {s.status && <p className="text-xs font-mono text-zinc-500">{s.status}</p>}
              </div>
            ))}
          </div>
        </div>
      )}
    </PanelShell>
  );
}

function Stat({ label, value, good }) {
  return (
    <div className={`rounded-lg border px-4 py-2 ${good ? "border-emerald-500/30 bg-emerald-500/5" : "border-red-500/30 bg-red-500/5"}`}>
      <p className="text-[10px] font-mono uppercase tracking-widest text-zinc-500">{label}</p>
      <p className={`text-lg font-mono ${good ? "text-emerald-400" : "text-red-400"}`}>{value}</p>
    </div>
  );
}
```

---

## File: `src/components/bridge/MintPanel.jsx`

```text
import React, { useState } from "react";
import { bridgeFetch } from "@/lib/forgeBridge";
import { KeyRound, ShieldCheck, ShieldX } from "lucide-react";

const OPS = ["npu.eval", "hopper.spawn", "coupler.mount", "net.egress", "fabric.conform", "fabric.splice", "fabric.reclaim"];
const PRESET_CAVEATS = ["read_only", "expires_in:60"];

export default function MintPanel() {
  const [op, setOp] = useState(OPS[0]);
  const [target, setTarget] = useState("");
  const [caveats, setCaveats] = useState(["read_only", "expires_in:60"]);
  const [customCaveat, setCustomCaveat] = useState("");
  const [busy, setBusy] = useState(false);
  const [result, setResult] = useState(null);

  const toggleCaveat = (c) =>
    setCaveats((prev) => (prev.includes(c) ? prev.filter((x) => x !== c) : [...prev, c]));

  const mint = async () => {
    setBusy(true);
    setResult(null);
    const all = [...caveats, ...(customCaveat.trim() ? [customCaveat.trim()] : [])];
    try {
      const res = await bridgeFetch("/mint", { method: "POST", body: JSON.stringify({ op, target, caveats: all }) });
      setResult(res);
    } catch (error) {
      setResult({ error: error.message });
    }
    setBusy(false);
  };

  return (
    <div className="space-y-4 max-w-2xl">
      <p className="text-xs font-mono text-zinc-500">
        Requests a narrowed, gate-signed capability. The Forge decides — the App just renders the verdict.
      </p>
      <div className="grid grid-cols-1 md:grid-cols-2 gap-3">
        <select
          value={op}
          onChange={(e) => setOp(e.target.value)}
          className="rounded-lg bg-zinc-950 border border-zinc-800 px-3 py-2 text-sm font-mono text-zinc-200 focus:border-amber-500/60 outline-none"
        >
          {OPS.map((o) => <option key={o} value={o}>{o}</option>)}
        </select>
        <input
          value={target}
          onChange={(e) => setTarget(e.target.value)}
          placeholder="target — section or wrap id"
          className="rounded-lg bg-zinc-950 border border-zinc-800 px-3 py-2 text-sm font-mono text-zinc-200 placeholder:text-zinc-600 focus:border-amber-500/60 outline-none"
        />
      </div>
      <div className="flex flex-wrap items-center gap-2">
        {PRESET_CAVEATS.map((c) => (
          <button
            key={c}
            onClick={() => toggleCaveat(c)}
            className={`rounded-full px-3 py-1 text-xs font-mono border transition-colors ${
              caveats.includes(c)
                ? "border-emerald-500/50 bg-emerald-500/10 text-emerald-400"
                : "border-zinc-800 text-zinc-500 hover:border-zinc-700"
            }`}
          >
            {c}
          </button>
        ))}
        <input
          value={customCaveat}
          onChange={(e) => setCustomCaveat(e.target.value)}
          placeholder="custom caveat e.g. only_section:<id>"
          className="rounded-full bg-zinc-950 border border-zinc-800 px-3 py-1 text-xs font-mono text-zinc-300 placeholder:text-zinc-600 focus:border-emerald-500/60 outline-none w-64"
        />
      </div>
      <button
        onClick={mint}
        disabled={busy || !target.trim()}
        className="inline-flex items-center gap-2 rounded-full border border-amber-500/40 bg-amber-500/10 px-5 py-2 text-sm font-mono uppercase tracking-wider text-amber-400 hover:bg-amber-500/20 transition-colors disabled:opacity-40"
      >
        <KeyRound className="h-4 w-4" /> {busy ? "Minting…" : "Request grant"}
      </button>
      {result && <MintResult result={result} />}
    </div>
  );
}

function MintResult({ result }) {
  if (result.error)
    return (
      <div className="rounded-xl border border-amber-500/30 bg-amber-500/5 p-4 text-xs font-mono text-amber-300 break-all">
        {result.error}
      </div>
    );
  const allowed = result.allowed;
  return (
    <div className={`rounded-xl border p-4 ${allowed ? "border-emerald-500/40 bg-emerald-500/5" : "border-red-500/40 bg-red-500/5"}`}>
      <div className={`flex items-center gap-2 mb-2 text-sm font-mono uppercase tracking-wider ${allowed ? "text-emerald-400" : "text-red-400"}`}>
        {allowed ? <ShieldCheck className="h-4 w-4" /> : <ShieldX className="h-4 w-4" />}
        Gate decision: {allowed ? "ALLOWED" : "DENIED"}
      </div>
      {result.finding && (
        <pre className="text-xs font-mono text-zinc-400 whitespace-pre-wrap break-all">{JSON.stringify(result.finding, null, 2)}</pre>
      )}
    </div>
  );
}
```

---

## File: `src/components/bridge/TroubleshootPanel.jsx`

```text
import React, { useEffect, useState } from "react";
import { base44 } from "@/api/base44Client";
import { bridgeFetch, getBridgeConfig } from "@/lib/forgeBridge";
import TaskRow from "@/components/bridge/TaskRow";
import { Wrench, Loader2 } from "lucide-react";

export default function TroubleshootPanel() {
  const [tasks, setTasks] = useState(null);
  const [diagnosing, setDiagnosing] = useState(false);

  const load = async () => setTasks(await base44.entities.ForgeTask.list("-created_date", 100));
  useEffect(() => { load(); }, []);

  const diagnose = async () => {
    setDiagnosing(true);
    let health = null, sections = null, bridgeError = null;
    try {
      [health, sections] = await Promise.all([bridgeFetch("/health"), bridgeFetch("/sections")]);
    } catch (e) {
      bridgeError = e.message;
    }
    const { url } = getBridgeConfig();
    const res = await base44.integrations.Core.InvokeLLM({
      prompt: `You are a troubleshooting assistant for "The Forge" — a local AI kernel on a Pop!_OS PC, reached through a Cloudflare Tunnel bridge at a private URL. The web app is a read-only window into it.

Current probe results:
- Bridge URL configured: ${url ? "yes" : "no"}
- Bridge reachable: ${bridgeError ? `NO — error: ${bridgeError}` : "yes"}
- /health: ${JSON.stringify(health)}
- /sections: ${JSON.stringify(sections)}

Generate a short, concrete checklist of troubleshooting/next-step tasks for the operator (Eugene). If the bridge is unreachable, focus on: is the PC on, is the bridge process running on 127.0.0.1:8787, is cloudflared tunnel up (docs/TRANSPORT.md), are the CF Access service token headers correct in the app settings. If healthy, suggest verification tasks instead (check feed heartbeat, run the test suite, mint a read-only capability, check the ledger verifies). 3-6 tasks max, each with a one-line title and a short actionable detail.`,
      response_json_schema: {
        type: "object",
        properties: {
          tasks: {
            type: "array",
            items: {
              type: "object",
              properties: {
                title: { type: "string" },
                detail: { type: "string" },
                source: { type: "string" }
              }
            }
          }
        }
      }
    });
    const newTasks = (res.tasks || []).map((t) => ({ ...t, status: "open" }));
    if (newTasks.length) await base44.entities.ForgeTask.bulkCreate(newTasks);
    await load();
    setDiagnosing(false);
  };

  return (
    <div>
      <div className="flex items-center justify-between mb-4">
        <div className="flex items-center gap-2 text-xs font-mono uppercase tracking-widest text-zinc-400">
          <Wrench className="h-3.5 w-3.5 text-amber-400" /> Troubleshoot · tasks are saved for next time
        </div>
        <button
          onClick={diagnose}
          disabled={diagnosing}
          className="inline-flex items-center gap-2 rounded-full border border-amber-500/40 bg-amber-500/10 px-4 py-1.5 text-xs font-mono uppercase tracking-wider text-amber-400 hover:bg-amber-500/20 transition-colors disabled:opacity-50"
        >
          {diagnosing && <Loader2 className="h-3.5 w-3.5 animate-spin" />}
          {diagnosing ? "Probing bridge…" : "Diagnose now"}
        </button>
      </div>
      {tasks === null ? (
        <p className="text-zinc-600 text-center py-16 font-mono text-sm">Loading tasks…</p>
      ) : tasks.length === 0 ? (
        <p className="text-zinc-600 text-center py-16 font-mono text-sm">No tasks yet — hit “Diagnose now” to probe the bridge and generate a checklist.</p>
      ) : (
        <div className="space-y-2 max-h-[60vh] overflow-y-auto pr-1">
          {tasks.map((t) => <TaskRow key={t.id} task={t} onChanged={load} />)}
        </div>
      )}
    </div>
  );
}
```

---

## File: `src/components/bridge/WrapsPanel.jsx`

```text
import React, { useEffect, useState } from "react";
import { bridgeFetch } from "@/lib/forgeBridge";
import PanelShell from "./PanelShell";
import { Package, Lock, Recycle } from "lucide-react";

export default function WrapsPanel() {
  const [state, setState] = useState({ loading: true });

  useEffect(() => {
    bridgeFetch("/wraps")
      .then((data) => setState({ wraps: Array.isArray(data) ? data : data.wraps || [] }))
      .catch((error) => setState({ error }));
  }, []);

  const { wraps, loading, error } = state;

  return (
    <PanelShell loading={loading} error={error} empty={wraps && wraps.length === 0} emptyText="WrapStore is empty.">
      <div className="grid grid-cols-1 sm:grid-cols-2 gap-3">
        {(wraps || []).map((w) => (
          <div key={w.id} className="rounded-lg border border-zinc-800 bg-zinc-900/60 p-4">
            <div className="flex items-center gap-2 mb-2">
              <Package className="h-4 w-4 text-violet-400" />
              <span className="text-sm font-mono text-zinc-200">{w.id}</span>
            </div>
            <p className="text-xs font-mono text-zinc-500 break-all mb-2">{w.fingerprint}</p>
            <div className="flex gap-2">
              {w.sealed && (
                <span className="inline-flex items-center gap-1 rounded-full border border-emerald-500/30 bg-emerald-500/10 px-2 py-0.5 text-[10px] font-mono text-emerald-400">
                  <Lock className="h-3 w-3" /> SEALED
                </span>
              )}
              {w.reclaimed && (
                <span className="inline-flex items-center gap-1 rounded-full border border-amber-500/30 bg-amber-500/10 px-2 py-0.5 text-[10px] font-mono text-amber-400">
                  <Recycle className="h-3 w-3" /> RECLAIMED
                </span>
              )}
            </div>
          </div>
        ))}
      </div>
    </PanelShell>
  );
}
```

---

## File: `src/components/bridge/LedgerPanel.jsx`

```text
import React, { useEffect, useState } from "react";
import { bridgeFetch } from "@/lib/forgeBridge";
import PanelShell from "./PanelShell";
import { Link2 } from "lucide-react";

export default function LedgerPanel() {
  const [state, setState] = useState({ loading: true });

  useEffect(() => {
    bridgeFetch("/ledger?since=0")
      .then((data) => setState({ entries: Array.isArray(data) ? data : data.entries || [], verified: data.verified }))
      .catch((error) => setState({ error }));
  }, []);

  const { entries, verified, loading, error } = state;

  return (
    <PanelShell loading={loading} error={error} empty={entries && entries.length === 0} emptyText="Ledger is empty.">
      <div>
      {verified !== undefined && verified !== null && (
        <div className={`inline-flex items-center gap-2 mb-4 rounded-full border px-3 py-1 text-xs font-mono uppercase tracking-wider ${verified ? "border-emerald-500/40 bg-emerald-500/10 text-emerald-400" : "border-red-500/40 bg-red-500/10 text-red-400"}`}>
          Hash chain: {verified ? "VERIFIED · tamper-free" : "BROKEN · tamper detected"}
        </div>
      )}
      <div className="space-y-2 max-h-[60vh] overflow-y-auto pr-1">
        {(entries || []).map((e, i) => (
          <div key={i} className="rounded-lg border border-zinc-800 bg-zinc-900/60 p-3 flex items-start gap-3">
            <Link2 className="h-3.5 w-3.5 text-cyan-400 mt-1 shrink-0" />
            <pre className="text-xs font-mono text-zinc-300 whitespace-pre-wrap break-all flex-1">
              {typeof e === "string" ? e : JSON.stringify(e, null, 2)}
            </pre>
          </div>
        ))}
      </div>
      </div>
    </PanelShell>
  );
}
```

---

## File: `src/components/bridge/PanelShell.jsx`

```text
import React from "react";
import { AlertTriangle } from "lucide-react";

export default function PanelShell({ loading, error, empty, emptyText, children }) {
  if (loading)
    return (
      <div className="flex justify-center py-16">
        <div className="w-6 h-6 border-2 border-zinc-800 border-t-cyan-400 rounded-full animate-spin" />
      </div>
    );
  if (error)
    return (
      <div className="flex items-start gap-3 rounded-xl border border-amber-500/30 bg-amber-500/5 p-4 text-sm text-amber-300">
        <AlertTriangle className="h-4 w-4 mt-0.5 shrink-0" />
        <div>
          <p className="font-mono text-xs uppercase tracking-wider mb-1">Forge unreachable</p>
          <p className="text-zinc-400 text-xs font-mono break-all">{String(error.message || error)}</p>
        </div>
      </div>
    );
  if (empty)
    return <p className="text-zinc-600 text-center py-16 font-mono text-sm">{emptyText || "Nothing here yet."}</p>;
  return children;
}
```

---

## File: `src/components/bridge/ConnectionGuide.jsx`

```text
import React, { useState } from "react";
import { bridgeFetch } from "@/lib/forgeBridge";
import { Copy, Check, Zap, Loader2 } from "lucide-react";

const STEPS = [
  {
    title: "Start the Forge bridge on your PC",
    detail: "On the Pop!_OS machine, boot the kernel + bridge so it listens locally (see docs/TRANSPORT.md in the repo).",
    cmd: "python -m forge_ng.bridge",
  },
  {
    title: "Open the Cloudflare tunnel",
    detail: "This gives your local bridge a public HTTPS address protected by Cloudflare Access.",
    cmd: "cloudflared tunnel run forge",
  },
  {
    title: "Fill in the connection form above",
    detail: "Paste the tunnel URL plus your CF Access Client ID and Secret, then hit Save & connect.",
  },
];

export default function ConnectionGuide() {
  const [copied, setCopied] = useState(null);
  const [test, setTest] = useState({ state: "idle" });

  const copy = (cmd, i) => {
    navigator.clipboard.writeText(cmd);
    setCopied(i);
    setTimeout(() => setCopied(null), 1500);
  };

  const runTest = async () => {
    setTest({ state: "running" });
    try {
      const health = await bridgeFetch("/health");
      setTest({ state: "ok", msg: `Bridge is up · booted: ${health.booted ? "yes" : "no"} · contract ${health.contract_version || "?"}` });
    } catch (e) {
      setTest({ state: "fail", msg: e.message });
    }
  };

  return (
    <div className="rounded-xl border border-zinc-800 bg-zinc-900/40 p-4 space-y-4">
      <p className="text-xs font-mono uppercase tracking-widest text-zinc-500">Getting connected · 3 steps</p>
      <ol className="space-y-3">
        {STEPS.map((s, i) => (
          <li key={i} className="flex gap-3">
            <span className="flex h-6 w-6 shrink-0 items-center justify-center rounded-full border border-cyan-500/40 text-cyan-400 text-xs font-mono">{i + 1}</span>
            <div className="min-w-0 flex-1">
              <p className="text-sm text-zinc-200">{s.title}</p>
              <p className="text-xs text-zinc-500 mt-0.5">{s.detail}</p>
              {s.cmd && (
                <button
                  onClick={() => copy(s.cmd, i)}
                  className="mt-1.5 inline-flex items-center gap-2 rounded-md bg-zinc-950 border border-zinc-800 px-3 py-1.5 text-xs font-mono text-emerald-400 hover:border-zinc-600 transition-colors"
                >
                  {s.cmd}
                  {copied === i ? <Check className="h-3 w-3" /> : <Copy className="h-3 w-3 text-zinc-600" />}
                </button>
              )}
            </div>
          </li>
        ))}
      </ol>
      <div className="flex items-center gap-3 pt-1 border-t border-zinc-800/60">
        <button
          onClick={runTest}
          disabled={test.state === "running"}
          className="mt-3 inline-flex items-center gap-2 rounded-full border border-emerald-500/40 bg-emerald-500/10 px-4 py-1.5 text-xs font-mono uppercase tracking-wider text-emerald-400 hover:bg-emerald-500/20 transition-colors disabled:opacity-50"
        >
          {test.state === "running" ? <Loader2 className="h-3.5 w-3.5 animate-spin" /> : <Zap className="h-3.5 w-3.5" />}
          Test connection
        </button>
        {test.msg && (
          <p className={`mt-3 text-xs font-mono ${test.state === "ok" ? "text-emerald-400" : "text-red-400"}`}>{test.msg}</p>
        )}
      </div>
    </div>
  );
}
```

---

## File: `src/components/bridge/LiveFeed.jsx`

```text
import React, { useEffect, useState } from "react";
import { openFeed } from "@/lib/forgeBridge";
import { Radio } from "lucide-react";

export default function LiveFeed() {
  const [events, setEvents] = useState([]);
  const [status, setStatus] = useState("connecting");
  const [lastBeat, setLastBeat] = useState(null);

  useEffect(() => {
    const abort = openFeed((raw) => {
      let data;
      try { data = JSON.parse(raw); } catch { data = { raw }; }
      if (data.kind === "heartbeat") {
        setLastBeat(Date.now());
        return;
      }
      setEvents((prev) => [{ ts: Date.now(), data }, ...prev].slice(0, 200));
    }, setStatus);
    return abort;
  }, []);

  const dot = { live: "bg-emerald-400", connecting: "bg-yellow-400", disconnected: "bg-red-500", unconfigured: "bg-zinc-600" }[status];

  return (
    <div>
      <div className="flex items-center gap-2 mb-4 text-xs font-mono uppercase tracking-widest text-zinc-400">
        <span className={`h-2 w-2 rounded-full ${dot} ${status === "live" ? "animate-pulse" : ""}`} />
        <Radio className="h-3.5 w-3.5" /> Overseer tap · {status}
        {lastBeat && <span className="text-zinc-600 normal-case">· heartbeat {new Date(lastBeat).toLocaleTimeString()}</span>}
      </div>
      {events.length === 0 ? (
        <p className="text-zinc-600 text-center py-16 font-mono text-sm">
          {status === "unconfigured" ? "Set your bridge URL in settings to open the feed." : "Waiting for findings + heartbeat ticks…"}
        </p>
      ) : (
        <div className="space-y-2 max-h-[60vh] overflow-y-auto pr-1">
          {events.map((e, i) => (
            <div key={i} className="rounded-lg border border-zinc-800 bg-zinc-900/60 p-3">
              <p className="text-[10px] font-mono text-zinc-600 mb-1">{new Date(e.ts).toLocaleTimeString()}</p>
              <pre className="text-xs font-mono text-zinc-300 whitespace-pre-wrap break-all">{JSON.stringify(e.data, null, 2)}</pre>
            </div>
          ))}
        </div>
      )}
    </div>
  );
}
```

---

## File: `src/components/ui/avatar.jsx`

```text
"use client"

import * as React from "react"
import * as AvatarPrimitive from "@radix-ui/react-avatar"

import { cn } from "@/lib/utils"

const Avatar = React.forwardRef(({ className, ...props }, ref) => (
  <AvatarPrimitive.Root
    ref={ref}
    className={cn("relative flex h-10 w-10 shrink-0 overflow-hidden rounded-full", className)}
    {...props} />
))
Avatar.displayName = AvatarPrimitive.Root.displayName

const AvatarImage = React.forwardRef(({ className, ...props }, ref) => (
  <AvatarPrimitive.Image
    ref={ref}
    className={cn("aspect-square h-full w-full", className)}
    {...props} />
))
AvatarImage.displayName = AvatarPrimitive.Image.displayName

const AvatarFallback = React.forwardRef(({ className, ...props }, ref) => (
  <AvatarPrimitive.Fallback
    ref={ref}
    className={cn(
      "flex h-full w-full items-center justify-center rounded-full bg-muted",
      className
    )}
    {...props} />
))
AvatarFallback.displayName = AvatarPrimitive.Fallback.displayName

export { Avatar, AvatarImage, AvatarFallback }

```

---

## File: `src/components/ui/breadcrumb.jsx`

```text
import * as React from "react"
import { Slot } from "@radix-ui/react-slot"
import { ChevronRight, MoreHorizontal } from "lucide-react"

import { cn } from "@/lib/utils"

const Breadcrumb = React.forwardRef(
  ({ ...props }, ref) => <nav ref={ref} aria-label="breadcrumb" {...props} />
)
Breadcrumb.displayName = "Breadcrumb"

const BreadcrumbList = React.forwardRef(({ className, ...props }, ref) => (
  <ol
    ref={ref}
    className={cn(
      "flex flex-wrap items-center gap-1.5 break-words text-sm text-muted-foreground sm:gap-2.5",
      className
    )}
    {...props} />
))
BreadcrumbList.displayName = "BreadcrumbList"

const BreadcrumbItem = React.forwardRef(({ className, ...props }, ref) => (
  <li
    ref={ref}
    className={cn("inline-flex items-center gap-1.5", className)}
    {...props} />
))
BreadcrumbItem.displayName = "BreadcrumbItem"

const BreadcrumbLink = React.forwardRef(({ asChild, className, ...props }, ref) => {
  const Comp = asChild ? Slot : "a"

  return (
    (<Comp
      ref={ref}
      className={cn("transition-colors hover:text-foreground", className)}
      {...props} />)
  );
})
BreadcrumbLink.displayName = "BreadcrumbLink"

const BreadcrumbPage = React.forwardRef(({ className, ...props }, ref) => (
  <span
    ref={ref}
    role="link"
    aria-disabled="true"
    aria-current="page"
    className={cn("font-normal text-foreground", className)}
    {...props} />
))
BreadcrumbPage.displayName = "BreadcrumbPage"

const BreadcrumbSeparator = ({
  children,
  className,
  ...props
}) => (
  <li
    role="presentation"
    aria-hidden="true"
    className={cn("[&>svg]:w-3.5 [&>svg]:h-3.5", className)}
    {...props}>
    {children ?? <ChevronRight />}
  </li>
)
BreadcrumbSeparator.displayName = "BreadcrumbSeparator"

const BreadcrumbEllipsis = ({
  className,
  ...props
}) => (
  <span
    role="presentation"
    aria-hidden="true"
    className={cn("flex h-9 w-9 items-center justify-center", className)}
    {...props}>
    <MoreHorizontal className="h-4 w-4" />
    <span className="sr-only">More</span>
  </span>
)
BreadcrumbEllipsis.displayName = "BreadcrumbElipssis"

export {
  Breadcrumb,
  BreadcrumbList,
  BreadcrumbItem,
  BreadcrumbLink,
  BreadcrumbPage,
  BreadcrumbSeparator,
  BreadcrumbEllipsis,
}

```

---

## File: `src/components/ui/separator.jsx`

```text
import * as React from "react"
import * as SeparatorPrimitive from "@radix-ui/react-separator"

import { cn } from "@/lib/utils"

const Separator = React.forwardRef((
  { className, orientation = "horizontal", decorative = true, ...props },
  ref
) => (
  <SeparatorPrimitive.Root
    ref={ref}
    decorative={decorative}
    orientation={orientation}
    className={cn(
      "shrink-0 bg-border",
      orientation === "horizontal" ? "h-[1px] w-full" : "h-full w-[1px]",
      className
    )}
    {...props} />
))
Separator.displayName = SeparatorPrimitive.Root.displayName

export { Separator }

```

---

## File: `src/components/ui/image.jsx`

```text
import * as React from "react"
import { useSize } from "@/hooks/use-size"
import { cn } from "@/lib/utils"

const FALLBACK_IMAGE_URL =
  "https://static.wixstatic.com/media/12d367_4f26ccd17f8f4e3a8958306ea08c2332~mv2.png"

// Wix Media Platform hosts whose images support /v1/ transform URLs
// (resize, focal-point crop, and format conversion via the OUTPUT FILENAME
// EXTENSION — a .webp output re-encodes JPG/PNG uploads to WebP on the fly).
const WIX_MEDIA_HOSTS = ["media.base44.com", "static.wixstatic.com"]
// First-paint width before the container is measured.
const DEFAULT_TRANSFORM_WIDTH = 1024
const DEVICE_PIXEL_RATIOS = [1, 2, 3]
// Not a documented CDN limit — verified live that w_/h_ up to 10000 succeed
// and requests start failing somewhere between 10000 and 15000. This is a
// defensive ceiling with generous headroom (a 3x DPR request needs a
// ~2000px container to reach it), not a real constraint we expect to hit.
const MAX_DIMENSION = 6000

/**
 * Detects a Wix Media URL and strips any existing /v1/ transform so it can be
 * rebuilt. Returns null for other hosts and for SVGs (vectors — a raster
 * transform only downgrades them).
 */
function parseWixMediaUrl(src) {
  try {
    const url = new URL(src)
    if (!WIX_MEDIA_HOSTS.includes(url.hostname)) return null
    const v1 = url.pathname.indexOf("/v1/")
    const basePath = v1 === -1 ? url.pathname : url.pathname.slice(0, v1)
    const filename = basePath.split("/").pop()
    if (!filename || /\.svg$/i.test(filename)) return null
    return { baseUrl: `${url.origin}${basePath}`, filename }
  } catch {
    return null
  }
}

const clampDim = (n) => Math.min(Math.max(Math.round(n), 1), MAX_DIMENSION)
const clamp01 = (n) => Math.min(1, Math.max(0, n))

/**
 * Builds a Wix Media transform URL:
 * `<base>/v1/{fill|fit}/w_,h_[,fp_x_y|al_c],q_,usm_…/<name>.webp`
 * GIFs keep their extension (WebP output could drop animation).
 */
function buildTransformUrl({ baseUrl, filename }, { width, height, crop, focalPoint, quality }) {
  const params = [`w_${clampDim(width)}`, `h_${clampDim(height || width)}`]
  if (crop) {
    params.push(
      focalPoint
        ? `fp_${clamp01(focalPoint.x).toFixed(2)}_${clamp01(focalPoint.y).toFixed(2)}`
        : "al_c"
    )
  }
  params.push(`q_${quality}`, "usm_0.66_1.00_0.01", "enc_webp", "quality_auto")
  const outputName = /\.gif$/i.test(filename)
    ? filename
    : filename.replace(/\.[a-z0-9]+$/i, "") + ".webp"
  return `${baseUrl}/v1/${crop ? "fill" : "fit"}/${params.join(",")}/${outputName}`
}

function buildSrcSet(parsed, options) {
  return DEVICE_PIXEL_RATIOS.map(
    (dpr) =>
      `${buildTransformUrl(parsed, {
        ...options,
        width: options.width * dpr,
        height: options.height ? options.height * dpr : undefined,
      })} ${dpr}x`
  ).join(", ")
}

const ImageWrapper = React.forwardRef(({ aspectRatio, className, style, children }, ref) => (
  <span
    ref={ref}
    className={cn("inline-block relative", className)}
    style={{ aspectRatio, ...style }}
  >
    {children}
  </span>
))
ImageWrapper.displayName = "ImageWrapper"

const ResponsiveImage = React.forwardRef(
  ({ parsed, fittingType, focalPoint, quality, className, style, aspectRatio, onLoad, ...props }, parentRef) => {
    const wrapperRef = React.useRef(null)
    const imgRef = React.useRef(null)
    const size = useSize(wrapperRef)
    const [loaded, setLoaded] = React.useState(false)

    React.useImperativeHandle(parentRef, () => imgRef.current)

    // Reset the blur-up when the underlying image changes.
    React.useEffect(() => {
      setLoaded(false)
    }, [parsed.baseUrl])

    const crop = fittingType !== "fit"
    // `size` is null exactly once: the pre-measurement first render, which we
    // never let reach the network (see below — useSize measures before paint).
    // A *measured* zero (content-sized wrapper with no CSS dimensions) falls
    // back to a fixed transform width so the image itself can size the box.
    const options = size && {
      width: size.width || DEFAULT_TRANSFORM_WIDTH,
      height: size.height ? size.height : undefined,
      crop,
      focalPoint: crop ? focalPoint : undefined,
      quality,
    }

    // Both layers render only once the container is measured, so the first
    // URL the browser ever fetches is already the right size — never a
    // DEFAULT_TRANSFORM_WIDTH guess that gets replaced a frame later (a
    // wasted full-size download per image). useSize measures in
    // useLayoutEffect, so nothing is lost: measurement lands before the
    // first paint.
    return (
      <ImageWrapper ref={wrapperRef} aspectRatio={aspectRatio} className={className} style={style}>
        {/* Tiny blurred placeholder (a few hundred bytes) covering the main
            image's load time. Same crop shape and focal anchor as the main
            image — fp_ is relative to the crop box, so a square or centered
            placeholder would blur-preview a different region. */}
        {options && !loaded && (
          <img
            src={buildTransformUrl(parsed, {
              ...options,
              width: 20,
              height: options.height
                ? Math.max(1, Math.round((20 * options.height) / options.width))
                : undefined,
              quality: 20,
            })}
            alt=""
            aria-hidden="true"
            className="w-full h-full inset-0 absolute"
            style={{
              objectFit: fittingType === "fit" ? "contain" : "cover",
              filter: "blur(10px)",
              transform: "scale(1.1)",
            }}
          />
        )}
        {options && (
          <img
            ref={imgRef}
            src={buildTransformUrl(parsed, options)}
            srcSet={buildSrcSet(parsed, options)}
            loading="lazy"
            className={cn(
              "w-full h-full inset-0 absolute",
              fittingType === "fit" ? "object-contain" : "object-cover"
            )}
            onLoad={(e) => {
              setLoaded(true)
              onLoad?.(e)
            }}
            {...props}
          />
        )}
      </ImageWrapper>
    )
  }
)
ResponsiveImage.displayName = "ResponsiveImage"

/**
 * Image with built-in Wix Media Platform support: URLs on media.base44.com /
 * static.wixstatic.com are served resized to the rendered container (per
 * device pixel ratio) and re-encoded to WebP; `fittingType="fill"` crops
 * server-side, optionally anchored at a focal point. Other URLs render as a
 * plain <img>. Failed loads swap to a fallback image.
 */
const Image = React.forwardRef(
  (
    {
      src,
      fittingType = "fill",
      originWidth,
      originHeight,
      focalPointX,
      focalPointY,
      quality = 90,
      ...props
    },
    ref
  ) => {
    const [imgSrc, setImgSrc] = React.useState(src)

    React.useEffect(() => {
      setImgSrc(src)
    }, [src])

    const imageProps = {
      ...props,
      onError: () => setImgSrc(FALLBACK_IMAGE_URL),
    }

    if (!src) {
      // Renders as a real <img> (not a <div>) — the visual editor's
      // click-to-edit toolbar keys its "Replace Image" action off the DOM
      // tag being `img`, so a placeholder div would be unrecoverable in the
      // editor. FALLBACK_IMAGE_URL doubles as the "no image chosen" graphic.
      return <img ref={ref} src={FALLBACK_IMAGE_URL} {...imageProps} data-empty-image />
    }

    // The fallback renders as a plain <img> so a broken upload can't cascade
    // into a second (transformed) failing request.
    const parsed = imgSrc === FALLBACK_IMAGE_URL ? null : parseWixMediaUrl(imgSrc)

    if (!parsed) {
      const isErrorUrl = imgSrc === FALLBACK_IMAGE_URL
      return (
        <img ref={ref} src={imgSrc} {...imageProps} data-error-image={isErrorUrl || undefined} />
      )
    }

    const focalPoint =
      typeof focalPointX === "number" && typeof focalPointY === "number"
        ? { x: focalPointX, y: focalPointY }
        : undefined
    // Origin dimensions are optional — when known they stabilize layout via
    // the wrapper's aspect-ratio before the image loads.
    const aspectRatio =
      originWidth && originHeight ? `${originWidth} / ${originHeight}` : undefined

    return (
      <ResponsiveImage
        ref={ref}
        parsed={parsed}
        fittingType={fittingType}
        focalPoint={focalPoint}
        quality={quality}
        aspectRatio={aspectRatio}
        {...imageProps}
      />
    )
  }
)
Image.displayName = "Image"

export { Image }

```

---

## File: `src/components/ui/sidebar.jsx`

```text
import * as React from "react"
import { Slot } from "@radix-ui/react-slot"
import { cva } from "class-variance-authority";
import { PanelLeft } from "lucide-react"

import { useIsMobile } from "@/hooks/use-mobile"
import { cn } from "@/lib/utils"
import { Button } from "@/components/ui/button"
import { Input } from "@/components/ui/input"
import { Separator } from "@/components/ui/separator"
import { Sheet, SheetContent } from "@/components/ui/sheet"
import { Skeleton } from "@/components/ui/skeleton"
import {
  Tooltip,
  TooltipContent,
  TooltipProvider,
  TooltipTrigger,
} from "@/components/ui/tooltip"

const SIDEBAR_COOKIE_NAME = "sidebar_state"
const SIDEBAR_COOKIE_MAX_AGE = 60 * 60 * 24 * 7
const SIDEBAR_WIDTH = "16rem"
const SIDEBAR_WIDTH_MOBILE = "18rem"
const SIDEBAR_WIDTH_ICON = "3rem"
const SIDEBAR_KEYBOARD_SHORTCUT = "b"

const SidebarContext = React.createContext(null)

function useSidebar() {
  const context = React.useContext(SidebarContext)
  if (!context) {
    throw new Error("useSidebar must be used within a SidebarProvider.")
  }

  return context
}

const SidebarProvider = React.forwardRef((
  {
    defaultOpen = true,
    open: openProp,
    onOpenChange: setOpenProp,
    className,
    style,
    children,
    ...props
  },
  ref
) => {
  const isMobile = useIsMobile()
  const [openMobile, setOpenMobile] = React.useState(false)

  // This is the internal state of the sidebar.
  // We use openProp and setOpenProp for control from outside the component.
  const [_open, _setOpen] = React.useState(defaultOpen)
  const open = openProp ?? _open
  const setOpen = React.useCallback((value) => {
    const openState = typeof value === "function" ? value(open) : value
    if (setOpenProp) {
      setOpenProp(openState)
    } else {
      _setOpen(openState)
    }

    // This sets the cookie to keep the sidebar state.
    document.cookie = `${SIDEBAR_COOKIE_NAME}=${openState}; path=/; max-age=${SIDEBAR_COOKIE_MAX_AGE}`
  }, [setOpenProp, open])

  // Helper to toggle the sidebar.
  const toggleSidebar = React.useCallback(() => {
    return isMobile
      ? setOpenMobile((open) => !open)
      : setOpen((open) => !open);
  }, [isMobile, setOpen, setOpenMobile])

  // Adds a keyboard shortcut to toggle the sidebar.
  React.useEffect(() => {
    const handleKeyDown = (event) => {
      if (
        event.key === SIDEBAR_KEYBOARD_SHORTCUT &&
        (event.metaKey || event.ctrlKey)
      ) {
        event.preventDefault()
        toggleSidebar()
      }
    }

    window.addEventListener("keydown", handleKeyDown)
    return () => window.removeEventListener("keydown", handleKeyDown);
  }, [toggleSidebar])

  // We add a state so that we can do data-state="expanded" or "collapsed".
  // This makes it easier to style the sidebar with Tailwind classes.
  const state = open ? "expanded" : "collapsed"

  const contextValue = React.useMemo(() => ({
    state,
    open,
    setOpen,
    isMobile,
    openMobile,
    setOpenMobile,
    toggleSidebar,
  }), [state, open, setOpen, isMobile, openMobile, setOpenMobile, toggleSidebar])

  return (
    (<SidebarContext.Provider value={contextValue}>
      <TooltipProvider delayDuration={0}>
        <div
          style={
            {
              "--sidebar-width": SIDEBAR_WIDTH,
              "--sidebar-width-icon": SIDEBAR_WIDTH_ICON,
              ...style
            }
          }
          className={cn(
            "group/sidebar-wrapper flex min-h-svh w-full has-[[data-variant=inset]]:bg-sidebar",
            className
          )}
          ref={ref}
          {...props}>
          {children}
        </div>
      </TooltipProvider>
    </SidebarContext.Provider>)
  );
})
SidebarProvider.displayName = "SidebarProvider"

const Sidebar = React.forwardRef((
  {
    side = "left",
    variant = "sidebar",
    collapsible = "offcanvas",
    className,
    children,
    ...props
  },
  ref
) => {
  const { isMobile, state, openMobile, setOpenMobile } = useSidebar()

  if (collapsible === "none") {
    return (
      (<div
        className={cn(
          "flex h-full w-[--sidebar-width] flex-col bg-sidebar text-sidebar-foreground",
          className
        )}
        ref={ref}
        {...props}>
        {children}
      </div>)
    );
  }

  if (isMobile) {
    return (
      (<Sheet open={openMobile} onOpenChange={setOpenMobile} {...props}>
        <SheetContent
          data-sidebar="sidebar"
          data-mobile="true"
          className="w-[--sidebar-width] bg-sidebar p-0 text-sidebar-foreground [&>button]:hidden"
          style={
            {
              "--sidebar-width": SIDEBAR_WIDTH_MOBILE
            }
          }
          side={side}>
          <div className="flex h-full w-full flex-col">{children}</div>
        </SheetContent>
      </Sheet>)
    );
  }

  return (
    (<div
      ref={ref}
      className="group peer hidden text-sidebar-foreground md:block"
      data-state={state}
      data-collapsible={state === "collapsed" ? collapsible : ""}
      data-variant={variant}
      data-side={side}>
      {/* This is what handles the sidebar gap on desktop */}
      <div
        className={cn(
          "relative h-svh w-[--sidebar-width] bg-transparent transition-[width] duration-200 ease-linear",
          "group-data-[collapsible=offcanvas]:w-0",
          "group-data-[side=right]:rotate-180",
          variant === "floating" || variant === "inset"
            ? "group-data-[collapsible=icon]:w-[calc(var(--sidebar-width-icon)_+_theme(spacing.4))]"
            : "group-data-[collapsible=icon]:w-[--sidebar-width-icon]"
        )} />
      <div
        className={cn(
          "fixed inset-y-0 z-10 hidden h-svh w-[--sidebar-width] transition-[left,right,width] duration-200 ease-linear md:flex",
          side === "left"
            ? "left-0 group-data-[collapsible=offcanvas]:left-[calc(var(--sidebar-width)*-1)]"
            : "right-0 group-data-[collapsible=offcanvas]:right-[calc(var(--sidebar-width)*-1)]",
          // Adjust the padding for floating and inset variants.
          variant === "floating" || variant === "inset"
            ? "p-2 group-data-[collapsible=icon]:w-[calc(var(--sidebar-width-icon)_+_theme(spacing.4)_+2px)]"
            : "group-data-[collapsible=icon]:w-[--sidebar-width-icon] group-data-[side=left]:border-r group-data-[side=right]:border-l",
          className
        )}
        {...props}>
        <div
          data-sidebar="sidebar"
          className="flex h-full w-full flex-col bg-sidebar group-data-[variant=floating]:rounded-lg group-data-[variant=floating]:border group-data-[variant=floating]:border-sidebar-border group-data-[variant=floating]:shadow">
          {children}
        </div>
      </div>
    </div>)
  );
})
Sidebar.displayName = "Sidebar"

const SidebarTrigger = React.forwardRef(({ className, onClick, asChild = false, ...props }, ref) => {
  const { toggleSidebar } = useSidebar()

  return (
    (<Button
      ref={ref}
      data-sidebar="trigger"
      variant="ghost"
      size="icon"
      className={cn("h-7 w-7", className)}
      onClick={(event) => {
        onClick?.(event)
        toggleSidebar()
      }}
      asChild={asChild}
      {...props}>
      {asChild ? (
        <PanelLeft />
      ) : (
        <>
          <PanelLeft />
          <span className="sr-only">Toggle Sidebar</span>
        </>
      )}
    </Button>)
  );
})
SidebarTrigger.displayName = "SidebarTrigger"

const SidebarRail = React.forwardRef(({ className, ...props }, ref) => {
  const { toggleSidebar } = useSidebar()

  return (
    (<button
      ref={ref}
      data-sidebar="rail"
      aria-label="Toggle Sidebar"
      tabIndex={-1}
      onClick={toggleSidebar}
      title="Toggle Sidebar"
      className={cn(
        "absolute inset-y-0 z-20 hidden w-4 -translate-x-1/2 transition-all ease-linear after:absolute after:inset-y-0 after:left-1/2 after:w-[2px] hover:after:bg-sidebar-border group-data-[side=left]:-right-4 group-data-[side=right]:left-0 sm:flex",
        "[[data-side=left]_&]:cursor-w-resize [[data-side=right]_&]:cursor-e-resize",
        "[[data-side=left][data-state=collapsed]_&]:cursor-e-resize [[data-side=right][data-state=collapsed]_&]:cursor-w-resize",
        "group-data-[collapsible=offcanvas]:translate-x-0 group-data-[collapsible=offcanvas]:after:left-full group-data-[collapsible=offcanvas]:hover:bg-sidebar",
        "[[data-side=left][data-collapsible=offcanvas]_&]:-right-2",
        "[[data-side=right][data-collapsible=offcanvas]_&]:-left-2",
        className
      )}
      {...props} />)
  );
})
SidebarRail.displayName = "SidebarRail"

const SidebarInset = React.forwardRef(({ className, ...props }, ref) => {
  return (
    (<main
      ref={ref}
      className={cn(
        "relative flex min-h-svh flex-1 flex-col bg-background",
        "peer-data-[variant=inset]:min-h-[calc(100svh-theme(spacing.4))] md:peer-data-[variant=inset]:m-2 md:peer-data-[state=collapsed]:peer-data-[variant=inset]:ml-2 md:peer-data-[variant=inset]:ml-0 md:peer-data-[variant=inset]:rounded-xl md:peer-data-[variant=inset]:shadow",
        className
      )}
      {...props} />)
  );
})
SidebarInset.displayName = "SidebarInset"

const SidebarInput = React.forwardRef(({ className, ...props }, ref) => {
  return (
    (<Input
      ref={ref}
      data-sidebar="input"
      className={cn(
        "h-8 w-full bg-background shadow-none focus-visible:ring-2 focus-visible:ring-sidebar-ring",
        className
      )}
      {...props} />)
  );
})
SidebarInput.displayName = "SidebarInput"

const SidebarHeader = React.forwardRef(({ className, ...props }, ref) => {
  return (
    (<div
      ref={ref}
      data-sidebar="header"
      className={cn("flex flex-col gap-2 p-2", className)}
      {...props} />)
  );
})
SidebarHeader.displayName = "SidebarHeader"

const SidebarFooter = React.forwardRef(({ className, ...props }, ref) => {
  return (
    (<div
      ref={ref}
      data-sidebar="footer"
      className={cn("flex flex-col gap-2 p-2", className)}
      {...props} />)
  );
})
SidebarFooter.displayName = "SidebarFooter"

const SidebarSeparator = React.forwardRef(({ className, ...props }, ref) => {
  return (
    (<Separator
      ref={ref}
      data-sidebar="separator"
      className={cn("mx-2 w-auto bg-sidebar-border", className)}
      {...props} />)
  );
})
SidebarSeparator.displayName = "SidebarSeparator"

const SidebarContent = React.forwardRef(({ className, ...props }, ref) => {
  return (
    (<div
      ref={ref}
      data-sidebar="content"
      className={cn(
        "flex min-h-0 flex-1 flex-col gap-2 overflow-auto group-data-[collapsible=icon]:overflow-hidden",
        className
      )}
      {...props} />)
  );
})
SidebarContent.displayName = "SidebarContent"

const SidebarGroup = React.forwardRef(({ className, ...props }, ref) => {
  return (
    (<div
      ref={ref}
      data-sidebar="group"
      className={cn("relative flex w-full min-w-0 flex-col p-2", className)}
      {...props} />)
  );
})
SidebarGroup.displayName = "SidebarGroup"

const SidebarGroupLabel = React.forwardRef(({ className, asChild = false, ...props }, ref) => {
  const Comp = asChild ? Slot : "div"

  return (
    (<Comp
      ref={ref}
      data-sidebar="group-label"
      className={cn(
        "flex h-8 shrink-0 items-center rounded-md px-2 text-xs font-medium text-sidebar-foreground/70 outline-none ring-sidebar-ring transition-[margin,opacity] duration-200 ease-linear focus-visible:ring-2 [&>svg]:size-4 [&>svg]:shrink-0",
        "group-data-[collapsible=icon]:-mt-8 group-data-[collapsible=icon]:opacity-0",
        className
      )}
      {...props} />)
  );
})
SidebarGroupLabel.displayName = "SidebarGroupLabel"

const SidebarGroupAction = React.forwardRef(({ className, asChild = false, ...props }, ref) => {
  const Comp = asChild ? Slot : "button"

  return (
    (<Comp
      ref={ref}
      data-sidebar="group-action"
      className={cn(
        "absolute right-3 top-3.5 flex aspect-square w-5 items-center justify-center rounded-md p-0 text-sidebar-foreground outline-none ring-sidebar-ring transition-transform hover:bg-sidebar-accent hover:text-sidebar-accent-foreground focus-visible:ring-2 [&>svg]:size-4 [&>svg]:shrink-0",
        // Increases the hit area of the button on mobile.
        "after:absolute after:-inset-2 after:md:hidden",
        "group-data-[collapsible=icon]:hidden",
        className
      )}
      {...props} />)
  );
})
SidebarGroupAction.displayName = "SidebarGroupAction"

const SidebarGroupContent = React.forwardRef(({ className, ...props }, ref) => (
  <div
    ref={ref}
    data-sidebar="group-content"
    className={cn("w-full text-sm", className)}
    {...props} />
))
SidebarGroupContent.displayName = "SidebarGroupContent"

const SidebarMenu = React.forwardRef(({ className, ...props }, ref) => (
  <ul
    ref={ref}
    data-sidebar="menu"
    className={cn("flex w-full min-w-0 flex-col gap-1", className)}
    {...props} />
))
SidebarMenu.displayName = "SidebarMenu"

const SidebarMenuItem = React.forwardRef(({ className, ...props }, ref) => (
  <li
    ref={ref}
    data-sidebar="menu-item"
    className={cn("group/menu-item relative", className)}
    {...props} />
))
SidebarMenuItem.displayName = "SidebarMenuItem"

const sidebarMenuButtonVariants = cva(
  "peer/menu-button flex w-full items-center gap-2 overflow-hidden rounded-md p-2 text-left text-sm outline-none ring-sidebar-ring transition-[width,height,padding] hover:bg-sidebar-accent hover:text-sidebar-accent-foreground focus-visible:ring-2 active:bg-sidebar-accent active:text-sidebar-accent-foreground disabled:pointer-events-none disabled:opacity-50 group-has-[[data-sidebar=menu-action]]/menu-item:pr-8 aria-disabled:pointer-events-none aria-disabled:opacity-50 data-[active=true]:bg-sidebar-accent data-[active=true]:font-medium data-[active=true]:text-sidebar-accent-foreground data-[state=open]:hover:bg-sidebar-accent data-[state=open]:hover:text-sidebar-accent-foreground group-data-[collapsible=icon]:!size-8 group-data-[collapsible=icon]:!p-2 [&>span:last-child]:truncate [&>svg]:size-4 [&>svg]:shrink-0",
  {
    variants: {
      variant: {
        default: "hover:bg-sidebar-accent hover:text-sidebar-accent-foreground",
        outline:
          "bg-background shadow-[0_0_0_1px_hsl(var(--sidebar-border))] hover:bg-sidebar-accent hover:text-sidebar-accent-foreground hover:shadow-[0_0_0_1px_hsl(var(--sidebar-accent))]",
      },
      size: {
        default: "h-8 text-sm",
        sm: "h-7 text-xs",
        lg: "h-12 text-sm group-data-[collapsible=icon]:!p-0",
      },
    },
    defaultVariants: {
      variant: "default",
      size: "default",
    },
  }
)

const SidebarMenuButton = React.forwardRef((
  {
    asChild = false,
    isActive = false,
    variant = "default",
    size = "default",
    tooltip,
    className,
    ...props
  },
  ref
) => {
  const Comp = asChild ? Slot : "button"
  const { isMobile, state } = useSidebar()

  const button = (
    <Comp
      ref={ref}
      data-sidebar="menu-button"
      data-size={size}
      data-active={isActive}
      className={cn(sidebarMenuButtonVariants({ variant, size }), className)}
      {...props} />
  )

  if (!tooltip) {
    return button
  }

  if (typeof tooltip === "string") {
    tooltip = {
      children: tooltip,
    }
  }

  return (
    (<Tooltip>
      <TooltipTrigger asChild>{button}</TooltipTrigger>
      <TooltipContent
        side="right"
        align="center"
        hidden={state !== "collapsed" || isMobile}
        {...tooltip} />
    </Tooltip>)
  );
})
SidebarMenuButton.displayName = "SidebarMenuButton"

const SidebarMenuAction = React.forwardRef(({ className, asChild = false, showOnHover = false, ...props }, ref) => {
  const Comp = asChild ? Slot : "button"

  return (
    (<Comp
      ref={ref}
      data-sidebar="menu-action"
      className={cn(
        "absolute right-1 top-1.5 flex aspect-square w-5 items-center justify-center rounded-md p-0 text-sidebar-foreground outline-none ring-sidebar-ring transition-transform hover:bg-sidebar-accent hover:text-sidebar-accent-foreground focus-visible:ring-2 peer-hover/menu-button:text-sidebar-accent-foreground [&>svg]:size-4 [&>svg]:shrink-0",
        // Increases the hit area of the button on mobile.
        "after:absolute after:-inset-2 after:md:hidden",
        "peer-data-[size=sm]/menu-button:top-1",
        "peer-data-[size=default]/menu-button:top-1.5",
        "peer-data-[size=lg]/menu-button:top-2.5",
        "group-data-[collapsible=icon]:hidden",
        showOnHover &&
        "group-focus-within/menu-item:opacity-100 group-hover/menu-item:opacity-100 data-[state=open]:opacity-100 peer-data-[active=true]/menu-button:text-sidebar-accent-foreground md:opacity-0",
        className
      )}
      {...props} />)
  );
})
SidebarMenuAction.displayName = "SidebarMenuAction"

const SidebarMenuBadge = React.forwardRef(({ className, ...props }, ref) => (
  <div
    ref={ref}
    data-sidebar="menu-badge"
    className={cn(
      "pointer-events-none absolute right-1 flex h-5 min-w-5 select-none items-center justify-center rounded-md px-1 text-xs font-medium tabular-nums text-sidebar-foreground",
      "peer-hover/menu-button:text-sidebar-accent-foreground peer-data-[active=true]/menu-button:text-sidebar-accent-foreground",
      "peer-data-[size=sm]/menu-button:top-1",
      "peer-data-[size=default]/menu-button:top-1.5",
      "peer-data-[size=lg]/menu-button:top-2.5",
      "group-data-[collapsible=icon]:hidden",
      className
    )}
    {...props} />
))
SidebarMenuBadge.displayName = "SidebarMenuBadge"

const SidebarMenuSkeleton = React.forwardRef(({ className, showIcon = false, ...props }, ref) => {
  // Random width between 50 to 90%.
  const width = React.useMemo(() => {
    return `${Math.floor(Math.random() * 40) + 50}%`;
  }, [])

  return (
    (<div
      ref={ref}
      data-sidebar="menu-skeleton"
      className={cn("flex h-8 items-center gap-2 rounded-md px-2", className)}
      {...props}>
      {showIcon && (
        <Skeleton className="size-4 rounded-md" data-sidebar="menu-skeleton-icon" />
      )}
      <Skeleton
        className="h-4 max-w-[--skeleton-width] flex-1"
        data-sidebar="menu-skeleton-text"
        style={
          {
            "--skeleton-width": width
          }
        } />
    </div>)
  );
})
SidebarMenuSkeleton.displayName = "SidebarMenuSkeleton"

const SidebarMenuSub = React.forwardRef(({ className, ...props }, ref) => (
  <ul
    ref={ref}
    data-sidebar="menu-sub"
    className={cn(
      "mx-3.5 flex min-w-0 translate-x-px flex-col gap-1 border-l border-sidebar-border px-2.5 py-0.5",
      "group-data-[collapsible=icon]:hidden",
      className
    )}
    {...props} />
))
SidebarMenuSub.displayName = "SidebarMenuSub"

const SidebarMenuSubItem = React.forwardRef(({ ...props }, ref) => <li ref={ref} {...props} />)
SidebarMenuSubItem.displayName = "SidebarMenuSubItem"

const SidebarMenuSubButton = React.forwardRef(
  ({ asChild = false, size = "md", isActive, className, ...props }, ref) => {
    const Comp = asChild ? Slot : "a"

    return (
      (<Comp
        ref={ref}
        data-sidebar="menu-sub-button"
        data-size={size}
        data-active={isActive}
        className={cn(
          "flex h-7 min-w-0 -translate-x-px items-center gap-2 overflow-hidden rounded-md px-2 text-sidebar-foreground outline-none ring-sidebar-ring hover:bg-sidebar-accent hover:text-sidebar-accent-foreground focus-visible:ring-2 active:bg-sidebar-accent active:text-sidebar-accent-foreground disabled:pointer-events-none disabled:opacity-50 aria-disabled:pointer-events-none aria-disabled:opacity-50 [&>span:last-child]:truncate [&>svg]:size-4 [&>svg]:shrink-0 [&>svg]:text-sidebar-accent-foreground",
          "data-[active=true]:bg-sidebar-accent data-[active=true]:text-sidebar-accent-foreground",
          size === "sm" && "text-xs",
          size === "md" && "text-sm",
          "group-data-[collapsible=icon]:hidden",
          className
        )}
        {...props} />)
    );
  }
)
SidebarMenuSubButton.displayName = "SidebarMenuSubButton"

export {
  Sidebar,
  SidebarContent,
  SidebarFooter,
  SidebarGroup,
  SidebarGroupAction,
  SidebarGroupContent,
  SidebarGroupLabel,
  SidebarHeader,
  SidebarInput,
  SidebarInset,
  SidebarMenu,
  SidebarMenuAction,
  SidebarMenuBadge,
  SidebarMenuButton,
  SidebarMenuItem,
  SidebarMenuSkeleton,
  SidebarMenuSub,
  SidebarMenuSubButton,
  SidebarMenuSubItem,
  SidebarProvider,
  SidebarRail,
  SidebarSeparator,
  SidebarTrigger,
  useSidebar,
}

```

---

## File: `src/components/ui/calendar.jsx`

```text
import * as React from "react"
import { ChevronLeft, ChevronRight } from "lucide-react"
import { DayPicker } from "react-day-picker"

import { cn } from "@/lib/utils"
import { buttonVariants } from "@/components/ui/button"

function Calendar({
  className,
  classNames,
  showOutsideDays = true,
  ...props
}) {
  return (
    (<DayPicker
      showOutsideDays={showOutsideDays}
      className={cn("p-3", className)}
      classNames={{
        months: "flex flex-col sm:flex-row space-y-4 sm:space-x-4 sm:space-y-0",
        month: "space-y-4",
        caption: "flex justify-center pt-1 relative items-center",
        caption_label: "text-sm font-medium",
        nav: "space-x-1 flex items-center",
        nav_button: cn(
          buttonVariants({ variant: "outline" }),
          "h-7 w-7 bg-transparent p-0 opacity-50 hover:opacity-100"
        ),
        nav_button_previous: "absolute left-1",
        nav_button_next: "absolute right-1",
        table: "w-full border-collapse space-y-1",
        head_row: "flex",
        head_cell:
          "text-muted-foreground rounded-md w-8 font-normal text-[0.8rem]",
        row: "flex w-full mt-2",
        cell: cn(
          "relative p-0 text-center text-sm focus-within:relative focus-within:z-20 [&:has([aria-selected])]:bg-accent [&:has([aria-selected].day-outside)]:bg-accent/50 [&:has([aria-selected].day-range-end)]:rounded-r-md",
          props.mode === "range"
            ? "[&:has(>.day-range-end)]:rounded-r-md [&:has(>.day-range-start)]:rounded-l-md first:[&:has([aria-selected])]:rounded-l-md last:[&:has([aria-selected])]:rounded-r-md"
            : "[&:has([aria-selected])]:rounded-md"
        ),
        day: cn(
          buttonVariants({ variant: "ghost" }),
          "h-8 w-8 p-0 font-normal aria-selected:opacity-100"
        ),
        day_range_start: "day-range-start",
        day_range_end: "day-range-end",
        day_selected:
          "bg-primary text-primary-foreground hover:bg-primary hover:text-primary-foreground focus:bg-primary focus:text-primary-foreground",
        day_today: "bg-accent text-accent-foreground",
        day_outside:
          "day-outside text-muted-foreground aria-selected:bg-accent/50 aria-selected:text-muted-foreground",
        day_disabled: "text-muted-foreground opacity-50",
        day_range_middle:
          "aria-selected:bg-accent aria-selected:text-accent-foreground",
        day_hidden: "invisible",
        ...classNames,
      }}
      components={{
        IconLeft: ({ className, ...props }) => (
          <ChevronLeft className={cn("h-4 w-4", className)} {...props} />
        ),
        IconRight: ({ className, ...props }) => (
          <ChevronRight className={cn("h-4 w-4", className)} {...props} />
        ),
      }}
      {...props} />)
  );
}
Calendar.displayName = "Calendar"

export { Calendar }

```

---

## File: `src/components/ui/label.jsx`

```text
import * as React from "react"
import * as LabelPrimitive from "@radix-ui/react-label"
import { cva } from "class-variance-authority";

import { cn } from "@/lib/utils"

const labelVariants = cva(
  "text-sm font-medium leading-none peer-disabled:cursor-not-allowed peer-disabled:opacity-70"
)

const Label = React.forwardRef(({ className, ...props }, ref) => (
  <LabelPrimitive.Root ref={ref} className={cn(labelVariants(), className)} {...props} />
))
Label.displayName = LabelPrimitive.Root.displayName

export { Label }

```

---

## File: `src/components/ui/alert-dialog.jsx`

```text
import * as React from "react"
import * as AlertDialogPrimitive from "@radix-ui/react-alert-dialog"

import { cn } from "@/lib/utils"
import { buttonVariants } from "@/components/ui/button"

const AlertDialog = AlertDialogPrimitive.Root

const AlertDialogTrigger = AlertDialogPrimitive.Trigger

const AlertDialogPortal = AlertDialogPrimitive.Portal

const AlertDialogOverlay = React.forwardRef(({ className, ...props }, ref) => (
  <AlertDialogPrimitive.Overlay
    className={cn(
      "fixed inset-0 z-50 bg-black/80 data-[state=open]:animate-in data-[state=closed]:animate-out data-[state=closed]:fade-out-0 data-[state=open]:fade-in-0",
      className
    )}
    {...props}
    ref={ref} />
))
AlertDialogOverlay.displayName = AlertDialogPrimitive.Overlay.displayName

const AlertDialogContent = React.forwardRef(({ className, ...props }, ref) => (
  <AlertDialogPortal>
    <AlertDialogOverlay />
    <AlertDialogPrimitive.Content
      ref={ref}
      className={cn(
        "fixed left-[50%] top-[50%] z-50 grid w-full max-w-lg translate-x-[-50%] translate-y-[-50%] gap-4 border bg-background p-6 shadow-lg duration-200 data-[state=open]:animate-in data-[state=closed]:animate-out data-[state=closed]:fade-out-0 data-[state=open]:fade-in-0 data-[state=closed]:zoom-out-95 data-[state=open]:zoom-in-95 data-[state=closed]:slide-out-to-left-1/2 data-[state=closed]:slide-out-to-top-[48%] data-[state=open]:slide-in-from-left-1/2 data-[state=open]:slide-in-from-top-[48%] sm:rounded-lg",
        className
      )}
      {...props} />
  </AlertDialogPortal>
))
AlertDialogContent.displayName = AlertDialogPrimitive.Content.displayName

const AlertDialogHeader = ({
  className,
  ...props
}) => (
  <div
    className={cn("flex flex-col space-y-2 text-center sm:text-left", className)}
    {...props} />
)
AlertDialogHeader.displayName = "AlertDialogHeader"

const AlertDialogFooter = ({
  className,
  ...props
}) => (
  <div
    className={cn("flex flex-col-reverse sm:flex-row sm:justify-end sm:space-x-2", className)}
    {...props} />
)
AlertDialogFooter.displayName = "AlertDialogFooter"

const AlertDialogTitle = React.forwardRef(({ className, ...props }, ref) => (
  <AlertDialogPrimitive.Title ref={ref} className={cn("text-lg font-semibold", className)} {...props} />
))
AlertDialogTitle.displayName = AlertDialogPrimitive.Title.displayName

const AlertDialogDescription = React.forwardRef(({ className, ...props }, ref) => (
  <AlertDialogPrimitive.Description
    ref={ref}
    className={cn("text-sm text-muted-foreground", className)}
    {...props} />
))
AlertDialogDescription.displayName =
  AlertDialogPrimitive.Description.displayName

const AlertDialogAction = React.forwardRef(({ className, ...props }, ref) => (
  <AlertDialogPrimitive.Action ref={ref} className={cn(buttonVariants(), className)} {...props} />
))
AlertDialogAction.displayName = AlertDialogPrimitive.Action.displayName

const AlertDialogCancel = React.forwardRef(({ className, ...props }, ref) => (
  <AlertDialogPrimitive.Cancel
    ref={ref}
    className={cn(buttonVariants({ variant: "outline" }), "mt-2 sm:mt-0", className)}
    {...props} />
))
AlertDialogCancel.displayName = AlertDialogPrimitive.Cancel.displayName

export {
  AlertDialog,
  AlertDialogPortal,
  AlertDialogOverlay,
  AlertDialogTrigger,
  AlertDialogContent,
  AlertDialogHeader,
  AlertDialogFooter,
  AlertDialogTitle,
  AlertDialogDescription,
  AlertDialogAction,
  AlertDialogCancel,
}

```

---

## File: `src/components/ui/checkbox.jsx`

```text
import * as React from "react"
import * as CheckboxPrimitive from "@radix-ui/react-checkbox"
import { Check } from "lucide-react"

import { cn } from "@/lib/utils"

const Checkbox = React.forwardRef(({ className, ...props }, ref) => (
  <CheckboxPrimitive.Root
    ref={ref}
    className={cn(
      "peer h-4 w-4 shrink-0 rounded-sm border border-primary shadow focus-visible:outline-none focus-visible:ring-1 focus-visible:ring-ring disabled:cursor-not-allowed disabled:opacity-50 data-[state=checked]:bg-primary data-[state=checked]:text-primary-foreground",
      className
    )}
    {...props}>
    <CheckboxPrimitive.Indicator className={cn("flex items-center justify-center text-current")}>
      <Check className="h-4 w-4" />
    </CheckboxPrimitive.Indicator>
  </CheckboxPrimitive.Root>
))
Checkbox.displayName = CheckboxPrimitive.Root.displayName

export { Checkbox }

```

---

## File: `src/components/ui/use-toast.jsx`

```text
// Inspired by react-hot-toast library
import { useState, useEffect } from "react";

const TOAST_LIMIT = 20;
const TOAST_REMOVE_DELAY = 1000000;

const actionTypes = {
  ADD_TOAST: "ADD_TOAST",
  UPDATE_TOAST: "UPDATE_TOAST",
  DISMISS_TOAST: "DISMISS_TOAST",
  REMOVE_TOAST: "REMOVE_TOAST",
};

let count = 0;

function genId() {
  count = (count + 1) % Number.MAX_VALUE;
  return count.toString();
}

const toastTimeouts = new Map();

const addToRemoveQueue = (toastId) => {
  if (toastTimeouts.has(toastId)) {
    return;
  }

  const timeout = setTimeout(() => {
    toastTimeouts.delete(toastId);
    dispatch({
      type: actionTypes.REMOVE_TOAST,
      toastId,
    });
  }, TOAST_REMOVE_DELAY);

  toastTimeouts.set(toastId, timeout);
};

const _clearFromRemoveQueue = (toastId) => {
  const timeout = toastTimeouts.get(toastId);
  if (timeout) {
    clearTimeout(timeout);
    toastTimeouts.delete(toastId);
  }
};

export const reducer = (state, action) => {
  switch (action.type) {
    case actionTypes.ADD_TOAST:
      return {
        ...state,
        toasts: [action.toast, ...state.toasts].slice(0, TOAST_LIMIT),
      };

    case actionTypes.UPDATE_TOAST:
      return {
        ...state,
        toasts: state.toasts.map((t) =>
          t.id === action.toast.id ? { ...t, ...action.toast } : t
        ),
      };

    case actionTypes.DISMISS_TOAST: {
      const { toastId } = action;

      // ! Side effects ! - This could be extracted into a dismissToast() action,
      // but I'll keep it here for simplicity
      if (toastId) {
        addToRemoveQueue(toastId);
      } else {
        state.toasts.forEach((toast) => {
          addToRemoveQueue(toast.id);
        });
      }

      return {
        ...state,
        toasts: state.toasts.map((t) =>
          t.id === toastId || toastId === undefined
            ? {
                ...t,
                open: false,
              }
            : t
        ),
      };
    }
    case actionTypes.REMOVE_TOAST:
      if (action.toastId === undefined) {
        return {
          ...state,
          toasts: [],
        };
      }
      return {
        ...state,
        toasts: state.toasts.filter((t) => t.id !== action.toastId),
      };
  }
};

const listeners = [];

let memoryState = { toasts: [] };

function dispatch(action) {
  memoryState = reducer(memoryState, action);
  listeners.forEach((listener) => {
    listener(memoryState);
  });
}

function toast({ ...props }) {
  const id = genId();

  const update = (props) =>
    dispatch({
      type: actionTypes.UPDATE_TOAST,
      toast: { ...props, id },
    });

  const dismiss = () =>
    dispatch({ type: actionTypes.DISMISS_TOAST, toastId: id });

  dispatch({
    type: actionTypes.ADD_TOAST,
    toast: {
      ...props,
      id,
      open: true,
      onOpenChange: (open) => {
        if (!open) dismiss();
      },
    },
  });

  return {
    id,
    dismiss,
    update,
  };
}

function useToast() {
  const [state, setState] = useState(memoryState);

  useEffect(() => {
    listeners.push(setState);
    return () => {
      const index = listeners.indexOf(setState);
      if (index > -1) {
        listeners.splice(index, 1);
      }
    };
  }, [state]);

  return {
    ...state,
    toast,
    dismiss: (toastId) => dispatch({ type: actionTypes.DISMISS_TOAST, toastId }),
  };
}

export { useToast, toast }; 
```

---

## File: `src/components/ui/sheet.jsx`

```text
"use client";
import * as React from "react"
import * as SheetPrimitive from "@radix-ui/react-dialog"
import { cva } from "class-variance-authority";
import { X } from "lucide-react"

import { cn } from "@/lib/utils"

const Sheet = SheetPrimitive.Root

const SheetTrigger = SheetPrimitive.Trigger

const SheetClose = SheetPrimitive.Close

const SheetPortal = SheetPrimitive.Portal

const SheetOverlay = React.forwardRef(({ className, ...props }, ref) => (
  <SheetPrimitive.Overlay
    className={cn(
      "fixed inset-0 z-50 bg-black/80  data-[state=open]:animate-in data-[state=closed]:animate-out data-[state=closed]:fade-out-0 data-[state=open]:fade-in-0",
      className
    )}
    {...props}
    ref={ref} />
))
SheetOverlay.displayName = SheetPrimitive.Overlay.displayName

const sheetVariants = cva(
  "fixed z-50 gap-4 bg-background p-6 shadow-lg transition ease-in-out data-[state=closed]:duration-300 data-[state=open]:duration-500 data-[state=open]:animate-in data-[state=closed]:animate-out",
  {
    variants: {
      side: {
        top: "inset-x-0 top-0 border-b data-[state=closed]:slide-out-to-top data-[state=open]:slide-in-from-top",
        bottom:
          "inset-x-0 bottom-0 border-t data-[state=closed]:slide-out-to-bottom data-[state=open]:slide-in-from-bottom",
        left: "inset-y-0 left-0 h-full w-3/4 border-r data-[state=closed]:slide-out-to-left data-[state=open]:slide-in-from-left sm:max-w-sm",
        right:
          "inset-y-0 right-0 h-full w-3/4 border-l data-[state=closed]:slide-out-to-right data-[state=open]:slide-in-from-right sm:max-w-sm",
      },
    },
    defaultVariants: {
      side: "right",
    },
  }
)

const SheetContent = React.forwardRef(({ side = "right", className, children, ...props }, ref) => (
  <SheetPortal>
    <SheetOverlay />
    <SheetPrimitive.Content ref={ref} className={cn(sheetVariants({ side }), className)} {...props}>
      <SheetPrimitive.Close
        className="absolute right-4 top-4 rounded-sm opacity-70 ring-offset-background transition-opacity hover:opacity-100 focus:outline-none focus:ring-2 focus:ring-ring focus:ring-offset-2 disabled:pointer-events-none data-[state=open]:bg-secondary">
        <X className="h-4 w-4" />
        <span className="sr-only">Close</span>
      </SheetPrimitive.Close>
      {children}
    </SheetPrimitive.Content>
  </SheetPortal>
))
SheetContent.displayName = SheetPrimitive.Content.displayName

const SheetHeader = ({
  className,
  ...props
}) => (
  <div
    className={cn("flex flex-col space-y-2 text-center sm:text-left", className)}
    {...props} />
)
SheetHeader.displayName = "SheetHeader"

const SheetFooter = ({
  className,
  ...props
}) => (
  <div
    className={cn("flex flex-col-reverse sm:flex-row sm:justify-end sm:space-x-2", className)}
    {...props} />
)
SheetFooter.displayName = "SheetFooter"

const SheetTitle = React.forwardRef(({ className, ...props }, ref) => (
  <SheetPrimitive.Title
    ref={ref}
    className={cn("text-lg font-semibold text-foreground", className)}
    {...props} />
))
SheetTitle.displayName = SheetPrimitive.Title.displayName

const SheetDescription = React.forwardRef(({ className, ...props }, ref) => (
  <SheetPrimitive.Description
    ref={ref}
    className={cn("text-sm text-muted-foreground", className)}
    {...props} />
))
SheetDescription.displayName = SheetPrimitive.Description.displayName

export {
  Sheet,
  SheetPortal,
  SheetOverlay,
  SheetTrigger,
  SheetClose,
  SheetContent,
  SheetHeader,
  SheetFooter,
  SheetTitle,
  SheetDescription,
}

```

---

## File: `src/components/ui/badge.jsx`

```text
import * as React from "react"
import { cva } from "class-variance-authority";

import { cn } from "@/lib/utils"

const badgeVariants = cva(
  "inline-flex items-center rounded-md border px-2.5 py-0.5 text-xs font-semibold transition-colors focus:outline-none focus:ring-2 focus:ring-ring focus:ring-offset-2",
  {
    variants: {
      variant: {
        default:
          "border-transparent bg-primary text-primary-foreground shadow hover:bg-primary/80",
        secondary:
          "border-transparent bg-secondary text-secondary-foreground hover:bg-secondary/80",
        destructive:
          "border-transparent bg-destructive text-destructive-foreground shadow hover:bg-destructive/80",
        outline: "text-foreground",
      },
    },
    defaultVariants: {
      variant: "default",
    },
  }
)

function Badge({
  className,
  variant,
  ...props
}) {
  return (<div className={cn(badgeVariants({ variant }), className)} {...props} />);
}

export { Badge, badgeVariants }

```

---

## File: `src/components/ui/carousel.jsx`

```text
import * as React from "react"
import useEmblaCarousel from "embla-carousel-react";
import { ArrowLeft, ArrowRight } from "lucide-react"

import { cn } from "@/lib/utils"
import { Button } from "@/components/ui/button"

const CarouselContext = React.createContext(null)

function useCarousel() {
  const context = React.useContext(CarouselContext)

  if (!context) {
    throw new Error("useCarousel must be used within a <Carousel />")
  }

  return context
}

const Carousel = React.forwardRef((
  {
    orientation = "horizontal",
    opts,
    setApi,
    plugins,
    className,
    children,
    ...props
  },
  ref
) => {
  const [carouselRef, api] = useEmblaCarousel({
    ...opts,
    axis: orientation === "horizontal" ? "x" : "y",
  }, plugins)
  const [canScrollPrev, setCanScrollPrev] = React.useState(false)
  const [canScrollNext, setCanScrollNext] = React.useState(false)

  const onSelect = React.useCallback((api) => {
    if (!api) {
      return
    }

    setCanScrollPrev(api.canScrollPrev())
    setCanScrollNext(api.canScrollNext())
  }, [])

  const scrollPrev = React.useCallback(() => {
    api?.scrollPrev()
  }, [api])

  const scrollNext = React.useCallback(() => {
    api?.scrollNext()
  }, [api])

  const handleKeyDown = React.useCallback((event) => {
    if (event.key === "ArrowLeft") {
      event.preventDefault()
      scrollPrev()
    } else if (event.key === "ArrowRight") {
      event.preventDefault()
      scrollNext()
    }
  }, [scrollPrev, scrollNext])

  React.useEffect(() => {
    if (!api || !setApi) {
      return
    }

    setApi(api)
  }, [api, setApi])

  React.useEffect(() => {
    if (!api) {
      return
    }

    onSelect(api)
    api.on("reInit", onSelect)
    api.on("select", onSelect)

    return () => {
      api?.off("select", onSelect)
    };
  }, [api, onSelect])

  return (
    (<CarouselContext.Provider
      value={{
        carouselRef,
        api: api,
        opts,
        orientation:
          orientation || (opts?.axis === "y" ? "vertical" : "horizontal"),
        scrollPrev,
        scrollNext,
        canScrollPrev,
        canScrollNext,
      }}>
      <div
        ref={ref}
        onKeyDownCapture={handleKeyDown}
        className={cn("relative", className)}
        role="region"
        aria-roledescription="carousel"
        {...props}>
        {children}
      </div>
    </CarouselContext.Provider>)
  );
})
Carousel.displayName = "Carousel"

const CarouselContent = React.forwardRef(({ className, ...props }, ref) => {
  const { carouselRef, orientation } = useCarousel()

  return (
    (<div ref={carouselRef} className="overflow-hidden">
      <div
        ref={ref}
        className={cn(
          "flex",
          orientation === "horizontal" ? "-ml-4" : "-mt-4 flex-col",
          className
        )}
        {...props} />
    </div>)
  );
})
CarouselContent.displayName = "CarouselContent"

const CarouselItem = React.forwardRef(({ className, ...props }, ref) => {
  const { orientation } = useCarousel()

  return (
    (<div
      ref={ref}
      role="group"
      aria-roledescription="slide"
      className={cn(
        "min-w-0 shrink-0 grow-0 basis-full",
        orientation === "horizontal" ? "pl-4" : "pt-4",
        className
      )}
      {...props} />)
  );
})
CarouselItem.displayName = "CarouselItem"

const CarouselPrevious = React.forwardRef(({ className, variant = "outline", size = "icon", ...props }, ref) => {
  const { orientation, scrollPrev, canScrollPrev } = useCarousel()

  return (
    (<Button
      ref={ref}
      variant={variant}
      size={size}
      className={cn("absolute  h-8 w-8 rounded-full", orientation === "horizontal"
        ? "-left-12 top-1/2 -translate-y-1/2"
        : "-top-12 left-1/2 -translate-x-1/2 rotate-90", className)}
      disabled={!canScrollPrev}
      onClick={scrollPrev}
      {...props}>
      <ArrowLeft className="h-4 w-4" />
      <span className="sr-only">Previous slide</span>
    </Button>)
  );
})
CarouselPrevious.displayName = "CarouselPrevious"

const CarouselNext = React.forwardRef(({ className, variant = "outline", size = "icon", ...props }, ref) => {
  const { orientation, scrollNext, canScrollNext } = useCarousel()

  return (
    (<Button
      ref={ref}
      variant={variant}
      size={size}
      className={cn("absolute h-8 w-8 rounded-full", orientation === "horizontal"
        ? "-right-12 top-1/2 -translate-y-1/2"
        : "-bottom-12 left-1/2 -translate-x-1/2 rotate-90", className)}
      disabled={!canScrollNext}
      onClick={scrollNext}
      {...props}>
      <ArrowRight className="h-4 w-4" />
      <span className="sr-only">Next slide</span>
    </Button>)
  );
})
CarouselNext.displayName = "CarouselNext"

export { Carousel, CarouselContent, CarouselItem, CarouselPrevious, CarouselNext };

```

---

## File: `src/components/ui/pagination.jsx`

```text
import * as React from "react"
import { ChevronLeft, ChevronRight, MoreHorizontal } from "lucide-react"

import { cn } from "@/lib/utils"
import { buttonVariants } from "@/components/ui/button";

const Pagination = ({
  className,
  ...props
}) => (
  <nav
    role="navigation"
    aria-label="pagination"
    className={cn("mx-auto flex w-full justify-center", className)}
    {...props} />
)
Pagination.displayName = "Pagination"

const PaginationContent = React.forwardRef(({ className, ...props }, ref) => (
  <ul
    ref={ref}
    className={cn("flex flex-row items-center gap-1", className)}
    {...props} />
))
PaginationContent.displayName = "PaginationContent"

const PaginationItem = React.forwardRef(({ className, ...props }, ref) => (
  <li ref={ref} className={cn("", className)} {...props} />
))
PaginationItem.displayName = "PaginationItem"

const PaginationLink = ({
  className,
  isActive,
  size = "icon",
  ...props
}) => (
  <a
    aria-current={isActive ? "page" : undefined}
    className={cn(buttonVariants({
      variant: isActive ? "outline" : "ghost",
      size,
    }), className)}
    {...props} />
)
PaginationLink.displayName = "PaginationLink"

const PaginationPrevious = ({
  className,
  ...props
}) => (
  <PaginationLink
    aria-label="Go to previous page"
    size="default"
    className={cn("gap-1 pl-2.5", className)}
    {...props}>
    <ChevronLeft className="h-4 w-4" />
    <span>Previous</span>
  </PaginationLink>
)
PaginationPrevious.displayName = "PaginationPrevious"

const PaginationNext = ({
  className,
  ...props
}) => (
  <PaginationLink
    aria-label="Go to next page"
    size="default"
    className={cn("gap-1 pr-2.5", className)}
    {...props}>
    <span>Next</span>
    <ChevronRight className="h-4 w-4" />
  </PaginationLink>
)
PaginationNext.displayName = "PaginationNext"

const PaginationEllipsis = ({
  className,
  ...props
}) => (
  <span
    aria-hidden
    className={cn("flex h-9 w-9 items-center justify-center", className)}
    {...props}>
    <MoreHorizontal className="h-4 w-4" />
    <span className="sr-only">More pages</span>
  </span>
)
PaginationEllipsis.displayName = "PaginationEllipsis"

export {
  Pagination,
  PaginationContent,
  PaginationLink,
  PaginationItem,
  PaginationPrevious,
  PaginationNext,
  PaginationEllipsis,
}

```

---

## File: `src/components/ui/command.jsx`

```text
import * as React from "react"
import { Command as CommandPrimitive } from "cmdk"
import { Search } from "lucide-react"

import { cn } from "@/lib/utils"
import { Dialog, DialogContent } from "@/components/ui/dialog"

const Command = React.forwardRef(({ className, ...props }, ref) => (
  <CommandPrimitive
    ref={ref}
    className={cn(
      "flex h-full w-full flex-col overflow-hidden rounded-md bg-popover text-popover-foreground",
      className
    )}
    {...props} />
))
Command.displayName = CommandPrimitive.displayName

const CommandDialog = ({
  children,
  ...props
}) => {
  return (
    (<Dialog {...props}>
      <DialogContent className="overflow-hidden p-0">
        <Command
          className="[&_[cmdk-group-heading]]:px-2 [&_[cmdk-group-heading]]:font-medium [&_[cmdk-group-heading]]:text-muted-foreground [&_[cmdk-group]:not([hidden])_~[cmdk-group]]:pt-0 [&_[cmdk-group]]:px-2 [&_[cmdk-input-wrapper]_svg]:h-5 [&_[cmdk-input-wrapper]_svg]:w-5 [&_[cmdk-input]]:h-12 [&_[cmdk-item]]:px-2 [&_[cmdk-item]]:py-3 [&_[cmdk-item]_svg]:h-5 [&_[cmdk-item]_svg]:w-5">
          {children}
        </Command>
      </DialogContent>
    </Dialog>)
  );
}

const CommandInput = React.forwardRef(({ className, ...props }, ref) => (
  <div className="flex items-center border-b px-3" cmdk-input-wrapper="">
    <Search className="mr-2 h-4 w-4 shrink-0 opacity-50" />
    <CommandPrimitive.Input
      ref={ref}
      className={cn(
        "flex h-10 w-full rounded-md bg-transparent py-3 text-sm outline-none placeholder:text-muted-foreground disabled:cursor-not-allowed disabled:opacity-50",
        className
      )}
      {...props} />
  </div>
))

CommandInput.displayName = CommandPrimitive.Input.displayName

const CommandList = React.forwardRef(({ className, ...props }, ref) => (
  <CommandPrimitive.List
    ref={ref}
    className={cn("max-h-[300px] overflow-y-auto overflow-x-hidden", className)}
    {...props} />
))

CommandList.displayName = CommandPrimitive.List.displayName

const CommandEmpty = React.forwardRef((props, ref) => (
  <CommandPrimitive.Empty ref={ref} className="py-6 text-center text-sm" {...props} />
))

CommandEmpty.displayName = CommandPrimitive.Empty.displayName

const CommandGroup = React.forwardRef(({ className, ...props }, ref) => (
  <CommandPrimitive.Group
    ref={ref}
    className={cn(
      "overflow-hidden p-1 text-foreground [&_[cmdk-group-heading]]:px-2 [&_[cmdk-group-heading]]:py-1.5 [&_[cmdk-group-heading]]:text-xs [&_[cmdk-group-heading]]:font-medium [&_[cmdk-group-heading]]:text-muted-foreground",
      className
    )}
    {...props} />
))

CommandGroup.displayName = CommandPrimitive.Group.displayName

const CommandSeparator = React.forwardRef(({ className, ...props }, ref) => (
  <CommandPrimitive.Separator ref={ref} className={cn("-mx-1 h-px bg-border", className)} {...props} />
))
CommandSeparator.displayName = CommandPrimitive.Separator.displayName

const CommandItem = React.forwardRef(({ className, ...props }, ref) => (
  <CommandPrimitive.Item
    ref={ref}
    className={cn(
      "relative flex cursor-default gap-2 select-none items-center rounded-sm px-2 py-1.5 text-sm outline-none data-[disabled=true]:pointer-events-none data-[selected=true]:bg-accent data-[selected=true]:text-accent-foreground data-[disabled=true]:opacity-50 [&_svg]:pointer-events-none [&_svg]:size-4 [&_svg]:shrink-0",
      className
    )}
    {...props} />
))

CommandItem.displayName = CommandPrimitive.Item.displayName

const CommandShortcut = ({
  className,
  ...props
}) => {
  return (
    (<span
      className={cn("ml-auto text-xs tracking-widest text-muted-foreground", className)}
      {...props} />)
  );
}
CommandShortcut.displayName = "CommandShortcut"

export {
  Command,
  CommandDialog,
  CommandInput,
  CommandList,
  CommandEmpty,
  CommandGroup,
  CommandItem,
  CommandShortcut,
  CommandSeparator,
}

```

---

## File: `src/components/ui/form.jsx`

```text
"use client";
import * as React from "react"
import { Slot } from "@radix-ui/react-slot"
import { Controller, FormProvider, useFormContext } from "react-hook-form";

import { cn } from "@/lib/utils"
import { Label } from "@/components/ui/label"

const Form = FormProvider

const FormFieldContext = React.createContext({})

const FormField = (
  {
    ...props
  }
) => {
  return (
    (<FormFieldContext.Provider value={{ name: props.name }}>
      <Controller {...props} />
    </FormFieldContext.Provider>)
  );
}

const useFormField = () => {
  const fieldContext = React.useContext(FormFieldContext)
  const itemContext = React.useContext(FormItemContext)
  const { getFieldState, formState } = useFormContext()

  const fieldState = getFieldState(fieldContext.name, formState)

  if (!fieldContext) {
    throw new Error("useFormField should be used within <FormField>")
  }

  const { id } = itemContext

  return {
    id,
    name: fieldContext.name,
    formItemId: `${id}-form-item`,
    formDescriptionId: `${id}-form-item-description`,
    formMessageId: `${id}-form-item-message`,
    ...fieldState,
  }
}

const FormItemContext = React.createContext({})

const FormItem = React.forwardRef(({ className, ...props }, ref) => {
  const id = React.useId()

  return (
    (<FormItemContext.Provider value={{ id }}>
      <div ref={ref} className={cn("space-y-2", className)} {...props} />
    </FormItemContext.Provider>)
  );
})
FormItem.displayName = "FormItem"

const FormLabel = React.forwardRef(({ className, ...props }, ref) => {
  const { error, formItemId } = useFormField()

  return (
    (<Label
      ref={ref}
      className={cn(error && "text-destructive", className)}
      htmlFor={formItemId}
      {...props} />)
  );
})
FormLabel.displayName = "FormLabel"

const FormControl = React.forwardRef(({ ...props }, ref) => {
  const { error, formItemId, formDescriptionId, formMessageId } = useFormField()

  return (
    (<Slot
      ref={ref}
      id={formItemId}
      aria-describedby={
        !error
          ? `${formDescriptionId}`
          : `${formDescriptionId} ${formMessageId}`
      }
      aria-invalid={!!error}
      {...props} />)
  );
})
FormControl.displayName = "FormControl"

const FormDescription = React.forwardRef(({ className, ...props }, ref) => {
  const { formDescriptionId } = useFormField()

  return (
    (<p
      ref={ref}
      id={formDescriptionId}
      className={cn("text-[0.8rem] text-muted-foreground", className)}
      {...props} />)
  );
})
FormDescription.displayName = "FormDescription"

const FormMessage = React.forwardRef(({ className, children, ...props }, ref) => {
  const { error, formMessageId } = useFormField()
  const body = error ? String(error?.message) : children

  if (!body) {
    return null
  }

  return (
    (<p
      ref={ref}
      id={formMessageId}
      className={cn("text-[0.8rem] font-medium text-destructive", className)}
      {...props}>
      {body}
    </p>)
  );
})
FormMessage.displayName = "FormMessage"

export {
  useFormField,
  Form,
  FormItem,
  FormLabel,
  FormControl,
  FormDescription,
  FormMessage,
  FormField,
}

```

---

## File: `src/components/ui/skeleton.jsx`

```text
import { cn } from "@/lib/utils"

function Skeleton({
  className,
  ...props
}) {
  return (
    (<div
      className={cn("animate-pulse rounded-md bg-primary/10", className)}
      {...props} />)
  );
}

export { Skeleton }

```

---

## File: `src/components/ui/select.jsx`

```text
"use client"

import * as React from "react"
import * as SelectPrimitive from "@radix-ui/react-select"
import { Check, ChevronDown, ChevronUp } from "lucide-react"

import { cn } from "@/lib/utils"

const Select = SelectPrimitive.Root

const SelectGroup = SelectPrimitive.Group

const SelectValue = SelectPrimitive.Value

const SelectTrigger = React.forwardRef(({ className, children, ...props }, ref) => (
  <SelectPrimitive.Trigger
    ref={ref}
    className={cn(
      "flex h-9 w-full items-center justify-between whitespace-nowrap rounded-md border border-input bg-transparent px-3 py-2 text-sm shadow-sm ring-offset-background data-[placeholder]:text-muted-foreground focus:outline-none focus:ring-1 focus:ring-ring disabled:cursor-not-allowed disabled:opacity-50 [&>span]:line-clamp-1",
      className
    )}
    {...props}>
    {children}
    <SelectPrimitive.Icon asChild>
      <ChevronDown className="h-4 w-4 opacity-50" />
    </SelectPrimitive.Icon>
  </SelectPrimitive.Trigger>
))
SelectTrigger.displayName = SelectPrimitive.Trigger.displayName

const SelectScrollUpButton = React.forwardRef(({ className, ...props }, ref) => (
  <SelectPrimitive.ScrollUpButton
    ref={ref}
    className={cn("flex cursor-default items-center justify-center py-1", className)}
    {...props}>
    <ChevronUp className="h-4 w-4" />
  </SelectPrimitive.ScrollUpButton>
))
SelectScrollUpButton.displayName = SelectPrimitive.ScrollUpButton.displayName

const SelectScrollDownButton = React.forwardRef(({ className, ...props }, ref) => (
  <SelectPrimitive.ScrollDownButton
    ref={ref}
    className={cn("flex cursor-default items-center justify-center py-1", className)}
    {...props}>
    <ChevronDown className="h-4 w-4" />
  </SelectPrimitive.ScrollDownButton>
))
SelectScrollDownButton.displayName =
  SelectPrimitive.ScrollDownButton.displayName

const SelectContent = React.forwardRef(({ className, children, position = "popper", ...props }, ref) => (
  <SelectPrimitive.Portal>
    <SelectPrimitive.Content
      ref={ref}
      className={cn(
        "relative z-50 max-h-96 min-w-[8rem] overflow-hidden rounded-md border bg-popover text-popover-foreground shadow-md data-[state=open]:animate-in data-[state=closed]:animate-out data-[state=closed]:fade-out-0 data-[state=open]:fade-in-0 data-[state=closed]:zoom-out-95 data-[state=open]:zoom-in-95 data-[side=bottom]:slide-in-from-top-2 data-[side=left]:slide-in-from-right-2 data-[side=right]:slide-in-from-left-2 data-[side=top]:slide-in-from-bottom-2",
        position === "popper" &&
          "data-[side=bottom]:translate-y-1 data-[side=left]:-translate-x-1 data-[side=right]:translate-x-1 data-[side=top]:-translate-y-1",
        className
      )}
      position={position}
      {...props}>
      <SelectScrollUpButton />
      <SelectPrimitive.Viewport
        className={cn("p-1", position === "popper" &&
          "h-[var(--radix-select-trigger-height)] w-full min-w-[var(--radix-select-trigger-width)]")}>
        {children}
      </SelectPrimitive.Viewport>
      <SelectScrollDownButton />
    </SelectPrimitive.Content>
  </SelectPrimitive.Portal>
))
SelectContent.displayName = SelectPrimitive.Content.displayName

const SelectLabel = React.forwardRef(({ className, ...props }, ref) => (
  <SelectPrimitive.Label
    ref={ref}
    className={cn("px-2 py-1.5 text-sm font-semibold", className)}
    {...props} />
))
SelectLabel.displayName = SelectPrimitive.Label.displayName

const SelectItem = React.forwardRef(({ className, children, ...props }, ref) => (
  <SelectPrimitive.Item
    ref={ref}
    className={cn(
      "relative flex w-full cursor-default select-none items-center rounded-sm py-1.5 pl-2 pr-8 text-sm outline-none focus:bg-accent focus:text-accent-foreground data-[disabled]:pointer-events-none data-[disabled]:opacity-50",
      className
    )}
    {...props}>
    <span className="absolute right-2 flex h-3.5 w-3.5 items-center justify-center">
      <SelectPrimitive.ItemIndicator>
        <Check className="h-4 w-4" />
      </SelectPrimitive.ItemIndicator>
    </span>
    <SelectPrimitive.ItemText>{children}</SelectPrimitive.ItemText>
  </SelectPrimitive.Item>
))
SelectItem.displayName = SelectPrimitive.Item.displayName

const SelectSeparator = React.forwardRef(({ className, ...props }, ref) => (
  <SelectPrimitive.Separator
    ref={ref}
    className={cn("-mx-1 my-1 h-px bg-muted", className)}
    {...props} />
))
SelectSeparator.displayName = SelectPrimitive.Separator.displayName

export {
  Select,
  SelectGroup,
  SelectValue,
  SelectTrigger,
  SelectContent,
  SelectLabel,
  SelectItem,
  SelectSeparator,
  SelectScrollUpButton,
  SelectScrollDownButton,
}

```

---

## File: `src/components/ui/alert.jsx`

```text
import * as React from "react"
import { cva } from "class-variance-authority";

import { cn } from "@/lib/utils"

const alertVariants = cva(
  "relative w-full rounded-lg border px-4 py-3 text-sm [&>svg+div]:translate-y-[-3px] [&>svg]:absolute [&>svg]:left-4 [&>svg]:top-4 [&>svg]:text-foreground [&>svg~*]:pl-7",
  {
    variants: {
      variant: {
        default: "bg-background text-foreground",
        destructive:
          "border-destructive/50 text-destructive dark:border-destructive [&>svg]:text-destructive",
      },
    },
    defaultVariants: {
      variant: "default",
    },
  }
)

const Alert = React.forwardRef(({ className, variant, ...props }, ref) => (
  <div
    ref={ref}
    role="alert"
    className={cn(alertVariants({ variant }), className)}
    {...props} />
))
Alert.displayName = "Alert"

const AlertTitle = React.forwardRef(({ className, ...props }, ref) => (
  <h5
    ref={ref}
    className={cn("mb-1 font-medium leading-none tracking-tight", className)}
    {...props} />
))
AlertTitle.displayName = "AlertTitle"

const AlertDescription = React.forwardRef(({ className, ...props }, ref) => (
  <div
    ref={ref}
    className={cn("text-sm [&_p]:leading-relaxed", className)}
    {...props} />
))
AlertDescription.displayName = "AlertDescription"

export { Alert, AlertTitle, AlertDescription }

```

---

## File: `src/components/ui/dialog.jsx`

```text
"use client"

import * as React from "react"
import * as DialogPrimitive from "@radix-ui/react-dialog"
import { X } from "lucide-react"

import { cn } from "@/lib/utils"

const Dialog = DialogPrimitive.Root

const DialogTrigger = DialogPrimitive.Trigger

const DialogPortal = DialogPrimitive.Portal

const DialogClose = DialogPrimitive.Close

const DialogOverlay = React.forwardRef(({ className, ...props }, ref) => (
  <DialogPrimitive.Overlay
    ref={ref}
    className={cn(
      "fixed inset-0 z-50 bg-black/80  data-[state=open]:animate-in data-[state=closed]:animate-out data-[state=closed]:fade-out-0 data-[state=open]:fade-in-0",
      className
    )}
    {...props} />
))
DialogOverlay.displayName = DialogPrimitive.Overlay.displayName

const DialogContent = React.forwardRef(({ className, children, ...props }, ref) => (
  <DialogPortal>
    <DialogOverlay />
    <DialogPrimitive.Content
      ref={ref}
      className={cn(
        "fixed left-[50%] top-[50%] z-50 grid w-full max-w-lg translate-x-[-50%] translate-y-[-50%] gap-4 border bg-background p-6 shadow-lg duration-200 data-[state=open]:animate-in data-[state=closed]:animate-out data-[state=closed]:fade-out-0 data-[state=open]:fade-in-0 data-[state=closed]:zoom-out-95 data-[state=open]:zoom-in-95 data-[state=closed]:slide-out-to-left-1/2 data-[state=closed]:slide-out-to-top-[48%] data-[state=open]:slide-in-from-left-1/2 data-[state=open]:slide-in-from-top-[48%] sm:rounded-lg",
        className
      )}
      {...props}>
      {children}
      <DialogPrimitive.Close
        className="absolute right-4 top-4 rounded-sm opacity-70 ring-offset-background transition-opacity hover:opacity-100 focus:outline-none focus:ring-2 focus:ring-ring focus:ring-offset-2 disabled:pointer-events-none data-[state=open]:bg-accent data-[state=open]:text-muted-foreground">
        <X className="h-4 w-4" />
        <span className="sr-only">Close</span>
      </DialogPrimitive.Close>
    </DialogPrimitive.Content>
  </DialogPortal>
))
DialogContent.displayName = DialogPrimitive.Content.displayName

const DialogHeader = ({
  className,
  ...props
}) => (
  <div
    className={cn("flex flex-col space-y-1.5 text-center sm:text-left", className)}
    {...props} />
)
DialogHeader.displayName = "DialogHeader"

const DialogFooter = ({
  className,
  ...props
}) => (
  <div
    className={cn("flex flex-col-reverse sm:flex-row sm:justify-end sm:space-x-2", className)}
    {...props} />
)
DialogFooter.displayName = "DialogFooter"

const DialogTitle = React.forwardRef(({ className, ...props }, ref) => (
  <DialogPrimitive.Title
    ref={ref}
    className={cn("text-lg font-semibold leading-none tracking-tight", className)}
    {...props} />
))
DialogTitle.displayName = DialogPrimitive.Title.displayName

const DialogDescription = React.forwardRef(({ className, ...props }, ref) => (
  <DialogPrimitive.Description
    ref={ref}
    className={cn("text-sm text-muted-foreground", className)}
    {...props} />
))
DialogDescription.displayName = DialogPrimitive.Description.displayName

export {
  Dialog,
  DialogPortal,
  DialogOverlay,
  DialogTrigger,
  DialogClose,
  DialogContent,
  DialogHeader,
  DialogFooter,
  DialogTitle,
  DialogDescription,
}

```

---

## File: `src/components/ui/resizable.jsx`

```text
"use client"

import { GripVertical } from "lucide-react"
import * as ResizablePrimitive from "react-resizable-panels"

import { cn } from "@/lib/utils"

const ResizablePanelGroup = ({
  className,
  ...props
}) => (
  <ResizablePrimitive.PanelGroup
    className={cn(
      "flex h-full w-full data-[panel-group-direction=vertical]:flex-col",
      className
    )}
    {...props} />
)

const ResizablePanel = ResizablePrimitive.Panel

const ResizableHandle = ({
  withHandle,
  className,
  ...props
}) => (
  <ResizablePrimitive.PanelResizeHandle
    className={cn(
      "relative flex w-px items-center justify-center bg-border after:absolute after:inset-y-0 after:left-1/2 after:w-1 after:-translate-x-1/2 focus-visible:outline-none focus-visible:ring-1 focus-visible:ring-ring focus-visible:ring-offset-1 data-[panel-group-direction=vertical]:h-px data-[panel-group-direction=vertical]:w-full data-[panel-group-direction=vertical]:after:left-0 data-[panel-group-direction=vertical]:after:h-1 data-[panel-group-direction=vertical]:after:w-full data-[panel-group-direction=vertical]:after:-translate-y-1/2 data-[panel-group-direction=vertical]:after:translate-x-0 [&[data-panel-group-direction=vertical]>div]:rotate-90",
      className
    )}
    {...props}>
    {withHandle && (
      <div
        className="z-10 flex h-4 w-3 items-center justify-center rounded-sm border bg-border">
        <GripVertical className="h-2.5 w-2.5" />
      </div>
    )}
  </ResizablePrimitive.PanelResizeHandle>
)

export { ResizablePanelGroup, ResizablePanel, ResizableHandle }

```

---

## File: `src/components/ui/slider.jsx`

```text
import * as React from "react"
import * as SliderPrimitive from "@radix-ui/react-slider"

import { cn } from "@/lib/utils"

const Slider = React.forwardRef(({ className, ...props }, ref) => (
  <SliderPrimitive.Root
    ref={ref}
    className={cn("relative flex w-full touch-none select-none items-center", className)}
    {...props}>
    <SliderPrimitive.Track
      className="relative h-1.5 w-full grow overflow-hidden rounded-full bg-primary/20">
      <SliderPrimitive.Range className="absolute h-full bg-primary" />
    </SliderPrimitive.Track>
    <SliderPrimitive.Thumb
      className="block h-4 w-4 rounded-full border border-primary/50 bg-background shadow transition-colors focus-visible:outline-none focus-visible:ring-1 focus-visible:ring-ring disabled:pointer-events-none disabled:opacity-50" />
  </SliderPrimitive.Root>
))
Slider.displayName = SliderPrimitive.Root.displayName

export { Slider }

```

---

## File: `src/components/ui/context-menu.jsx`

```text
import * as React from "react"
import * as ContextMenuPrimitive from "@radix-ui/react-context-menu"
import { Check, ChevronRight, Circle } from "lucide-react"

import { cn } from "@/lib/utils"

const ContextMenu = ContextMenuPrimitive.Root

const ContextMenuTrigger = ContextMenuPrimitive.Trigger

const ContextMenuGroup = ContextMenuPrimitive.Group

const ContextMenuPortal = ContextMenuPrimitive.Portal

const ContextMenuSub = ContextMenuPrimitive.Sub

const ContextMenuRadioGroup = ContextMenuPrimitive.RadioGroup

const ContextMenuSubTrigger = React.forwardRef(({ className, inset, children, ...props }, ref) => (
  <ContextMenuPrimitive.SubTrigger
    ref={ref}
    className={cn(
      "flex cursor-default select-none items-center rounded-sm px-2 py-1.5 text-sm outline-none focus:bg-accent focus:text-accent-foreground data-[state=open]:bg-accent data-[state=open]:text-accent-foreground",
      inset && "pl-8",
      className
    )}
    {...props}>
    {children}
    <ChevronRight className="ml-auto h-4 w-4" />
  </ContextMenuPrimitive.SubTrigger>
))
ContextMenuSubTrigger.displayName = ContextMenuPrimitive.SubTrigger.displayName

const ContextMenuSubContent = React.forwardRef(({ className, ...props }, ref) => (
  <ContextMenuPrimitive.SubContent
    ref={ref}
    className={cn(
      "z-50 min-w-[8rem] overflow-hidden rounded-md border bg-popover p-1 text-popover-foreground shadow-lg data-[state=open]:animate-in data-[state=closed]:animate-out data-[state=closed]:fade-out-0 data-[state=open]:fade-in-0 data-[state=closed]:zoom-out-95 data-[state=open]:zoom-in-95 data-[side=bottom]:slide-in-from-top-2 data-[side=left]:slide-in-from-right-2 data-[side=right]:slide-in-from-left-2 data-[side=top]:slide-in-from-bottom-2",
      className
    )}
    {...props} />
))
ContextMenuSubContent.displayName = ContextMenuPrimitive.SubContent.displayName

const ContextMenuContent = React.forwardRef(({ className, ...props }, ref) => (
  <ContextMenuPrimitive.Portal>
    <ContextMenuPrimitive.Content
      ref={ref}
      className={cn(
        "z-50 min-w-[8rem] overflow-hidden rounded-md border bg-popover p-1 text-popover-foreground shadow-md data-[state=open]:animate-in data-[state=closed]:animate-out data-[state=closed]:fade-out-0 data-[state=open]:fade-in-0 data-[state=closed]:zoom-out-95 data-[state=open]:zoom-in-95 data-[side=bottom]:slide-in-from-top-2 data-[side=left]:slide-in-from-right-2 data-[side=right]:slide-in-from-left-2 data-[side=top]:slide-in-from-bottom-2",
        className
      )}
      {...props} />
  </ContextMenuPrimitive.Portal>
))
ContextMenuContent.displayName = ContextMenuPrimitive.Content.displayName

const ContextMenuItem = React.forwardRef(({ className, inset, ...props }, ref) => (
  <ContextMenuPrimitive.Item
    ref={ref}
    className={cn(
      "relative flex cursor-default select-none items-center rounded-sm px-2 py-1.5 text-sm outline-none focus:bg-accent focus:text-accent-foreground data-[disabled]:pointer-events-none data-[disabled]:opacity-50",
      inset && "pl-8",
      className
    )}
    {...props} />
))
ContextMenuItem.displayName = ContextMenuPrimitive.Item.displayName

const ContextMenuCheckboxItem = React.forwardRef(({ className, children, checked, ...props }, ref) => (
  <ContextMenuPrimitive.CheckboxItem
    ref={ref}
    className={cn(
      "relative flex cursor-default select-none items-center rounded-sm py-1.5 pl-8 pr-2 text-sm outline-none focus:bg-accent focus:text-accent-foreground data-[disabled]:pointer-events-none data-[disabled]:opacity-50",
      className
    )}
    checked={checked}
    {...props}>
    <span className="absolute left-2 flex h-3.5 w-3.5 items-center justify-center">
      <ContextMenuPrimitive.ItemIndicator>
        <Check className="h-4 w-4" />
      </ContextMenuPrimitive.ItemIndicator>
    </span>
    {children}
  </ContextMenuPrimitive.CheckboxItem>
))
ContextMenuCheckboxItem.displayName =
  ContextMenuPrimitive.CheckboxItem.displayName

const ContextMenuRadioItem = React.forwardRef(({ className, children, ...props }, ref) => (
  <ContextMenuPrimitive.RadioItem
    ref={ref}
    className={cn(
      "relative flex cursor-default select-none items-center rounded-sm py-1.5 pl-8 pr-2 text-sm outline-none focus:bg-accent focus:text-accent-foreground data-[disabled]:pointer-events-none data-[disabled]:opacity-50",
      className
    )}
    {...props}>
    <span className="absolute left-2 flex h-3.5 w-3.5 items-center justify-center">
      <ContextMenuPrimitive.ItemIndicator>
        <Circle className="h-4 w-4 fill-current" />
      </ContextMenuPrimitive.ItemIndicator>
    </span>
    {children}
  </ContextMenuPrimitive.RadioItem>
))
ContextMenuRadioItem.displayName = ContextMenuPrimitive.RadioItem.displayName

const ContextMenuLabel = React.forwardRef(({ className, inset, ...props }, ref) => (
  <ContextMenuPrimitive.Label
    ref={ref}
    className={cn(
      "px-2 py-1.5 text-sm font-semibold text-foreground",
      inset && "pl-8",
      className
    )}
    {...props} />
))
ContextMenuLabel.displayName = ContextMenuPrimitive.Label.displayName

const ContextMenuSeparator = React.forwardRef(({ className, ...props }, ref) => (
  <ContextMenuPrimitive.Separator
    ref={ref}
    className={cn("-mx-1 my-1 h-px bg-border", className)}
    {...props} />
))
ContextMenuSeparator.displayName = ContextMenuPrimitive.Separator.displayName

const ContextMenuShortcut = ({
  className,
  ...props
}) => {
  return (
    (<span
      className={cn("ml-auto text-xs tracking-widest text-muted-foreground", className)}
      {...props} />)
  );
}
ContextMenuShortcut.displayName = "ContextMenuShortcut"

export {
  ContextMenu,
  ContextMenuTrigger,
  ContextMenuContent,
  ContextMenuItem,
  ContextMenuCheckboxItem,
  ContextMenuRadioItem,
  ContextMenuLabel,
  ContextMenuSeparator,
  ContextMenuShortcut,
  ContextMenuGroup,
  ContextMenuPortal,
  ContextMenuSub,
  ContextMenuSubContent,
  ContextMenuSubTrigger,
  ContextMenuRadioGroup,
}

```

---

## File: `src/components/ui/table.jsx`

```text
import * as React from "react"

import { cn } from "@/lib/utils"

const Table = React.forwardRef(({ className, ...props }, ref) => (
  <div className="relative w-full overflow-auto">
    <table
      ref={ref}
      className={cn("w-full caption-bottom text-sm", className)}
      {...props} />
  </div>
))
Table.displayName = "Table"

const TableHeader = React.forwardRef(({ className, ...props }, ref) => (
  <thead ref={ref} className={cn("[&_tr]:border-b", className)} {...props} />
))
TableHeader.displayName = "TableHeader"

const TableBody = React.forwardRef(({ className, ...props }, ref) => (
  <tbody
    ref={ref}
    className={cn("[&_tr:last-child]:border-0", className)}
    {...props} />
))
TableBody.displayName = "TableBody"

const TableFooter = React.forwardRef(({ className, ...props }, ref) => (
  <tfoot
    ref={ref}
    className={cn("border-t bg-muted/50 font-medium [&>tr]:last:border-b-0", className)}
    {...props} />
))
TableFooter.displayName = "TableFooter"

const TableRow = React.forwardRef(({ className, ...props }, ref) => (
  <tr
    ref={ref}
    className={cn(
      "border-b transition-colors hover:bg-muted/50 data-[state=selected]:bg-muted",
      className
    )}
    {...props} />
))
TableRow.displayName = "TableRow"

const TableHead = React.forwardRef(({ className, ...props }, ref) => (
  <th
    ref={ref}
    className={cn(
      "h-10 px-2 text-left align-middle font-medium text-muted-foreground [&:has([role=checkbox])]:pr-0 [&>[role=checkbox]]:translate-y-[2px]",
      className
    )}
    {...props} />
))
TableHead.displayName = "TableHead"

const TableCell = React.forwardRef(({ className, ...props }, ref) => (
  <td
    ref={ref}
    className={cn(
      "p-2 align-middle [&:has([role=checkbox])]:pr-0 [&>[role=checkbox]]:translate-y-[2px]",
      className
    )}
    {...props} />
))
TableCell.displayName = "TableCell"

const TableCaption = React.forwardRef(({ className, ...props }, ref) => (
  <caption
    ref={ref}
    className={cn("mt-4 text-sm text-muted-foreground", className)}
    {...props} />
))
TableCaption.displayName = "TableCaption"

export {
  Table,
  TableHeader,
  TableBody,
  TableFooter,
  TableHead,
  TableRow,
  TableCell,
  TableCaption,
}

```

---

## File: `src/components/ui/textarea.jsx`

```text
import * as React from "react"

import { cn } from "@/lib/utils"

const Textarea = React.forwardRef(({ className, ...props }, ref) => {
  return (
    (<textarea
      className={cn(
        "flex min-h-[60px] w-full rounded-md border border-input bg-transparent px-3 py-2 text-base shadow-sm placeholder:text-muted-foreground focus-visible:outline-none focus-visible:ring-1 focus-visible:ring-ring disabled:cursor-not-allowed disabled:opacity-50 md:text-sm",
        className
      )}
      ref={ref}
      {...props} />)
  );
})
Textarea.displayName = "Textarea"

export { Textarea }

```

---

## File: `src/components/ui/progress.jsx`

```text
"use client"

import * as React from "react"
import * as ProgressPrimitive from "@radix-ui/react-progress"

import { cn } from "@/lib/utils"

const Progress = React.forwardRef(({ className, value, ...props }, ref) => (
  <ProgressPrimitive.Root
    ref={ref}
    className={cn(
      "relative h-2 w-full overflow-hidden rounded-full bg-primary/20",
      className
    )}
    {...props}>
    <ProgressPrimitive.Indicator
      className="h-full w-full flex-1 bg-primary transition-all"
      style={{ transform: `translateX(-${100 - (value || 0)}%)` }} />
  </ProgressPrimitive.Root>
))
Progress.displayName = ProgressPrimitive.Root.displayName

export { Progress }

```

---

## File: `src/components/ui/drawer.jsx`

```text
"use client"

import * as React from "react"
import { Drawer as DrawerPrimitive } from "vaul"

import { cn } from "@/lib/utils"

const Drawer = ({
  shouldScaleBackground = true,
  ...props
}) => (
  <DrawerPrimitive.Root shouldScaleBackground={shouldScaleBackground} {...props} />
)
Drawer.displayName = "Drawer"

const DrawerTrigger = DrawerPrimitive.Trigger

const DrawerPortal = DrawerPrimitive.Portal

const DrawerClose = DrawerPrimitive.Close

const DrawerOverlay = React.forwardRef(({ className, ...props }, ref) => (
  <DrawerPrimitive.Overlay
    ref={ref}
    className={cn("fixed inset-0 z-50 bg-black/80", className)}
    {...props} />
))
DrawerOverlay.displayName = DrawerPrimitive.Overlay.displayName

const DrawerContent = React.forwardRef(({ className, children, ...props }, ref) => (
  <DrawerPortal>
    <DrawerOverlay />
    <DrawerPrimitive.Content
      ref={ref}
      className={cn(
        "fixed inset-x-0 bottom-0 z-50 mt-24 flex h-auto flex-col rounded-t-[10px] border bg-background",
        className
      )}
      {...props}>
      <div className="mx-auto mt-4 h-2 w-[100px] rounded-full bg-muted" />
      {children}
    </DrawerPrimitive.Content>
  </DrawerPortal>
))
DrawerContent.displayName = "DrawerContent"

const DrawerHeader = ({
  className,
  ...props
}) => (
  <div
    className={cn("grid gap-1.5 p-4 text-center sm:text-left", className)}
    {...props} />
)
DrawerHeader.displayName = "DrawerHeader"

const DrawerFooter = ({
  className,
  ...props
}) => (
  <div className={cn("mt-auto flex flex-col gap-2 p-4", className)} {...props} />
)
DrawerFooter.displayName = "DrawerFooter"

const DrawerTitle = React.forwardRef(({ className, ...props }, ref) => (
  <DrawerPrimitive.Title
    ref={ref}
    className={cn("text-lg font-semibold leading-none tracking-tight", className)}
    {...props} />
))
DrawerTitle.displayName = DrawerPrimitive.Title.displayName

const DrawerDescription = React.forwardRef(({ className, ...props }, ref) => (
  <DrawerPrimitive.Description
    ref={ref}
    className={cn("text-sm text-muted-foreground", className)}
    {...props} />
))
DrawerDescription.displayName = DrawerPrimitive.Description.displayName

export {
  Drawer,
  DrawerPortal,
  DrawerOverlay,
  DrawerTrigger,
  DrawerClose,
  DrawerContent,
  DrawerHeader,
  DrawerFooter,
  DrawerTitle,
  DrawerDescription,
}

```

---

## File: `src/components/ui/toast.jsx`

```text
import * as React from "react";
import { cva } from "class-variance-authority";
import { X } from "lucide-react";
import { cn } from "@/lib/utils";

const ToastProvider = React.forwardRef(({ ...props }, ref) => (
  <div
    ref={ref}
    className="fixed top-0 z-[100] flex max-h-screen w-full flex-col-reverse p-4 sm:bottom-0 sm:right-0 sm:top-auto sm:flex-col md:max-w-[420px]"
    {...props}
  />
));
ToastProvider.displayName = "ToastProvider";

const ToastViewport = React.forwardRef(({ ...props }, ref) => (
  <div
    ref={ref}
    className="fixed top-0 z-[100] flex max-h-screen w-full flex-col-reverse p-4 sm:bottom-0 sm:right-0 sm:top-auto sm:flex-col md:max-w-[420px]"
    {...props}
  />
));
ToastViewport.displayName = "ToastViewport";

const toastVariants = cva(
  "group pointer-events-auto relative flex w-full items-center justify-between space-x-4 overflow-hidden rounded-md border p-6 pr-8 shadow-lg transition-all data-[swipe=cancel]:translate-x-0 data-[swipe=end]:translate-x-[var(--radix-toast-swipe-end-x)] data-[swipe=move]:translate-x-[var(--radix-toast-swipe-move-x)] data-[swipe=move]:transition-none data-[state=open]:animate-in data-[state=closed]:animate-out data-[swipe=end]:animate-out data-[state=closed]:fade-out-80 data-[state=closed]:slide-out-to-right-full data-[state=open]:slide-in-from-top-full data-[state=open]:sm:slide-in-from-bottom-full",
  {
    variants: {
      variant: {
        default: "border bg-background text-foreground",
        destructive:
          "destructive group border-destructive bg-destructive text-destructive-foreground",
      },
    },
    defaultVariants: {
      variant: "default",
    },
  }
);

const Toast = React.forwardRef(({ className, variant, ...props }, ref) => {
  return (
    <div
      ref={ref}
      className={cn(toastVariants({ variant }), className)}
      {...props}
    />
  );
});
Toast.displayName = "Toast";

const ToastAction = React.forwardRef(({ className, ...props }, ref) => (
  <div
    ref={ref}
    className={cn(
      "inline-flex h-8 shrink-0 items-center justify-center rounded-md border bg-transparent px-3 text-sm font-medium ring-offset-background transition-colors hover:bg-secondary focus:outline-none focus:ring-2 focus:ring-ring focus:ring-offset-2 disabled:pointer-events-none disabled:opacity-50 group-[.destructive]:border-muted/40 group-[.destructive]:hover:border-destructive/30 group-[.destructive]:hover:bg-destructive group-[.destructive]:hover:text-destructive-foreground group-[.destructive]:focus:ring-destructive",
      className
    )}
    {...props}
  />
));
ToastAction.displayName = "ToastAction";

const ToastClose = React.forwardRef(({ className, ...props }, ref) => (
  <button
    ref={ref}
    className={cn(
      "absolute right-2 top-2 rounded-md p-1 text-foreground/50 opacity-0 transition-opacity hover:text-foreground focus:opacity-100 focus:outline-none focus:ring-2 group-hover:opacity-100 group-[.destructive]:text-red-300 group-[.destructive]:hover:text-red-50 group-[.destructive]:focus:ring-red-400 group-[.destructive]:focus:ring-offset-red-600",
      className
    )}
    toast-close=""
    {...props}
  >
    <X className="h-4 w-4" />
  </button>
));
ToastClose.displayName = "ToastClose";

const ToastTitle = React.forwardRef(({ className, ...props }, ref) => (
  <div
    ref={ref}
    className={cn("text-sm font-semibold", className)}
    {...props}
  />
));
ToastTitle.displayName = "ToastTitle";

const ToastDescription = React.forwardRef(({ className, ...props }, ref) => (
  <div
    ref={ref}
    className={cn("text-sm opacity-90", className)}
    {...props}
  />
));
ToastDescription.displayName = "ToastDescription";

export {
  ToastProvider,
  ToastViewport,
  Toast,
  ToastTitle,
  ToastDescription,
  ToastClose,
  ToastAction,
}; 
```

---

## File: `src/components/ui/toggle-group.jsx`

```text
"use client";
import * as React from "react"
import * as ToggleGroupPrimitive from "@radix-ui/react-toggle-group"

import { cn } from "@/lib/utils"
import { toggleVariants } from "@/components/ui/toggle"

const ToggleGroupContext = React.createContext({
  size: "default",
  variant: "default",
})

const ToggleGroup = React.forwardRef(({ className, variant, size, children, ...props }, ref) => (
  <ToggleGroupPrimitive.Root
    ref={ref}
    className={cn("flex items-center justify-center gap-1", className)}
    {...props}>
    <ToggleGroupContext.Provider value={{ variant, size }}>
      {children}
    </ToggleGroupContext.Provider>
  </ToggleGroupPrimitive.Root>
))

ToggleGroup.displayName = ToggleGroupPrimitive.Root.displayName

const ToggleGroupItem = React.forwardRef(({ className, children, variant, size, ...props }, ref) => {
  const context = React.useContext(ToggleGroupContext)

  return (
    (<ToggleGroupPrimitive.Item
      ref={ref}
      className={cn(toggleVariants({
        variant: context.variant || variant,
        size: context.size || size,
      }), className)}
      {...props}>
      {children}
    </ToggleGroupPrimitive.Item>)
  );
})

ToggleGroupItem.displayName = ToggleGroupPrimitive.Item.displayName

export { ToggleGroup, ToggleGroupItem }

```

---

## File: `src/components/ui/tabs.jsx`

```text
import * as React from "react"
import * as TabsPrimitive from "@radix-ui/react-tabs"

import { cn } from "@/lib/utils"

const Tabs = TabsPrimitive.Root

const TabsList = React.forwardRef(({ className, ...props }, ref) => (
  <TabsPrimitive.List
    ref={ref}
    className={cn(
      "inline-flex h-9 items-center justify-center rounded-lg bg-muted p-1 text-muted-foreground",
      className
    )}
    {...props} />
))
TabsList.displayName = TabsPrimitive.List.displayName

const TabsTrigger = React.forwardRef(({ className, ...props }, ref) => (
  <TabsPrimitive.Trigger
    ref={ref}
    className={cn(
      "inline-flex items-center justify-center whitespace-nowrap rounded-md px-3 py-1 text-sm font-medium ring-offset-background transition-all focus-visible:outline-none focus-visible:ring-2 focus-visible:ring-ring focus-visible:ring-offset-2 disabled:pointer-events-none disabled:opacity-50 data-[state=active]:bg-background data-[state=active]:text-foreground data-[state=active]:shadow",
      className
    )}
    {...props} />
))
TabsTrigger.displayName = TabsPrimitive.Trigger.displayName

const TabsContent = React.forwardRef(({ className, ...props }, ref) => (
  <TabsPrimitive.Content
    ref={ref}
    className={cn(
      "mt-2 ring-offset-background focus-visible:outline-none focus-visible:ring-2 focus-visible:ring-ring focus-visible:ring-offset-2",
      className
    )}
    {...props} />
))
TabsContent.displayName = TabsPrimitive.Content.displayName

export { Tabs, TabsList, TabsTrigger, TabsContent }

```

---

## File: `src/components/ui/accordion.jsx`

```text
import * as React from "react"
import * as AccordionPrimitive from "@radix-ui/react-accordion"
import { ChevronDown } from "lucide-react"

import { cn } from "@/lib/utils"

const Accordion = AccordionPrimitive.Root

const AccordionItem = React.forwardRef(({ className, ...props }, ref) => (
  <AccordionPrimitive.Item ref={ref} className={cn("border-b", className)} {...props} />
))
AccordionItem.displayName = "AccordionItem"

const AccordionTrigger = React.forwardRef(({ className, children, ...props }, ref) => (
  <AccordionPrimitive.Header className="flex">
    <AccordionPrimitive.Trigger
      ref={ref}
      className={cn(
        "flex flex-1 items-center justify-between py-4 text-sm font-medium transition-all hover:underline text-left [&[data-state=open]>svg]:rotate-180",
        className
      )}
      {...props}>
      {children}
      <ChevronDown
        className="h-4 w-4 shrink-0 text-muted-foreground transition-transform duration-200" />
    </AccordionPrimitive.Trigger>
  </AccordionPrimitive.Header>
))
AccordionTrigger.displayName = AccordionPrimitive.Trigger.displayName

const AccordionContent = React.forwardRef(({ className, children, ...props }, ref) => (
  <AccordionPrimitive.Content
    ref={ref}
    className="overflow-hidden text-sm data-[state=closed]:animate-accordion-up data-[state=open]:animate-accordion-down"
    {...props}>
    <div className={cn("pb-4 pt-0", className)}>{children}</div>
  </AccordionPrimitive.Content>
))
AccordionContent.displayName = AccordionPrimitive.Content.displayName

export { Accordion, AccordionItem, AccordionTrigger, AccordionContent }

```

---

## File: `src/components/ui/aspect-ratio.jsx`

```text
import * as AspectRatioPrimitive from "@radix-ui/react-aspect-ratio"

const AspectRatio = AspectRatioPrimitive.Root

export { AspectRatio }

```

---

## File: `src/components/ui/navigation-menu.jsx`

```text
import * as React from "react"
import * as NavigationMenuPrimitive from "@radix-ui/react-navigation-menu"
import { cva } from "class-variance-authority"
import { ChevronDown } from "lucide-react"

import { cn } from "@/lib/utils"

const NavigationMenu = React.forwardRef(({ className, children, ...props }, ref) => (
  <NavigationMenuPrimitive.Root
    ref={ref}
    className={cn(
      "relative z-10 flex max-w-max flex-1 items-center justify-center",
      className
    )}
    {...props}>
    {children}
    <NavigationMenuViewport />
  </NavigationMenuPrimitive.Root>
))
NavigationMenu.displayName = NavigationMenuPrimitive.Root.displayName

const NavigationMenuList = React.forwardRef(({ className, ...props }, ref) => (
  <NavigationMenuPrimitive.List
    ref={ref}
    className={cn(
      "group flex flex-1 list-none items-center justify-center space-x-1",
      className
    )}
    {...props} />
))
NavigationMenuList.displayName = NavigationMenuPrimitive.List.displayName

const NavigationMenuItem = NavigationMenuPrimitive.Item

const navigationMenuTriggerStyle = cva(
  "group inline-flex h-9 w-max items-center justify-center rounded-md bg-background px-4 py-2 text-sm font-medium transition-colors hover:bg-accent hover:text-accent-foreground focus:bg-accent focus:text-accent-foreground focus:outline-none disabled:pointer-events-none disabled:opacity-50 data-[active]:bg-accent/50 data-[state=open]:bg-accent/50"
)

const NavigationMenuTrigger = React.forwardRef(({ className, children, ...props }, ref) => (
  <NavigationMenuPrimitive.Trigger
    ref={ref}
    className={cn(navigationMenuTriggerStyle(), "group", className)}
    {...props}>
    {children}{" "}
    <ChevronDown
      className="relative top-[1px] ml-1 h-3 w-3 transition duration-300 group-data-[state=open]:rotate-180"
      aria-hidden="true" />
  </NavigationMenuPrimitive.Trigger>
))
NavigationMenuTrigger.displayName = NavigationMenuPrimitive.Trigger.displayName

const NavigationMenuContent = React.forwardRef(({ className, ...props }, ref) => (
  <NavigationMenuPrimitive.Content
    ref={ref}
    className={cn(
      "left-0 top-0 w-full data-[motion^=from-]:animate-in data-[motion^=to-]:animate-out data-[motion^=from-]:fade-in data-[motion^=to-]:fade-out data-[motion=from-end]:slide-in-from-right-52 data-[motion=from-start]:slide-in-from-left-52 data-[motion=to-end]:slide-out-to-right-52 data-[motion=to-start]:slide-out-to-left-52 md:absolute md:w-auto ",
      className
    )}
    {...props} />
))
NavigationMenuContent.displayName = NavigationMenuPrimitive.Content.displayName

const NavigationMenuLink = NavigationMenuPrimitive.Link

const NavigationMenuViewport = React.forwardRef(({ className, ...props }, ref) => (
  <div className={cn("absolute left-0 top-full flex justify-center")}>
    <NavigationMenuPrimitive.Viewport
      className={cn(
        "origin-top-center relative mt-1.5 h-[var(--radix-navigation-menu-viewport-height)] w-full overflow-hidden rounded-md border bg-popover text-popover-foreground shadow data-[state=open]:animate-in data-[state=closed]:animate-out data-[state=closed]:zoom-out-95 data-[state=open]:zoom-in-90 md:w-[var(--radix-navigation-menu-viewport-width)]",
        className
      )}
      ref={ref}
      {...props} />
  </div>
))
NavigationMenuViewport.displayName =
  NavigationMenuPrimitive.Viewport.displayName

const NavigationMenuIndicator = React.forwardRef(({ className, ...props }, ref) => (
  <NavigationMenuPrimitive.Indicator
    ref={ref}
    className={cn(
      "top-full z-[1] flex h-1.5 items-end justify-center overflow-hidden data-[state=visible]:animate-in data-[state=hidden]:animate-out data-[state=hidden]:fade-out data-[state=visible]:fade-in",
      className
    )}
    {...props}>
    <div
      className="relative top-[60%] h-2 w-2 rotate-45 rounded-tl-sm bg-border shadow-md" />
  </NavigationMenuPrimitive.Indicator>
))
NavigationMenuIndicator.displayName =
  NavigationMenuPrimitive.Indicator.displayName

export {
  navigationMenuTriggerStyle,
  NavigationMenu,
  NavigationMenuList,
  NavigationMenuItem,
  NavigationMenuContent,
  NavigationMenuTrigger,
  NavigationMenuLink,
  NavigationMenuIndicator,
  NavigationMenuViewport,
}

```

---

## File: `src/components/ui/popover.jsx`

```text
import * as React from "react"
import * as PopoverPrimitive from "@radix-ui/react-popover"

import { cn } from "@/lib/utils"

const Popover = PopoverPrimitive.Root

const PopoverTrigger = PopoverPrimitive.Trigger

const PopoverAnchor = PopoverPrimitive.Anchor

const PopoverContent = React.forwardRef(({ className, align = "center", sideOffset = 4, ...props }, ref) => (
  <PopoverPrimitive.Portal>
    <PopoverPrimitive.Content
      ref={ref}
      align={align}
      sideOffset={sideOffset}
      className={cn(
        "z-50 w-72 rounded-md border bg-popover p-4 text-popover-foreground shadow-md outline-none data-[state=open]:animate-in data-[state=closed]:animate-out data-[state=closed]:fade-out-0 data-[state=open]:fade-in-0 data-[state=closed]:zoom-out-95 data-[state=open]:zoom-in-95 data-[side=bottom]:slide-in-from-top-2 data-[side=left]:slide-in-from-right-2 data-[side=right]:slide-in-from-left-2 data-[side=top]:slide-in-from-bottom-2",
        className
      )}
      {...props} />
  </PopoverPrimitive.Portal>
))
PopoverContent.displayName = PopoverPrimitive.Content.displayName

export { Popover, PopoverTrigger, PopoverContent, PopoverAnchor }

```

---

## File: `src/components/ui/toggle.jsx`

```text
import * as React from "react"
import * as TogglePrimitive from "@radix-ui/react-toggle"
import { cva } from "class-variance-authority";

import { cn } from "@/lib/utils"

const toggleVariants = cva(
  "inline-flex items-center justify-center gap-2 rounded-md text-sm font-medium transition-colors hover:bg-muted hover:text-muted-foreground focus-visible:outline-none focus-visible:ring-1 focus-visible:ring-ring disabled:pointer-events-none disabled:opacity-50 data-[state=on]:bg-accent data-[state=on]:text-accent-foreground [&_svg]:pointer-events-none [&_svg]:size-4 [&_svg]:shrink-0",
  {
    variants: {
      variant: {
        default: "bg-transparent",
        outline:
          "border border-input bg-transparent shadow-sm hover:bg-accent hover:text-accent-foreground",
      },
      size: {
        default: "h-9 px-2 min-w-9",
        sm: "h-8 px-1.5 min-w-8",
        lg: "h-10 px-2.5 min-w-10",
      },
    },
    defaultVariants: {
      variant: "default",
      size: "default",
    },
  }
)

const Toggle = React.forwardRef(({ className, variant, size, ...props }, ref) => (
  <TogglePrimitive.Root
    ref={ref}
    className={cn(toggleVariants({ variant, size, className }))}
    {...props} />
))

Toggle.displayName = TogglePrimitive.Root.displayName

export { Toggle, toggleVariants }

```

---

## File: `src/components/ui/radio-group.jsx`

```text
import * as React from "react"
import * as RadioGroupPrimitive from "@radix-ui/react-radio-group"
import { Circle } from "lucide-react"

import { cn } from "@/lib/utils"

const RadioGroup = React.forwardRef(({ className, ...props }, ref) => {
  return (<RadioGroupPrimitive.Root className={cn("grid gap-2", className)} {...props} ref={ref} />);
})
RadioGroup.displayName = RadioGroupPrimitive.Root.displayName

const RadioGroupItem = React.forwardRef(({ className, ...props }, ref) => {
  return (
    (<RadioGroupPrimitive.Item
      ref={ref}
      className={cn(
        "aspect-square h-4 w-4 rounded-full border border-primary text-primary shadow focus:outline-none focus-visible:ring-1 focus-visible:ring-ring disabled:cursor-not-allowed disabled:opacity-50",
        className
      )}
      {...props}>
      <RadioGroupPrimitive.Indicator className="flex items-center justify-center">
        <Circle className="h-3.5 w-3.5 fill-primary" />
      </RadioGroupPrimitive.Indicator>
    </RadioGroupPrimitive.Item>)
  );
})
RadioGroupItem.displayName = RadioGroupPrimitive.Item.displayName

export { RadioGroup, RadioGroupItem }

```

---

## File: `src/components/ui/dropdown-menu.jsx`

```text
import * as React from "react"
import * as DropdownMenuPrimitive from "@radix-ui/react-dropdown-menu"
import { Check, ChevronRight, Circle } from "lucide-react"

import { cn } from "@/lib/utils"

const DropdownMenu = DropdownMenuPrimitive.Root

const DropdownMenuTrigger = DropdownMenuPrimitive.Trigger

const DropdownMenuGroup = DropdownMenuPrimitive.Group

const DropdownMenuPortal = DropdownMenuPrimitive.Portal

const DropdownMenuSub = DropdownMenuPrimitive.Sub

const DropdownMenuRadioGroup = DropdownMenuPrimitive.RadioGroup

const DropdownMenuSubTrigger = React.forwardRef(({ className, inset, children, ...props }, ref) => (
  <DropdownMenuPrimitive.SubTrigger
    ref={ref}
    className={cn(
      "flex cursor-default gap-2 select-none items-center rounded-sm px-2 py-1.5 text-sm outline-none focus:bg-accent data-[state=open]:bg-accent [&_svg]:pointer-events-none [&_svg]:size-4 [&_svg]:shrink-0",
      inset && "pl-8",
      className
    )}
    {...props}>
    {children}
    <ChevronRight className="ml-auto" />
  </DropdownMenuPrimitive.SubTrigger>
))
DropdownMenuSubTrigger.displayName =
  DropdownMenuPrimitive.SubTrigger.displayName

const DropdownMenuSubContent = React.forwardRef(({ className, ...props }, ref) => (
  <DropdownMenuPrimitive.SubContent
    ref={ref}
    className={cn(
      "z-50 min-w-[8rem] overflow-hidden rounded-md border bg-popover p-1 text-popover-foreground shadow-lg data-[state=open]:animate-in data-[state=closed]:animate-out data-[state=closed]:fade-out-0 data-[state=open]:fade-in-0 data-[state=closed]:zoom-out-95 data-[state=open]:zoom-in-95 data-[side=bottom]:slide-in-from-top-2 data-[side=left]:slide-in-from-right-2 data-[side=right]:slide-in-from-left-2 data-[side=top]:slide-in-from-bottom-2",
      className
    )}
    {...props} />
))
DropdownMenuSubContent.displayName =
  DropdownMenuPrimitive.SubContent.displayName

const DropdownMenuContent = React.forwardRef(({ className, sideOffset = 4, ...props }, ref) => (
  <DropdownMenuPrimitive.Portal>
    <DropdownMenuPrimitive.Content
      ref={ref}
      sideOffset={sideOffset}
      className={cn(
        "z-50 min-w-[8rem] overflow-hidden rounded-md border bg-popover p-1 text-popover-foreground shadow-md",
        "data-[state=open]:animate-in data-[state=closed]:animate-out data-[state=closed]:fade-out-0 data-[state=open]:fade-in-0 data-[state=closed]:zoom-out-95 data-[state=open]:zoom-in-95 data-[side=bottom]:slide-in-from-top-2 data-[side=left]:slide-in-from-right-2 data-[side=right]:slide-in-from-left-2 data-[side=top]:slide-in-from-bottom-2",
        className
      )}
      {...props} />
  </DropdownMenuPrimitive.Portal>
))
DropdownMenuContent.displayName = DropdownMenuPrimitive.Content.displayName

const DropdownMenuItem = React.forwardRef(({ className, inset, ...props }, ref) => (
  <DropdownMenuPrimitive.Item
    ref={ref}
    className={cn(
      "relative flex cursor-default select-none items-center gap-2 rounded-sm px-2 py-1.5 text-sm outline-none transition-colors focus:bg-accent focus:text-accent-foreground data-[disabled]:pointer-events-none data-[disabled]:opacity-50 [&>svg]:size-4 [&>svg]:shrink-0",
      inset && "pl-8",
      className
    )}
    {...props} />
))
DropdownMenuItem.displayName = DropdownMenuPrimitive.Item.displayName

const DropdownMenuCheckboxItem = React.forwardRef(({ className, children, checked, ...props }, ref) => (
  <DropdownMenuPrimitive.CheckboxItem
    ref={ref}
    className={cn(
      "relative flex cursor-default select-none items-center rounded-sm py-1.5 pl-8 pr-2 text-sm outline-none transition-colors focus:bg-accent focus:text-accent-foreground data-[disabled]:pointer-events-none data-[disabled]:opacity-50",
      className
    )}
    checked={checked}
    {...props}>
    <span className="absolute left-2 flex h-3.5 w-3.5 items-center justify-center">
      <DropdownMenuPrimitive.ItemIndicator>
        <Check className="h-4 w-4" />
      </DropdownMenuPrimitive.ItemIndicator>
    </span>
    {children}
  </DropdownMenuPrimitive.CheckboxItem>
))
DropdownMenuCheckboxItem.displayName =
  DropdownMenuPrimitive.CheckboxItem.displayName

const DropdownMenuRadioItem = React.forwardRef(({ className, children, ...props }, ref) => (
  <DropdownMenuPrimitive.RadioItem
    ref={ref}
    className={cn(
      "relative flex cursor-default select-none items-center rounded-sm py-1.5 pl-8 pr-2 text-sm outline-none transition-colors focus:bg-accent focus:text-accent-foreground data-[disabled]:pointer-events-none data-[disabled]:opacity-50",
      className
    )}
    {...props}>
    <span className="absolute left-2 flex h-3.5 w-3.5 items-center justify-center">
      <DropdownMenuPrimitive.ItemIndicator>
        <Circle className="h-2 w-2 fill-current" />
      </DropdownMenuPrimitive.ItemIndicator>
    </span>
    {children}
  </DropdownMenuPrimitive.RadioItem>
))
DropdownMenuRadioItem.displayName = DropdownMenuPrimitive.RadioItem.displayName

const DropdownMenuLabel = React.forwardRef(({ className, inset, ...props }, ref) => (
  <DropdownMenuPrimitive.Label
    ref={ref}
    className={cn("px-2 py-1.5 text-sm font-semibold", inset && "pl-8", className)}
    {...props} />
))
DropdownMenuLabel.displayName = DropdownMenuPrimitive.Label.displayName

const DropdownMenuSeparator = React.forwardRef(({ className, ...props }, ref) => (
  <DropdownMenuPrimitive.Separator
    ref={ref}
    className={cn("-mx-1 my-1 h-px bg-muted", className)}
    {...props} />
))
DropdownMenuSeparator.displayName = DropdownMenuPrimitive.Separator.displayName

const DropdownMenuShortcut = ({
  className,
  ...props
}) => {
  return (
    (<span
      className={cn("ml-auto text-xs tracking-widest opacity-60", className)}
      {...props} />)
  );
}
DropdownMenuShortcut.displayName = "DropdownMenuShortcut"

export {
  DropdownMenu,
  DropdownMenuTrigger,
  DropdownMenuContent,
  DropdownMenuItem,
  DropdownMenuCheckboxItem,
  DropdownMenuRadioItem,
  DropdownMenuLabel,
  DropdownMenuSeparator,
  DropdownMenuShortcut,
  DropdownMenuGroup,
  DropdownMenuPortal,
  DropdownMenuSub,
  DropdownMenuSubContent,
  DropdownMenuSubTrigger,
  DropdownMenuRadioGroup,
}

```

---

## File: `src/components/ui/hover-card.jsx`

```text
"use client"

import * as React from "react"
import * as HoverCardPrimitive from "@radix-ui/react-hover-card"

import { cn } from "@/lib/utils"

const HoverCard = HoverCardPrimitive.Root

const HoverCardTrigger = HoverCardPrimitive.Trigger

const HoverCardContent = React.forwardRef(({ className, align = "center", sideOffset = 4, ...props }, ref) => (
  <HoverCardPrimitive.Content
    ref={ref}
    align={align}
    sideOffset={sideOffset}
    className={cn(
      "z-50 w-64 rounded-md border bg-popover p-4 text-popover-foreground shadow-md outline-none data-[state=open]:animate-in data-[state=closed]:animate-out data-[state=closed]:fade-out-0 data-[state=open]:fade-in-0 data-[state=closed]:zoom-out-95 data-[state=open]:zoom-in-95 data-[side=bottom]:slide-in-from-top-2 data-[side=left]:slide-in-from-right-2 data-[side=right]:slide-in-from-left-2 data-[side=top]:slide-in-from-bottom-2",
      className
    )}
    {...props} />
))
HoverCardContent.displayName = HoverCardPrimitive.Content.displayName

export { HoverCard, HoverCardTrigger, HoverCardContent }

```

---

## File: `src/components/ui/switch.jsx`

```text
import * as React from "react"
import * as SwitchPrimitives from "@radix-ui/react-switch"

import { cn } from "@/lib/utils"

const Switch = React.forwardRef(({ className, ...props }, ref) => (
  <SwitchPrimitives.Root
    className={cn(
      "peer inline-flex h-5 w-9 shrink-0 cursor-pointer items-center rounded-full border-2 border-transparent shadow-sm transition-colors focus-visible:outline-none focus-visible:ring-2 focus-visible:ring-ring focus-visible:ring-offset-2 focus-visible:ring-offset-background disabled:cursor-not-allowed disabled:opacity-50 data-[state=checked]:bg-primary data-[state=unchecked]:bg-input",
      className
    )}
    {...props}
    ref={ref}>
    <SwitchPrimitives.Thumb
      className={cn(
        "pointer-events-none block h-4 w-4 rounded-full bg-background shadow-lg ring-0 transition-transform data-[state=checked]:translate-x-4 data-[state=unchecked]:translate-x-0"
      )} />
  </SwitchPrimitives.Root>
))
Switch.displayName = SwitchPrimitives.Root.displayName

export { Switch }

```

---

## File: `src/components/ui/menubar.jsx`

```text
"use client"

import * as React from "react"
import * as MenubarPrimitive from "@radix-ui/react-menubar"
import { Check, ChevronRight, Circle } from "lucide-react"

import { cn } from "@/lib/utils"

function MenubarMenu({
  ...props
}) {
  return <MenubarPrimitive.Menu {...props} />;
}

function MenubarGroup({
  ...props
}) {
  return <MenubarPrimitive.Group {...props} />;
}

function MenubarPortal({
  ...props
}) {
  return <MenubarPrimitive.Portal {...props} />;
}

function MenubarRadioGroup({
  ...props
}) {
  return <MenubarPrimitive.RadioGroup {...props} />;
}

function MenubarSub({
  ...props
}) {
  return <MenubarPrimitive.Sub data-slot="menubar-sub" {...props} />;
}

const Menubar = React.forwardRef(({ className, ...props }, ref) => (
  <MenubarPrimitive.Root
    ref={ref}
    className={cn(
      "flex h-9 items-center space-x-1 rounded-md border bg-background p-1 shadow-sm",
      className
    )}
    {...props} />
))
Menubar.displayName = MenubarPrimitive.Root.displayName

const MenubarTrigger = React.forwardRef(({ className, ...props }, ref) => (
  <MenubarPrimitive.Trigger
    ref={ref}
    className={cn(
      "flex cursor-default select-none items-center rounded-sm px-3 py-1 text-sm font-medium outline-none focus:bg-accent focus:text-accent-foreground data-[state=open]:bg-accent data-[state=open]:text-accent-foreground",
      className
    )}
    {...props} />
))
MenubarTrigger.displayName = MenubarPrimitive.Trigger.displayName

const MenubarSubTrigger = React.forwardRef(({ className, inset, children, ...props }, ref) => (
  <MenubarPrimitive.SubTrigger
    ref={ref}
    className={cn(
      "flex cursor-default select-none items-center rounded-sm px-2 py-1.5 text-sm outline-none focus:bg-accent focus:text-accent-foreground data-[state=open]:bg-accent data-[state=open]:text-accent-foreground",
      inset && "pl-8",
      className
    )}
    {...props}>
    {children}
    <ChevronRight className="ml-auto h-4 w-4" />
  </MenubarPrimitive.SubTrigger>
))
MenubarSubTrigger.displayName = MenubarPrimitive.SubTrigger.displayName

const MenubarSubContent = React.forwardRef(({ className, ...props }, ref) => (
  <MenubarPrimitive.SubContent
    ref={ref}
    className={cn(
      "z-50 min-w-[8rem] overflow-hidden rounded-md border bg-popover p-1 text-popover-foreground shadow-lg data-[state=open]:animate-in data-[state=closed]:animate-out data-[state=closed]:fade-out-0 data-[state=open]:fade-in-0 data-[state=closed]:zoom-out-95 data-[state=open]:zoom-in-95 data-[side=bottom]:slide-in-from-top-2 data-[side=left]:slide-in-from-right-2 data-[side=right]:slide-in-from-left-2 data-[side=top]:slide-in-from-bottom-2",
      className
    )}
    {...props} />
))
MenubarSubContent.displayName = MenubarPrimitive.SubContent.displayName

const MenubarContent = React.forwardRef((
  { className, align = "start", alignOffset = -4, sideOffset = 8, ...props },
  ref
) => (
  <MenubarPrimitive.Portal>
    <MenubarPrimitive.Content
      ref={ref}
      align={align}
      alignOffset={alignOffset}
      sideOffset={sideOffset}
      className={cn(
        "z-50 min-w-[12rem] overflow-hidden rounded-md border bg-popover p-1 text-popover-foreground shadow-md data-[state=open]:animate-in data-[state=closed]:fade-out-0 data-[state=open]:fade-in-0 data-[state=closed]:zoom-out-95 data-[state=open]:zoom-in-95 data-[side=bottom]:slide-in-from-top-2 data-[side=left]:slide-in-from-right-2 data-[side=right]:slide-in-from-left-2 data-[side=top]:slide-in-from-bottom-2",
        className
      )}
      {...props} />
  </MenubarPrimitive.Portal>
))
MenubarContent.displayName = MenubarPrimitive.Content.displayName

const MenubarItem = React.forwardRef(({ className, inset, ...props }, ref) => (
  <MenubarPrimitive.Item
    ref={ref}
    className={cn(
      "relative flex cursor-default select-none items-center rounded-sm px-2 py-1.5 text-sm outline-none focus:bg-accent focus:text-accent-foreground data-[disabled]:pointer-events-none data-[disabled]:opacity-50",
      inset && "pl-8",
      className
    )}
    {...props} />
))
MenubarItem.displayName = MenubarPrimitive.Item.displayName

const MenubarCheckboxItem = React.forwardRef(({ className, children, checked, ...props }, ref) => (
  <MenubarPrimitive.CheckboxItem
    ref={ref}
    className={cn(
      "relative flex cursor-default select-none items-center rounded-sm py-1.5 pl-8 pr-2 text-sm outline-none focus:bg-accent focus:text-accent-foreground data-[disabled]:pointer-events-none data-[disabled]:opacity-50",
      className
    )}
    checked={checked}
    {...props}>
    <span className="absolute left-2 flex h-3.5 w-3.5 items-center justify-center">
      <MenubarPrimitive.ItemIndicator>
        <Check className="h-4 w-4" />
      </MenubarPrimitive.ItemIndicator>
    </span>
    {children}
  </MenubarPrimitive.CheckboxItem>
))
MenubarCheckboxItem.displayName = MenubarPrimitive.CheckboxItem.displayName

const MenubarRadioItem = React.forwardRef(({ className, children, ...props }, ref) => (
  <MenubarPrimitive.RadioItem
    ref={ref}
    className={cn(
      "relative flex cursor-default select-none items-center rounded-sm py-1.5 pl-8 pr-2 text-sm outline-none focus:bg-accent focus:text-accent-foreground data-[disabled]:pointer-events-none data-[disabled]:opacity-50",
      className
    )}
    {...props}>
    <span className="absolute left-2 flex h-3.5 w-3.5 items-center justify-center">
      <MenubarPrimitive.ItemIndicator>
        <Circle className="h-4 w-4 fill-current" />
      </MenubarPrimitive.ItemIndicator>
    </span>
    {children}
  </MenubarPrimitive.RadioItem>
))
MenubarRadioItem.displayName = MenubarPrimitive.RadioItem.displayName

const MenubarLabel = React.forwardRef(({ className, inset, ...props }, ref) => (
  <MenubarPrimitive.Label
    ref={ref}
    className={cn("px-2 py-1.5 text-sm font-semibold", inset && "pl-8", className)}
    {...props} />
))
MenubarLabel.displayName = MenubarPrimitive.Label.displayName

const MenubarSeparator = React.forwardRef(({ className, ...props }, ref) => (
  <MenubarPrimitive.Separator
    ref={ref}
    className={cn("-mx-1 my-1 h-px bg-muted", className)}
    {...props} />
))
MenubarSeparator.displayName = MenubarPrimitive.Separator.displayName

const MenubarShortcut = ({
  className,
  ...props
}) => {
  return (
    (<span
      className={cn("ml-auto text-xs tracking-widest text-muted-foreground", className)}
      {...props} />)
  );
}
MenubarShortcut.displayname = "MenubarShortcut"

export {
  Menubar,
  MenubarMenu,
  MenubarTrigger,
  MenubarContent,
  MenubarItem,
  MenubarSeparator,
  MenubarLabel,
  MenubarCheckboxItem,
  MenubarRadioGroup,
  MenubarRadioItem,
  MenubarPortal,
  MenubarSubContent,
  MenubarSubTrigger,
  MenubarGroup,
  MenubarSub,
  MenubarShortcut,
}

```

---

## File: `src/components/ui/input.jsx`

```text
import * as React from "react"

import { cn } from "@/lib/utils"

const Input = React.forwardRef(({ className, type, ...props }, ref) => {
  return (
    (<input
      type={type}
      className={cn(
        "flex h-9 w-full rounded-md border border-input bg-transparent px-3 py-1 text-base shadow-sm transition-colors file:border-0 file:bg-transparent file:text-sm file:font-medium file:text-foreground placeholder:text-muted-foreground focus-visible:outline-none focus-visible:ring-1 focus-visible:ring-ring disabled:cursor-not-allowed disabled:opacity-50 md:text-sm",
        className
      )}
      ref={ref}
      {...props} />)
  );
})
Input.displayName = "Input"

export { Input }

```

---

## File: `src/components/ui/scroll-area.jsx`

```text
import * as React from "react"
import * as ScrollAreaPrimitive from "@radix-ui/react-scroll-area"

import { cn } from "@/lib/utils"

const ScrollArea = React.forwardRef(({ className, children, ...props }, ref) => (
  <ScrollAreaPrimitive.Root
    ref={ref}
    className={cn("relative overflow-hidden", className)}
    {...props}>
    <ScrollAreaPrimitive.Viewport className="h-full w-full rounded-[inherit]">
      {children}
    </ScrollAreaPrimitive.Viewport>
    <ScrollBar />
    <ScrollAreaPrimitive.Corner />
  </ScrollAreaPrimitive.Root>
))
ScrollArea.displayName = ScrollAreaPrimitive.Root.displayName

const ScrollBar = React.forwardRef(({ className, orientation = "vertical", ...props }, ref) => (
  <ScrollAreaPrimitive.ScrollAreaScrollbar
    ref={ref}
    orientation={orientation}
    className={cn(
      "flex touch-none select-none transition-colors",
      orientation === "vertical" &&
        "h-full w-2.5 border-l border-l-transparent p-[1px]",
      orientation === "horizontal" &&
        "h-2.5 flex-col border-t border-t-transparent p-[1px]",
      className
    )}
    {...props}>
    <ScrollAreaPrimitive.ScrollAreaThumb className="relative flex-1 rounded-full bg-border" />
  </ScrollAreaPrimitive.ScrollAreaScrollbar>
))
ScrollBar.displayName = ScrollAreaPrimitive.ScrollAreaScrollbar.displayName

export { ScrollArea, ScrollBar }

```

---

## File: `src/components/ui/chart.jsx`

```text
"use client";
import * as React from "react"
import * as RechartsPrimitive from "recharts"

import { cn } from "@/lib/utils"

// Format: { THEME_NAME: CSS_SELECTOR }
const THEMES = {
  light: "",
  dark: ".dark"
}

const ChartContext = React.createContext(null)

function useChart() {
  const context = React.useContext(ChartContext)

  if (!context) {
    throw new Error("useChart must be used within a <ChartContainer />")
  }

  return context
}

const ChartContainer = React.forwardRef(({ id, className, children, config, ...props }, ref) => {
  const uniqueId = React.useId()
  const chartId = `chart-${id || uniqueId.replace(/:/g, "")}`

  return (
    (<ChartContext.Provider value={{ config }}>
      <div
        data-chart={chartId}
        ref={ref}
        className={cn(
          "flex aspect-video justify-center text-xs [&_.recharts-cartesian-axis-tick_text]:fill-muted-foreground [&_.recharts-cartesian-grid_line[stroke='#ccc']]:stroke-border/50 [&_.recharts-curve.recharts-tooltip-cursor]:stroke-border [&_.recharts-dot[stroke='#fff']]:stroke-transparent [&_.recharts-layer]:outline-none [&_.recharts-polar-grid_[stroke='#ccc']]:stroke-border [&_.recharts-radial-bar-background-sector]:fill-muted [&_.recharts-rectangle.recharts-tooltip-cursor]:fill-muted [&_.recharts-reference-line_[stroke='#ccc']]:stroke-border [&_.recharts-sector[stroke='#fff']]:stroke-transparent [&_.recharts-sector]:outline-none [&_.recharts-surface]:outline-none",
          className
        )}
        {...props}>
        <ChartStyle id={chartId} config={config} />
        <RechartsPrimitive.ResponsiveContainer>
          {children}
        </RechartsPrimitive.ResponsiveContainer>
      </div>
    </ChartContext.Provider>)
  );
})
ChartContainer.displayName = "Chart"

const ChartStyle = ({
  id,
  config
}) => {
  const colorConfig = Object.entries(config).filter(([, config]) => config.theme || config.color)

  if (!colorConfig.length) {
    return null
  }

  return (
    (<style
      dangerouslySetInnerHTML={{
        __html: Object.entries(THEMES)
          .map(([theme, prefix]) => `
${prefix} [data-chart=${id}] {
${colorConfig
.map(([key, itemConfig]) => {
const color =
  itemConfig.theme?.[theme] ||
  itemConfig.color
return color ? `  --color-${key}: ${color};` : null
})
.join("\n")}
}
`)
          .join("\n"),
      }} />)
  );
}

const ChartTooltip = RechartsPrimitive.Tooltip

const ChartTooltipContent = React.forwardRef((
  {
    active,
    payload,
    className,
    indicator = "dot",
    hideLabel = false,
    hideIndicator = false,
    label,
    labelFormatter,
    labelClassName,
    formatter,
    color,
    nameKey,
    labelKey,
  },
  ref
) => {
  const { config } = useChart()

  const tooltipLabel = React.useMemo(() => {
    if (hideLabel || !payload?.length) {
      return null
    }

    const [item] = payload
    const key = `${labelKey || item.dataKey || item.name || "value"}`
    const itemConfig = getPayloadConfigFromPayload(config, item, key)
    const value =
      !labelKey && typeof label === "string"
        ? config[label]?.label || label
        : itemConfig?.label

    if (labelFormatter) {
      return (
        (<div className={cn("font-medium", labelClassName)}>
          {labelFormatter(value, payload)}
        </div>)
      );
    }

    if (!value) {
      return null
    }

    return <div className={cn("font-medium", labelClassName)}>{value}</div>;
  }, [
    label,
    labelFormatter,
    payload,
    hideLabel,
    labelClassName,
    config,
    labelKey,
  ])

  if (!active || !payload?.length) {
    return null
  }

  const nestLabel = payload.length === 1 && indicator !== "dot"

  return (
    (<div
      ref={ref}
      className={cn(
        "grid min-w-[8rem] items-start gap-1.5 rounded-lg border border-border/50 bg-background px-2.5 py-1.5 text-xs shadow-xl",
        className
      )}>
      {!nestLabel ? tooltipLabel : null}
      <div className="grid gap-1.5">
        {payload.map((item, index) => {
          const key = `${nameKey || item.name || item.dataKey || "value"}`
          const itemConfig = getPayloadConfigFromPayload(config, item, key)
          const indicatorColor = color || item.payload.fill || item.color

          return (
            (<div
              key={item.dataKey}
              className={cn(
                "flex w-full flex-wrap items-stretch gap-2 [&>svg]:h-2.5 [&>svg]:w-2.5 [&>svg]:text-muted-foreground",
                indicator === "dot" && "items-center"
              )}>
              {formatter && item?.value !== undefined && item.name ? (
                formatter(item.value, item.name, item, index, item.payload)
              ) : (
                <>
                  {itemConfig?.icon ? (
                    <itemConfig.icon />
                  ) : (
                    !hideIndicator && (
                      <div
                        className={cn("shrink-0 rounded-[2px] border-[--color-border] bg-[--color-bg]", {
                          "h-2.5 w-2.5": indicator === "dot",
                          "w-1": indicator === "line",
                          "w-0 border-[1.5px] border-dashed bg-transparent":
                            indicator === "dashed",
                          "my-0.5": nestLabel && indicator === "dashed",
                        })}
                        style={
                          {
                            "--color-bg": indicatorColor,
                            "--color-border": indicatorColor
                          }
                        } />
                    )
                  )}
                  <div
                    className={cn(
                      "flex flex-1 justify-between leading-none",
                      nestLabel ? "items-end" : "items-center"
                    )}>
                    <div className="grid gap-1.5">
                      {nestLabel ? tooltipLabel : null}
                      <span className="text-muted-foreground">
                        {itemConfig?.label || item.name}
                      </span>
                    </div>
                    {item.value && (
                      <span className="font-mono font-medium tabular-nums text-foreground">
                        {item.value.toLocaleString()}
                      </span>
                    )}
                  </div>
                </>
              )}
            </div>)
          );
        })}
      </div>
    </div>)
  );
})
ChartTooltipContent.displayName = "ChartTooltip"

const ChartLegend = RechartsPrimitive.Legend

const ChartLegendContent = React.forwardRef((
  { className, hideIcon = false, payload, verticalAlign = "bottom", nameKey },
  ref
) => {
  const { config } = useChart()

  if (!payload?.length) {
    return null
  }

  return (
    (<div
      ref={ref}
      className={cn(
        "flex items-center justify-center gap-4",
        verticalAlign === "top" ? "pb-3" : "pt-3",
        className
      )}>
      {payload.map((item) => {
        const key = `${nameKey || item.dataKey || "value"}`
        const itemConfig = getPayloadConfigFromPayload(config, item, key)

        return (
          (<div
            key={item.value}
            className={cn(
              "flex items-center gap-1.5 [&>svg]:h-3 [&>svg]:w-3 [&>svg]:text-muted-foreground"
            )}>
            {itemConfig?.icon && !hideIcon ? (
              <itemConfig.icon />
            ) : (
              <div
                className="h-2 w-2 shrink-0 rounded-[2px]"
                style={{
                  backgroundColor: item.color,
                }} />
            )}
            {itemConfig?.label}
          </div>)
        );
      })}
    </div>)
  );
})
ChartLegendContent.displayName = "ChartLegend"

// Helper to extract item config from a payload.
function getPayloadConfigFromPayload(
  config,
  payload,
  key
) {
  if (typeof payload !== "object" || payload === null) {
    return undefined
  }

  const payloadPayload =
    "payload" in payload &&
    typeof payload.payload === "object" &&
    payload.payload !== null
      ? payload.payload
      : undefined

  let configLabelKey = key

  if (
    key in payload &&
    typeof payload[key] === "string"
  ) {
    configLabelKey = payload[key]
  } else if (
    payloadPayload &&
    key in payloadPayload &&
    typeof payloadPayload[key] === "string"
  ) {
    configLabelKey = payloadPayload[key]
  }

  return configLabelKey in config
    ? config[configLabelKey]
    : config[key];
}

export {
  ChartContainer,
  ChartTooltip,
  ChartTooltipContent,
  ChartLegend,
  ChartLegendContent,
  ChartStyle,
}

```

---

## File: `src/components/ui/input-otp.jsx`

```text
import * as React from "react"
import { OTPInput, OTPInputContext } from "input-otp"
import { Minus } from "lucide-react"

import { cn } from "@/lib/utils"

const InputOTP = React.forwardRef(({ className, containerClassName, ...props }, ref) => (
  <OTPInput
    ref={ref}
    containerClassName={cn("flex items-center gap-2 has-[:disabled]:opacity-50", containerClassName)}
    className={cn("disabled:cursor-not-allowed", className)}
    {...props} />
))
InputOTP.displayName = "InputOTP"

const InputOTPGroup = React.forwardRef(({ className, ...props }, ref) => (
  <div ref={ref} className={cn("flex items-center", className)} {...props} />
))
InputOTPGroup.displayName = "InputOTPGroup"

const InputOTPSlot = React.forwardRef(({ index, className, ...props }, ref) => {
  const inputOTPContext = React.useContext(OTPInputContext)
  const { char, hasFakeCaret, isActive } = inputOTPContext.slots[index]

  return (
    (<div
      ref={ref}
      className={cn(
        "relative flex h-9 w-9 items-center justify-center border-y border-r border-input text-sm shadow-sm transition-all first:rounded-l-md first:border-l last:rounded-r-md",
        isActive && "z-10 ring-1 ring-ring",
        className
      )}
      {...props}>
      {char}
      {hasFakeCaret && (
        <div
          className="pointer-events-none absolute inset-0 flex items-center justify-center">
          <div className="h-4 w-px animate-caret-blink bg-foreground duration-1000" />
        </div>
      )}
    </div>)
  );
})
InputOTPSlot.displayName = "InputOTPSlot"

const InputOTPSeparator = React.forwardRef(({ ...props }, ref) => (
  <div ref={ref} role="separator" {...props}>
    <Minus />
  </div>
))
InputOTPSeparator.displayName = "InputOTPSeparator"

export { InputOTP, InputOTPGroup, InputOTPSlot, InputOTPSeparator }

```

---

## File: `src/components/ui/tooltip.jsx`

```text
"use client"

import * as React from "react"
import * as TooltipPrimitive from "@radix-ui/react-tooltip"

import { cn } from "@/lib/utils"

const TooltipProvider = TooltipPrimitive.Provider

const Tooltip = TooltipPrimitive.Root

const TooltipTrigger = TooltipPrimitive.Trigger

const TooltipContent = React.forwardRef(({ className, sideOffset = 4, ...props }, ref) => (
  <TooltipPrimitive.Portal>
    <TooltipPrimitive.Content
      ref={ref}
      sideOffset={sideOffset}
      className={cn(
        "z-50 overflow-hidden rounded-md bg-primary px-3 py-1.5 text-xs text-primary-foreground animate-in fade-in-0 zoom-in-95 data-[state=closed]:animate-out data-[state=closed]:fade-out-0 data-[state=closed]:zoom-out-95 data-[side=bottom]:slide-in-from-top-2 data-[side=left]:slide-in-from-right-2 data-[side=right]:slide-in-from-left-2 data-[side=top]:slide-in-from-bottom-2",
        className
      )}
      {...props} />
  </TooltipPrimitive.Portal>
))
TooltipContent.displayName = TooltipPrimitive.Content.displayName

export { Tooltip, TooltipTrigger, TooltipContent, TooltipProvider }

```

---

## File: `src/components/ui/sonner.jsx`

```text
"use client";
import { useTheme } from "next-themes"
import { Toaster as Sonner } from "sonner"

const Toaster = ({
  ...props
}) => {
  const { theme = "system" } = useTheme()

  return (
    (<Sonner
      theme={theme}
      className="toaster group"
      toastOptions={{
        classNames: {
          toast:
            "group toast group-[.toaster]:bg-background group-[.toaster]:text-foreground group-[.toaster]:border-border group-[.toaster]:shadow-lg",
          description: "group-[.toast]:text-muted-foreground",
          actionButton:
            "group-[.toast]:bg-primary group-[.toast]:text-primary-foreground",
          cancelButton:
            "group-[.toast]:bg-muted group-[.toast]:text-muted-foreground",
        },
      }}
      {...props} />)
  );
}

export { Toaster }

```

---

## File: `src/components/ui/collapsible.jsx`

```text
"use client"

import * as CollapsiblePrimitive from "@radix-ui/react-collapsible"

const Collapsible = CollapsiblePrimitive.Root

const CollapsibleTrigger = CollapsiblePrimitive.CollapsibleTrigger

const CollapsibleContent = CollapsiblePrimitive.CollapsibleContent

export { Collapsible, CollapsibleTrigger, CollapsibleContent }

```

---

## File: `src/components/ui/card.jsx`

```text
import * as React from "react"

import { cn } from "@/lib/utils"

const Card = React.forwardRef(({ className, ...props }, ref) => (
  <div
    ref={ref}
    className={cn("rounded-xl border bg-card text-card-foreground shadow", className)}
    {...props} />
))
Card.displayName = "Card"

const CardHeader = React.forwardRef(({ className, ...props }, ref) => (
  <div
    ref={ref}
    className={cn("flex flex-col space-y-1.5 p-6", className)}
    {...props} />
))
CardHeader.displayName = "CardHeader"

const CardTitle = React.forwardRef(({ className, ...props }, ref) => (
  <div
    ref={ref}
    className={cn("font-semibold leading-none tracking-tight", className)}
    {...props} />
))
CardTitle.displayName = "CardTitle"

const CardDescription = React.forwardRef(({ className, ...props }, ref) => (
  <div
    ref={ref}
    className={cn("text-sm text-muted-foreground", className)}
    {...props} />
))
CardDescription.displayName = "CardDescription"

const CardContent = React.forwardRef(({ className, ...props }, ref) => (
  <div ref={ref} className={cn("p-6 pt-0", className)} {...props} />
))
CardContent.displayName = "CardContent"

const CardFooter = React.forwardRef(({ className, ...props }, ref) => (
  <div
    ref={ref}
    className={cn("flex items-center p-6 pt-0", className)}
    {...props} />
))
CardFooter.displayName = "CardFooter"

export { Card, CardHeader, CardFooter, CardTitle, CardDescription, CardContent }

```

---

## File: `src/components/ui/button.jsx`

```text
import * as React from "react"
import { Slot } from "@radix-ui/react-slot"
import { cva } from "class-variance-authority";

import { cn } from "@/lib/utils"

const buttonVariants = cva(
  "inline-flex items-center justify-center gap-2 whitespace-nowrap rounded-md text-sm font-medium transition-colors focus-visible:outline-none focus-visible:ring-1 focus-visible:ring-ring disabled:pointer-events-none disabled:opacity-50 [&_svg]:pointer-events-none [&_svg]:size-4 [&_svg]:shrink-0",
  {
    variants: {
      variant: {
        default:
          "bg-primary text-primary-foreground shadow hover:bg-primary/90",
        destructive:
          "bg-destructive text-destructive-foreground shadow-sm hover:bg-destructive/90",
        outline:
          "border border-input bg-transparent shadow-sm hover:bg-accent hover:text-accent-foreground",
        secondary:
          "bg-secondary text-secondary-foreground shadow-sm hover:bg-secondary/80",
        ghost: "hover:bg-accent hover:text-accent-foreground",
        link: "text-primary underline-offset-4 hover:underline",
      },
      size: {
        default: "h-9 px-4 py-2",
        sm: "h-8 rounded-md px-3 text-xs",
        lg: "h-10 rounded-md px-8",
        icon: "h-9 w-9",
      },
    },
    defaultVariants: {
      variant: "default",
      size: "default",
    },
  }
)

const Button = React.forwardRef(({ className, variant, size, asChild = false, ...props }, ref) => {
  const Comp = asChild ? Slot : "button"
  return (
    (<Comp
      className={cn(buttonVariants({ variant, size, className }))}
      ref={ref}
      {...props} />)
  );
})
Button.displayName = "Button"

export { Button, buttonVariants }

```

---

## File: `src/components/ui/toaster.jsx`

```text
import { useToast } from "@/components/ui/use-toast";
import {
  Toast,
  ToastClose,
  ToastDescription,
  ToastProvider,
  ToastTitle,
  ToastViewport,
} from "@/components/ui/toast";

export function Toaster() {
  const { toasts } = useToast();

  return (
    <ToastProvider>
      {toasts.map(function ({ id, title, description, action, ...props }) {
        return (
          <Toast key={id} {...props}>
            <div className="grid gap-1">
              {title && <ToastTitle>{title}</ToastTitle>}
              {description && (
                <ToastDescription>{description}</ToastDescription>
              )}
            </div>
            {action}
            <ToastClose />
          </Toast>
        );
      })}
      <ToastViewport />
    </ToastProvider>
  );
} 
```

---

## File: `src/pages/ResetPassword.jsx`

```text
import React, { useState } from "react";
import { Link, useSearchParams } from "react-router-dom";
import { base44 } from "@/api/base44Client";
import { Button } from "@/components/ui/button";
import { Input } from "@/components/ui/input";
import { Label } from "@/components/ui/label";
import { Lock, Loader2, AlertTriangle } from "lucide-react";
import AuthLayout from "@/components/AuthLayout";

export default function ResetPassword() {
  const [searchParams] = useSearchParams();
  const resetToken = searchParams.get("token");

  const [newPassword, setNewPassword] = useState("");
  const [confirmPassword, setConfirmPassword] = useState("");
  const [error, setError] = useState("");
  const [loading, setLoading] = useState(false);

  const handleSubmit = async (e) => {
    e.preventDefault();
    setError("");
    if (newPassword !== confirmPassword) {
      setError("Passwords do not match");
      return;
    }
    setLoading(true);
    try {
      await base44.auth.resetPassword({ resetToken, newPassword });
      window.location.href = "/login";
    } catch (err) {
      setError(err.message || "Failed to reset password");
    } finally {
      setLoading(false);
    }
  };

  if (!resetToken) {
    return (
      <AuthLayout
        icon={AlertTriangle}
        title="Invalid reset link"
        subtitle="This password reset link is missing or invalid"
        footer={
          <Link to="/forgot-password" className="text-primary font-medium hover:underline">
            Request a new link
          </Link>
        }
      >
        <p className="text-sm text-foreground text-center">
          The link you used appears to be incomplete. Please request a new password reset email.
        </p>
      </AuthLayout>
    );
  }

  return (
    <AuthLayout
      icon={Lock}
      title="New password"
      subtitle="Enter your new password below"
    >
      {error && (
        <div className="mb-4 p-3 rounded-lg bg-destructive/10 text-destructive text-sm">
          {error}
        </div>
      )}
      <form onSubmit={handleSubmit} className="space-y-4">
        <div className="space-y-2">
          <Label htmlFor="password">New Password</Label>
          <div className="relative">
            <Lock className="absolute left-3 top-1/2 -translate-y-1/2 w-4 h-4 text-muted-foreground" aria-hidden="true" />
            <Input
              id="password"
              type="password"
              autoComplete="new-password"
              autoFocus
              placeholder="••••••••"
              value={newPassword}
              onChange={(e) => setNewPassword(e.target.value)}
              className="pl-10 h-12"
              required
            />
          </div>
        </div>
        <div className="space-y-2">
          <Label htmlFor="confirm">Confirm Password</Label>
          <div className="relative">
            <Lock className="absolute left-3 top-1/2 -translate-y-1/2 w-4 h-4 text-muted-foreground" aria-hidden="true" />
            <Input
              id="confirm"
              type="password"
              autoComplete="new-password"
              placeholder="••••••••"
              value={confirmPassword}
              onChange={(e) => setConfirmPassword(e.target.value)}
              className="pl-10 h-12"
              required
            />
          </div>
        </div>
        <Button type="submit" className="w-full h-12 font-medium" disabled={loading}>
          {loading ? (
            <>
              <Loader2 className="w-4 h-4 mr-2 animate-spin" />
              Resetting...
            </>
          ) : (
            "Reset password"
          )}
        </Button>
      </form>
    </AuthLayout>
  );
}

```

---

## File: `src/pages/Register.jsx`

```text
import React, { useState } from "react";
import { Link } from "react-router-dom";
import { base44 } from "@/api/base44Client";
import { Button } from "@/components/ui/button";
import { Input } from "@/components/ui/input";
import { Label } from "@/components/ui/label";
import { UserPlus, Mail, Lock, Loader2 } from "lucide-react";
import { InputOTP, InputOTPGroup, InputOTPSlot } from "@/components/ui/input-otp";
import AuthLayout from "@/components/AuthLayout";
import GoogleIcon from "@/components/GoogleIcon";
import { toast } from "@/components/ui/use-toast";

export default function Register() {
  const [email, setEmail] = useState("");
  const [password, setPassword] = useState("");
  const [confirmPassword, setConfirmPassword] = useState("");
  const [error, setError] = useState("");
  const [loading, setLoading] = useState(false);
  const [showOtp, setShowOtp] = useState(false);
  const [otpCode, setOtpCode] = useState("");

  const handleSubmit = async (e) => {
    e.preventDefault();
    setError("");
    if (password !== confirmPassword) {
      setError("Passwords do not match");
      return;
    }
    setLoading(true);
    try {
      await base44.auth.register({ email, password });
      setShowOtp(true);
    } catch (err) {
      setError(err.message || "Registration failed");
    } finally {
      setLoading(false);
    }
  };

  const handleVerify = async () => {
    setError("");
    setLoading(true);
    try {
      const result = await base44.auth.verifyOtp({ email, otpCode });
      if (result?.access_token) {
        base44.auth.setToken(result.access_token);
      }
      window.location.href = "/";
    } catch (err) {
      setError(err.message || "Invalid verification code");
    } finally {
      setLoading(false);
    }
  };

  const handleResend = async () => {
    setError("");
    try {
      await base44.auth.resendOtp(email);
      toast({
        title: "Code sent",
        description: "Check your email for the new code.",
      });
    } catch (err) {
      setError(err.message || "Failed to resend code");
    }
  };

  const handleGoogle = () => {
    base44.auth.loginWithProvider("google", "/");
  };

  if (showOtp) {
    return (
      <AuthLayout
        icon={Mail}
        title="Verify your email"
        subtitle={`We sent a code to ${email}`}
      >
        {error && (
          <div className="mb-4 p-3 rounded-lg bg-destructive/10 text-destructive text-sm">
            {error}
          </div>
        )}
        <div className="flex justify-center mb-6">
          <InputOTP
            maxLength={6}
            value={otpCode}
            onChange={setOtpCode}
            autoFocus
            autoComplete="one-time-code"
          >
            <InputOTPGroup>
              <InputOTPSlot index={0} />
              <InputOTPSlot index={1} />
              <InputOTPSlot index={2} />
              <InputOTPSlot index={3} />
              <InputOTPSlot index={4} />
              <InputOTPSlot index={5} />
            </InputOTPGroup>
          </InputOTP>
        </div>
        <Button
          className="w-full h-12 font-medium"
          onClick={handleVerify}
          disabled={loading || otpCode.length < 6}
        >
          {loading ? (
            <>
              <Loader2 className="w-4 h-4 mr-2 animate-spin" />
              Verifying...
            </>
          ) : (
            "Verify"
          )}
        </Button>
        <p className="text-center text-sm text-muted-foreground mt-4">
          Didn't receive the code?{" "}
          <button onClick={handleResend} className="text-primary font-medium hover:underline">
            Resend
          </button>
        </p>
      </AuthLayout>
    );
  }

  return (
    <AuthLayout
      icon={UserPlus}
      title="Create your account"
      subtitle="Sign up to get started"
      footer={
        <>
          Already have an account?{" "}
          <Link to="/login" className="text-primary font-medium hover:underline">
            Log in
          </Link>
        </>
      }
    >
      <Button
        variant="outline"
        className="w-full h-12 text-sm font-medium mb-6"
        onClick={handleGoogle}
      >
        <GoogleIcon className="w-5 h-5 mr-2" />
        Continue with Google
      </Button>

      <div className="relative mb-6">
        <div className="absolute inset-0 flex items-center">
          <div className="w-full border-t border-border" />
        </div>
        <div className="relative flex justify-center text-xs uppercase">
          <span className="bg-card px-3 text-muted-foreground">or</span>
        </div>
      </div>

      {error && (
        <div className="mb-4 p-3 rounded-lg bg-destructive/10 text-destructive text-sm">
          {error}
        </div>
      )}

      <form onSubmit={handleSubmit} className="space-y-4">
        <div className="space-y-2">
          <Label htmlFor="email">Email</Label>
          <div className="relative">
            <Mail className="absolute left-3 top-1/2 -translate-y-1/2 w-4 h-4 text-muted-foreground" aria-hidden="true" />
            <Input
              id="email"
              type="email"
              autoComplete="email"
              autoFocus
              placeholder="you@example.com"
              value={email}
              onChange={(e) => setEmail(e.target.value)}
              className="pl-10 h-12"
              required
            />
          </div>
        </div>
        <div className="space-y-2">
          <Label htmlFor="password">Password</Label>
          <div className="relative">
            <Lock className="absolute left-3 top-1/2 -translate-y-1/2 w-4 h-4 text-muted-foreground" aria-hidden="true" />
            <Input
              id="password"
              type="password"
              autoComplete="new-password"
              placeholder="••••••••"
              value={password}
              onChange={(e) => setPassword(e.target.value)}
              className="pl-10 h-12"
              required
            />
          </div>
        </div>
        <div className="space-y-2">
          <Label htmlFor="confirm">Confirm Password</Label>
          <div className="relative">
            <Lock className="absolute left-3 top-1/2 -translate-y-1/2 w-4 h-4 text-muted-foreground" aria-hidden="true" />
            <Input
              id="confirm"
              type="password"
              autoComplete="new-password"
              placeholder="••••••••"
              value={confirmPassword}
              onChange={(e) => setConfirmPassword(e.target.value)}
              className="pl-10 h-12"
              required
            />
          </div>
        </div>
        <Button type="submit" className="w-full h-12 font-medium" disabled={loading}>
          {loading ? (
            <>
              <Loader2 className="w-4 h-4 mr-2 animate-spin" />
              Creating account...
            </>
          ) : (
            "Create account"
          )}
        </Button>
      </form>
    </AuthLayout>
  );
}

```

---

## File: `src/pages/ForgotPassword.jsx`

```text
import React, { useState } from "react";
import { Link } from "react-router-dom";
import { base44 } from "@/api/base44Client";
import { Button } from "@/components/ui/button";
import { Input } from "@/components/ui/input";
import { Label } from "@/components/ui/label";
import { Mail, ArrowLeft, Loader2 } from "lucide-react";
import AuthLayout from "@/components/AuthLayout";

export default function ForgotPassword() {
  const [email, setEmail] = useState("");
  const [loading, setLoading] = useState(false);
  const [sent, setSent] = useState(false);

  const handleSubmit = async (e) => {
    e.preventDefault();
    setLoading(true);
    try {
      await base44.auth.resetPasswordRequest(email);
    } catch {
      // Always show success regardless
    } finally {
      setLoading(false);
      setSent(true);
    }
  };

  return (
    <AuthLayout
      icon={Mail}
      title="Reset password"
      subtitle="We'll send you a link to reset it"
      footer={
        <Link to="/login" className="text-primary font-medium hover:underline">
          <ArrowLeft className="w-3 h-3 inline mr-1" />Back to log in
        </Link>
      }
    >
      {sent ? (
        <p className="text-sm text-foreground text-center">
          If an account exists with that email, you'll receive a password reset link shortly.
        </p>
      ) : (
        <form onSubmit={handleSubmit} className="space-y-4">
          <div className="space-y-2">
            <Label htmlFor="email">Email address</Label>
            <div className="relative">
              <Mail className="absolute left-3 top-1/2 -translate-y-1/2 w-4 h-4 text-muted-foreground" aria-hidden="true" />
              <Input
                id="email"
                type="email"
                autoComplete="email"
                autoFocus
                placeholder="you@example.com"
                value={email}
                onChange={(e) => setEmail(e.target.value)}
                className="pl-10 h-12"
                required
              />
            </div>
          </div>
          <Button type="submit" className="w-full h-12 font-medium" disabled={loading}>
            {loading ? (
              <>
                <Loader2 className="w-4 h-4 mr-2 animate-spin" />
                Sending...
              </>
            ) : (
              "Send reset link"
            )}
          </Button>
        </form>
      )}
    </AuthLayout>
  );
}

```

---

## File: `src/pages/Login.jsx`

```text
import React, { useState } from "react";
import { Link } from "react-router-dom";
import { base44 } from "@/api/base44Client";
import { Button } from "@/components/ui/button";
import { Input } from "@/components/ui/input";
import { Label } from "@/components/ui/label";
import { LogIn, Mail, Lock, Loader2 } from "lucide-react";
import AuthLayout from "@/components/AuthLayout";
import GoogleIcon from "@/components/GoogleIcon";

export default function Login() {
  const [email, setEmail] = useState("");
  const [password, setPassword] = useState("");
  const [error, setError] = useState("");
  const [loading, setLoading] = useState(false);

  const handleSubmit = async (e) => {
    e.preventDefault();
    setError("");
    setLoading(true);
    try {
      await base44.auth.loginViaEmailPassword(email, password);
      window.location.href = "/";
    } catch (err) {
      setError(err.message || "Invalid email or password");
    } finally {
      setLoading(false);
    }
  };

  const handleGoogle = () => {
    base44.auth.loginWithProvider("google", "/");
  };

  return (
    <AuthLayout
      icon={LogIn}
      title="Welcome back"
      subtitle="Log in to your account"
      footer={
        <>
          Don't have an account?{" "}
          <Link to="/register" className="text-primary font-medium hover:underline">
            Create one
          </Link>
        </>
      }
    >
      <Button
        variant="outline"
        className="w-full h-12 text-sm font-medium mb-6"
        onClick={handleGoogle}
      >
        <GoogleIcon className="w-5 h-5 mr-2" />
        Continue with Google
      </Button>

      <div className="relative mb-6">
        <div className="absolute inset-0 flex items-center">
          <div className="w-full border-t border-border" />
        </div>
        <div className="relative flex justify-center text-xs uppercase">
          <span className="bg-card px-3 text-muted-foreground">or</span>
        </div>
      </div>

      {error && (
        <div className="mb-4 p-3 rounded-lg bg-destructive/10 text-destructive text-sm">
          {error}
        </div>
      )}

      <form onSubmit={handleSubmit} className="space-y-4">
        <div className="space-y-2">
          <Label htmlFor="email">Email</Label>
          <div className="relative">
            <Mail className="absolute left-3 top-1/2 -translate-y-1/2 w-4 h-4 text-muted-foreground" aria-hidden="true" />
            <Input
              id="email"
              type="email"
              autoComplete="email"
              autoFocus
              placeholder="you@example.com"
              value={email}
              onChange={(e) => setEmail(e.target.value)}
              className="pl-10 h-12"
              required
            />
          </div>
        </div>
        <div className="space-y-2">
          <div className="flex items-center justify-between">
            <Label htmlFor="password">Password</Label>
            <Link to="/forgot-password" className="text-xs text-primary hover:underline">
              Forgot password?
            </Link>
          </div>
          <div className="relative">
            <Lock className="absolute left-3 top-1/2 -translate-y-1/2 w-4 h-4 text-muted-foreground" aria-hidden="true" />
            <Input
              id="password"
              type="password"
              autoComplete="current-password"
              placeholder="••••••••"
              value={password}
              onChange={(e) => setPassword(e.target.value)}
              className="pl-10 h-12"
              required
            />
          </div>
        </div>
        <Button type="submit" className="w-full h-12 font-medium" disabled={loading}>
          {loading ? (
            <>
              <Loader2 className="w-4 h-4 mr-2 animate-spin" />
              Logging in...
            </>
          ) : (
            "Log in"
          )}
        </Button>
      </form>
    </AuthLayout>
  );
}

```

---

## File: `src/pages/CheatSheet.jsx`

```text
import React from "react";
import { Link } from "react-router-dom";
import { ArrowLeft, BookOpen } from "lucide-react";
import { CHEAT_SECTIONS } from "@/components/forge/cheatSheet";
import { NEON } from "@/components/deck/deckColors";

export default function CheatSheet() {
  return (
    <div className="min-h-screen bg-zinc-950 text-zinc-100">
      <div className="max-w-3xl mx-auto px-6 py-12">
        <Link to="/" className="inline-flex items-center gap-2 text-zinc-500 hover:text-amber-400 text-sm font-mono mb-8 transition-colors">
          <ArrowLeft className="h-4 w-4" /> Back to the board
        </Link>

        <header className="mb-10">
          <div className="flex items-center gap-3 mb-2">
            <BookOpen className="h-6 w-6 text-amber-500" />
            <h1 className="font-heading text-3xl tracking-tight">
              Cheat Sheet <span className="text-zinc-500 font-light">· how to use THE FORGE</span>
            </h1>
          </div>
          <p className="text-zinc-500 text-sm">One page, everything an operator needs. Hand this to your client.</p>
        </header>

        <div className="space-y-8">
          {CHEAT_SECTIONS.map((sec) => {
            const c = NEON[sec.color] || NEON.cyan;
            return (
              <section key={sec.title} className={`rounded-xl border ${c.border} bg-zinc-900/50 p-5`}>
                <h2 className={`font-heading text-lg mb-4 ${c.text}`}>{sec.title}</h2>
                <dl className="space-y-3">
                  {sec.items.map(([term, def]) => (
                    <div key={term} className="grid grid-cols-1 sm:grid-cols-[160px_1fr] gap-1 sm:gap-4">
                      <dt className="font-mono text-sm text-zinc-200">{term}</dt>
                      <dd className="text-sm text-zinc-400 leading-relaxed">{def}</dd>
                    </div>
                  ))}
                </dl>
              </section>
            );
          })}
        </div>
      </div>
    </div>
  );
}
```

---

## File: `src/pages/InstallGuide.jsx`

```text
import React from "react";
import { Link } from "react-router-dom";
import { ArrowLeft, Terminal } from "lucide-react";
import CodeBlock from "@/components/forge/CodeBlock";
import { INSTALL_STEPS } from "@/components/forge/installSteps";

export default function InstallGuide() {
  return (
    <div className="min-h-screen bg-zinc-950 text-zinc-100">
      <div className="max-w-3xl mx-auto px-6 py-12">
        <Link to="/" className="inline-flex items-center gap-2 text-zinc-500 hover:text-amber-400 text-sm font-mono mb-8 transition-colors">
          <ArrowLeft className="h-4 w-4" /> Back to the board
        </Link>

        <header className="mb-10">
          <div className="flex items-center gap-3 mb-2">
            <Terminal className="h-6 w-6 text-amber-500" />
            <h1 className="font-heading text-3xl tracking-tight">
              Install Guide <span className="text-zinc-500 font-light">· Pop!_OS bare metal</span>
            </h1>
          </div>
          <p className="text-zinc-500 text-sm leading-relaxed">
            From green tests to a living resident process: environment, NPU wiring, kernel bootstrap,
            real-seat binding, and boot-on-startup. Copy each block in order. Bootstrap code snippets
            are templates — adapt import paths and signatures to your exact forge_ng code.
          </p>
        </header>

        <div className="space-y-10">
          {INSTALL_STEPS.map((step, i) => (
            <section key={i}>
              <div className="flex items-baseline gap-3 mb-2">
                <span className="font-mono text-amber-500 text-sm">{String(i + 1).padStart(2, "0")}</span>
                <h2 className="font-heading text-xl text-zinc-100">{step.title}</h2>
              </div>
              <p className="text-sm text-zinc-400 leading-relaxed mb-4 pl-8">{step.note}</p>
              <div className="space-y-3 pl-8">
                {step.blocks.map((b, j) => (
                  <CodeBlock key={j} code={b.code} lang={b.lang} />
                ))}
              </div>
            </section>
          ))}
        </div>

        <footer className="mt-14 border-t border-zinc-800 pt-6">
          <p className="text-xs font-mono text-zinc-600 leading-relaxed">
            Order matters: green tests (03) before boot (05), NPU visible (04) before real seat (06).
            If the NPU never shows up, the Forge still runs on HeuristicSeat — bonded, not fused.
          </p>
        </footer>
      </div>
    </div>
  );
}
```

---

## File: `src/pages/ControlDeck.jsx`

```text
import React, { useEffect, useState } from "react";
import { Link } from "react-router-dom";
import { base44 } from "@/api/base44Client";
import { ArrowLeft, Radio, Trash2 } from "lucide-react";
import NeonSlider from "@/components/deck/NeonSlider";
import NeonToggle from "@/components/deck/NeonToggle";
import NeonButton from "@/components/deck/NeonButton";
import AddControlDialog from "@/components/deck/AddControlDialog";

export default function ControlDeck() {
  const [controls, setControls] = useState(null);
  const [removeMode, setRemoveMode] = useState(false);

  const load = async () => setControls(await base44.entities.ForgeControl.list("created_date", 200));

  useEffect(() => {
    load();
    const unsubscribe = base44.entities.ForgeControl.subscribe((event) => {
      setControls((prev) => {
        if (!prev) return prev;
        if (event.type === "create") return prev.some((c) => c.id === event.data.id) ? prev : [...prev, event.data];
        if (event.type === "update") return prev.map((c) => (c.id === event.data.id ? event.data : c));
        if (event.type === "delete") return prev.filter((c) => c.id !== event.data.id);
        return prev;
      });
    });
    return unsubscribe;
  }, []);

  const setValue = async (control, value) => {
    setControls((prev) => prev.map((c) => (c.id === control.id ? { ...c, value } : c)));
    await base44.entities.ForgeControl.update(control.id, { value });
  };

  const create = async (data) => {
    await base44.entities.ForgeControl.create(data);
  };

  const remove = async (control) => {
    setControls((prev) => prev.filter((c) => c.id !== control.id));
    await base44.entities.ForgeControl.delete(control.id);
  };

  const sections = [...new Set((controls || []).map((c) => c.section || "Fabric"))];

  return (
    <div className="min-h-screen bg-zinc-950 text-zinc-100">
      <div className="max-w-6xl mx-auto px-6 py-12">
        <Link to="/" className="inline-flex items-center gap-2 text-zinc-500 hover:text-cyan-400 text-sm font-mono mb-8 transition-colors">
          <ArrowLeft className="h-4 w-4" /> Back to the board
        </Link>

        <header className="flex flex-wrap items-center justify-between gap-4 mb-10">
          <div>
            <div className="flex items-center gap-3 mb-1">
              <Radio className="h-6 w-6 text-cyan-400 animate-pulse" />
              <h1 className="font-heading text-3xl tracking-tight">
                Control Deck <span className="text-zinc-500 font-light">· live</span>
              </h1>
            </div>
            <p className="text-zinc-500 text-sm font-mono">
              Codeless operator console — every move syncs in real time. Your Forge reads this deck through the bridge.
            </p>
          </div>
          <div className="flex items-center gap-2">
            <button
              onClick={() => setRemoveMode((v) => !v)}
              className={`rounded-full border px-4 py-2 text-xs font-mono uppercase tracking-wider transition-colors ${
                removeMode ? "border-red-500/60 bg-red-500/10 text-red-400" : "border-zinc-800 text-zinc-500 hover:border-zinc-700"
              }`}
            >
              {removeMode ? "Done removing" : "Remove"}
            </button>
            <AddControlDialog onCreate={create} />
          </div>
        </header>

        {!controls ? (
          <div className="flex justify-center py-24">
            <div className="w-8 h-8 border-2 border-zinc-800 border-t-cyan-400 rounded-full animate-spin" />
          </div>
        ) : controls.length === 0 ? (
          <p className="text-zinc-600 text-center py-24 font-mono text-sm">Empty deck — snap on your first control.</p>
        ) : (
          <div className="space-y-10">
            {sections.map((sec) => (
              <div key={sec}>
                <h2 className="text-[11px] font-mono uppercase tracking-widest text-zinc-500 mb-4 border-b border-zinc-800/80 pb-2">
                  {sec}
                </h2>
                <div className="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-4">
                  {controls
                    .filter((c) => (c.section || "Fabric") === sec)
                    .map((c) => (
                      <div key={c.id} className="relative">
                        {removeMode && (
                          <button
                            onClick={() => remove(c)}
                            className="absolute -top-2 -right-2 z-10 rounded-full bg-red-600 p-1.5 text-white hover:bg-red-500"
                          >
                            <Trash2 className="h-3.5 w-3.5" />
                          </button>
                        )}
                        {c.kind === "slider" && <NeonSlider control={c} onChange={(v) => setValue(c, v)} />}
                        {c.kind === "toggle" && <NeonToggle control={c} onChange={(v) => setValue(c, v)} />}
                        {c.kind === "button" && <NeonButton control={c} onChange={(v) => setValue(c, v)} />}
                      </div>
                    ))}
                </div>
              </div>
            ))}
          </div>
        )}
      </div>
    </div>
  );
}
```

---

## File: `src/pages/ReviewBay.jsx`

```text
import React, { useEffect, useState } from "react";
import { Link } from "react-router-dom";
import { base44 } from "@/api/base44Client";
import { ArrowLeft, ScanSearch, Loader2 } from "lucide-react";
import DropZone from "@/components/review/DropZone";
import ReviewCard from "@/components/review/ReviewCard";
import { gradeFile } from "@/components/review/reviewGrader";

export default function ReviewBay() {
  const [reviews, setReviews] = useState(null);
  const [queue, setQueue] = useState([]);

  useEffect(() => {
    base44.entities.FileReview.list("-created_date", 100).then(setReviews);
  }, []);

  const handleFiles = async (files) => {
    setQueue(files.map((f) => f.name));
    for (const file of files) {
      const created = await gradeFile(file);
      setReviews((prev) => [created, ...(prev || [])]);
      setQueue((prev) => prev.filter((n) => n !== file.name));
    }
  };

  const handleDelete = async (review) => {
    setReviews((prev) => prev.filter((r) => r.id !== review.id));
    await base44.entities.FileReview.delete(review.id);
  };

  return (
    <div className="min-h-screen bg-zinc-950 text-zinc-100">
      <div className="max-w-3xl mx-auto px-6 py-12">
        <Link to="/" className="inline-flex items-center gap-2 text-zinc-500 hover:text-emerald-400 text-sm font-mono mb-8 transition-colors">
          <ArrowLeft className="h-4 w-4" /> Back to the board
        </Link>

        <header className="mb-8">
          <div className="flex items-center gap-3 mb-2">
            <ScanSearch className="h-6 w-6 text-emerald-400" />
            <h1 className="font-heading text-3xl tracking-tight">
              Review Bay <span className="text-zinc-500 font-light">· the once-over</span>
            </h1>
          </div>
          <p className="text-zinc-500 text-sm leading-relaxed">
            Drop any file and it gets the full rubric — code, structure, security, and install-readiness graded
            separately — plus a written review, integration how-tos, and preinstall issues caught before they bite.
          </p>
        </header>

        <DropZone onFiles={handleFiles} busy={queue.length > 0} />

        {queue.length > 0 && (
          <div className="mt-4 space-y-2">
            {queue.map((name) => (
              <div key={name} className="flex items-center gap-3 rounded-xl border border-zinc-800 bg-zinc-900/60 p-4">
                <Loader2 className="h-4 w-4 animate-spin text-emerald-400" />
                <span className="font-mono text-sm text-zinc-400">Grading {name}…</span>
              </div>
            ))}
          </div>
        )}

        <div className="mt-8 space-y-4">
          {reviews === null ? (
            <div className="flex justify-center py-16">
              <div className="w-8 h-8 border-2 border-zinc-800 border-t-emerald-400 rounded-full animate-spin" />
            </div>
          ) : reviews.length === 0 && queue.length === 0 ? (
            <p className="text-zinc-600 text-center py-16 font-mono text-sm">No reviews yet — drop the first file.</p>
          ) : (
            reviews.map((r) => <ReviewCard key={r.id} review={r} onDelete={handleDelete} />)
          )}
        </div>
      </div>
    </div>
  );
}
```

---

## File: `src/pages/PieceDetail.jsx`

```text
import React, { useState } from "react";
import { useParams, Link } from "react-router-dom";
import { useQuery, useMutation, useQueryClient } from "@tanstack/react-query";
import { base44 } from "@/api/base44Client";
import { ArrowLeft, Pencil, Code2, Lightbulb } from "lucide-react";
import { Button } from "@/components/ui/button";
import GradeBadge from "@/components/forge/GradeBadge";
import PieceEditForm from "@/components/forge/PieceEditForm";

const Section = ({ label, children, accent }) => (
  <div className="border-t border-zinc-800/80 pt-5">
    <h2 className="text-[11px] font-mono uppercase tracking-widest text-zinc-500 mb-2">{label}</h2>
    <p className={`leading-relaxed ${accent ? "text-amber-400 font-mono text-sm" : "text-zinc-300"}`}>{children}</p>
  </div>
);

export default function PieceDetail() {
  const { id } = useParams();
  const [editing, setEditing] = useState(false);
  const queryClient = useQueryClient();

  const { data: piece, isLoading } = useQuery({
    queryKey: ["forgePiece", id],
    queryFn: () => base44.entities.ForgePiece.get(id),
  });

  const mutation = useMutation({
    mutationFn: (form) =>
      base44.entities.ForgePiece.update(id, {
        name: form.name,
        grade: form.grade,
        what_it_is: form.what_it_is,
        serves: form.serves,
        gaps: form.gaps,
        next_brick: form.next_brick,
      }),
    onSuccess: () => {
      queryClient.invalidateQueries({ queryKey: ["forgePiece", id] });
      queryClient.invalidateQueries({ queryKey: ["forgePieces"] });
      setEditing(false);
    },
  });

  return (
    <div className="min-h-screen bg-zinc-950 text-zinc-100">
      <div className="max-w-3xl mx-auto px-6 py-12">
        <Link to="/" className="inline-flex items-center gap-2 text-zinc-500 hover:text-amber-400 text-sm font-mono mb-8 transition-colors">
          <ArrowLeft className="h-4 w-4" /> Back to the board
        </Link>

        {isLoading ? (
          <div className="flex justify-center py-24">
            <div className="w-8 h-8 border-2 border-zinc-800 border-t-amber-500 rounded-full animate-spin" />
          </div>
        ) : !piece ? (
          <p className="text-zinc-500 font-mono text-center py-24">Piece not found.</p>
        ) : editing ? (
          <PieceEditForm piece={piece} saving={mutation.isPending} onSave={(f) => mutation.mutate(f)} onCancel={() => setEditing(false)} />
        ) : (
          <div className="space-y-6">
            <div className="flex items-start justify-between gap-4">
              <div>
                <div className="flex items-center gap-2 text-zinc-500 mb-2">
                  <span className="font-mono text-xs">{String(piece.order || 0).padStart(2, "0")}</span>
                  {piece.piece_type === "Code" ? <Code2 className="h-4 w-4" /> : <Lightbulb className="h-4 w-4" />}
                  <span className="text-[11px] uppercase tracking-widest">{piece.piece_type}</span>
                </div>
                <h1 className="font-heading text-3xl md:text-4xl tracking-tight">{piece.name}</h1>
              </div>
              <div className="flex items-center gap-3 shrink-0 pt-1">
                <GradeBadge grade={piece.grade} />
                <Button size="icon" variant="ghost" onClick={() => setEditing(true)} className="text-zinc-500 hover:text-amber-400">
                  <Pencil className="h-4 w-4" />
                </Button>
              </div>
            </div>

            <Section label="What it is">{piece.what_it_is || "—"}</Section>
            <Section label="What part it serves">{piece.serves || "—"}</Section>
            <Section label="Weak spots / gaps">{piece.gaps || "—"}</Section>
            <Section label="Upgrade · next brick" accent>→ {piece.next_brick || "—"}</Section>
          </div>
        )}
      </div>
    </div>
  );
}
```

---

## File: `src/pages/Board.jsx`

```text
import React, { useState } from "react";
import { useQuery } from "@tanstack/react-query";
import { base44 } from "@/api/base44Client";
import { Flame, Terminal, Radio, BookOpen, ScanSearch, Cable } from "lucide-react";
import { Link } from "react-router-dom";
import PieceCard from "@/components/forge/PieceCard";
import { GRADES, GRADE_ORDER } from "@/components/forge/gradeConfig";
import BoardControlStrip from "@/components/deck/BoardControlStrip";

export default function Board() {
  const [filter, setFilter] = useState("ALL");
  const { data: pieces, isLoading } = useQuery({
    queryKey: ["forgePieces"],
    queryFn: () => base44.entities.ForgePiece.list("order", 100),
  });

  const list = (pieces || []).filter((p) => filter === "ALL" || p.grade === filter);
  const counts = (pieces || []).reduce((acc, p) => ({ ...acc, [p.grade]: (acc[p.grade] || 0) + 1 }), {});

  return (
    <div className="min-h-screen bg-background text-foreground">
      <div className="max-w-6xl mx-auto px-6 py-12">
        <div className="flex items-center gap-2 mb-6" aria-hidden="true">
          <div className="h-2 flex-1 rounded-full bg-primary/70" />
          <div className="h-2 w-16 rounded-full bg-accent/70" />
          <div className="h-2 w-8 rounded-full bg-primary/40" />
          <div className="h-2 w-4 rounded-full bg-accent/40" />
        </div>
        <header className="mb-10">
          <div className="flex items-center justify-between gap-4 mb-2">
            <div className="flex items-center gap-3">
              <Flame className="h-7 w-7 text-amber-500" />
              <h1 className="font-heading text-3xl md:text-4xl tracking-tight">
                THE FORGE <span className="text-amber-500">·</span>{" "}
                <span className="text-zinc-400 font-light">Command Board</span>
              </h1>
            </div>
            <div className="flex flex-wrap items-center gap-2 shrink-0">
              <Link
                to="/forge"
                className="inline-flex items-center gap-2 rounded-full border border-sky-500/40 bg-sky-500/10 px-4 py-1.5 text-xs font-mono uppercase tracking-wider text-sky-400 hover:bg-sky-500/20 transition-colors"
              >
                <Cable className="h-3.5 w-3.5" /> Forge Link
              </Link>
              <Link
                to="/deck"
                className="inline-flex items-center gap-2 rounded-full border border-cyan-500/40 bg-cyan-500/10 px-4 py-1.5 text-xs font-mono uppercase tracking-wider text-cyan-400 hover:bg-cyan-500/20 transition-colors"
              >
                <Radio className="h-3.5 w-3.5" /> Control Deck
              </Link>
              <Link
                to="/review"
                className="inline-flex items-center gap-2 rounded-full border border-emerald-500/40 bg-emerald-500/10 px-4 py-1.5 text-xs font-mono uppercase tracking-wider text-emerald-400 hover:bg-emerald-500/20 transition-colors"
              >
                <ScanSearch className="h-3.5 w-3.5" /> Review Bay
              </Link>
              <Link
                to="/cheatsheet"
                className="inline-flex items-center gap-2 rounded-full border border-fuchsia-500/40 bg-fuchsia-500/10 px-4 py-1.5 text-xs font-mono uppercase tracking-wider text-fuchsia-400 hover:bg-fuchsia-500/20 transition-colors"
              >
                <BookOpen className="h-3.5 w-3.5" /> Cheat Sheet
              </Link>
              <Link
                to="/install"
                className="inline-flex items-center gap-2 rounded-full border border-amber-500/40 bg-amber-500/10 px-4 py-1.5 text-xs font-mono uppercase tracking-wider text-amber-400 hover:bg-amber-500/20 transition-colors"
              >
                <Terminal className="h-3.5 w-3.5" /> Install Guide
              </Link>
            </div>
          </div>
          <p className="text-zinc-500 text-sm font-mono">
            {pieces?.length || 0} pieces on the board · every organ graded, nothing thrown away
          </p>
        </header>

        <div className="flex flex-wrap gap-2 mb-8">
          <button
            onClick={() => setFilter("ALL")}
            className={`rounded-full px-4 py-1.5 text-xs font-mono uppercase tracking-wider border transition-colors ${
              filter === "ALL"
                ? "border-amber-500/60 bg-amber-500/10 text-amber-400"
                : "border-zinc-800 text-zinc-500 hover:border-zinc-700"
            }`}
          >
            All
          </button>
          {GRADE_ORDER.map((gr) => {
            const g = GRADES[gr];
            return (
              <button
                key={gr}
                onClick={() => setFilter(filter === gr ? "ALL" : gr)}
                className={`rounded-full px-4 py-1.5 text-xs font-mono uppercase tracking-wider border transition-colors ${
                  filter === gr ? `${g.border} ${g.bg} ${g.text}` : "border-zinc-800 text-zinc-500 hover:border-zinc-700"
                }`}
              >
                {gr} {counts[gr] ? `· ${counts[gr]}` : ""}
              </button>
            );
          })}
        </div>

        <BoardControlStrip />

        {isLoading ? (
          <div className="flex justify-center py-24">
            <div className="w-8 h-8 border-2 border-zinc-800 border-t-amber-500 rounded-full animate-spin" />
          </div>
        ) : list.length === 0 ? (
          <p className="text-zinc-600 text-center py-24 font-mono text-sm">No pieces match this grade.</p>
        ) : (
          <div className="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-4">
            {list.map((p, i) => (
              <PieceCard key={p.id} piece={p} index={i} />
            ))}
          </div>
        )}
      </div>
    </div>
  );
}
```

---

## File: `src/pages/ForgeLink.jsx`

```text
import React, { useState } from "react";
import { Link } from "react-router-dom";
import { ArrowLeft, Cable, Settings } from "lucide-react";
import { Tabs, TabsList, TabsTrigger, TabsContent } from "@/components/ui/tabs";
import { isBridgeConfigured } from "@/lib/forgeBridge";
import BridgeSettings from "@/components/bridge/BridgeSettings";
import LiveFeed from "@/components/bridge/LiveFeed";
import HealthPanel from "@/components/bridge/HealthPanel";
import WrapsPanel from "@/components/bridge/WrapsPanel";
import LedgerPanel from "@/components/bridge/LedgerPanel";
import MintPanel from "@/components/bridge/MintPanel";
import ConcoctPanel from "@/components/bridge/ConcoctPanel";
import TroubleshootPanel from "@/components/bridge/TroubleshootPanel";
import ConnectionGuide from "@/components/bridge/ConnectionGuide";
import SocketDock from "@/components/sockets/SocketDock";

export default function ForgeLink() {
  const [showSettings, setShowSettings] = useState(!isBridgeConfigured());
  const [connKey, setConnKey] = useState(0);

  return (
    <div className="min-h-screen bg-zinc-950 text-zinc-100">
      <div className="max-w-6xl mx-auto px-6 py-12">
        <Link to="/" className="inline-flex items-center gap-2 text-zinc-500 hover:text-cyan-400 text-sm font-mono mb-8 transition-colors">
          <ArrowLeft className="h-4 w-4" /> Back to the board
        </Link>

        <header className="flex flex-wrap items-center justify-between gap-4 mb-6">
          <div>
            <div className="flex items-center gap-3 mb-1">
              <Cable className="h-6 w-6 text-cyan-400" />
              <h1 className="font-heading text-3xl tracking-tight">
                Forge Link <span className="text-zinc-500 font-light">· the glass</span>
              </h1>
            </div>
            <p className="text-zinc-500 text-sm font-mono">
              Read-only window into the Forge + gate-signed capability requests. No logic, no secrets held here.
            </p>
          </div>
          <button
            onClick={() => setShowSettings((v) => !v)}
            className="inline-flex items-center gap-2 rounded-full border border-zinc-800 px-4 py-1.5 text-xs font-mono uppercase tracking-wider text-zinc-400 hover:border-zinc-700 transition-colors"
          >
            <Settings className="h-3.5 w-3.5" /> Connection
          </button>
        </header>

        {showSettings && (
          <div className="mb-8 space-y-4">
            <BridgeSettings onSaved={() => { setShowSettings(false); setConnKey((k) => k + 1); }} />
            <ConnectionGuide />
          </div>
        )}

        <Tabs defaultValue="feed" key={connKey}>
          <TabsList className="bg-zinc-900 border border-zinc-800 mb-6">
            <TabsTrigger value="sockets">Sockets</TabsTrigger>
            <TabsTrigger value="feed">Live Feed</TabsTrigger>
            <TabsTrigger value="health">Health</TabsTrigger>
            <TabsTrigger value="wraps">Wraps</TabsTrigger>
            <TabsTrigger value="ledger">Ledger</TabsTrigger>
            <TabsTrigger value="mint">Mint</TabsTrigger>
            <TabsTrigger value="concoct">Concoct</TabsTrigger>
            <TabsTrigger value="tasks">Tasks</TabsTrigger>
          </TabsList>
          <TabsContent value="sockets"><SocketDock onBridged={() => setConnKey((k) => k + 1)} /></TabsContent>
          <TabsContent value="feed"><LiveFeed /></TabsContent>
          <TabsContent value="health"><HealthPanel /></TabsContent>
          <TabsContent value="wraps"><WrapsPanel /></TabsContent>
          <TabsContent value="ledger"><LedgerPanel /></TabsContent>
          <TabsContent value="mint"><MintPanel /></TabsContent>
          <TabsContent value="concoct"><ConcoctPanel /></TabsContent>
          <TabsContent value="tasks"><TroubleshootPanel /></TabsContent>
        </Tabs>
      </div>
    </div>
  );
}
```

---

## File: `src/hooks/use-mobile.jsx`

```text
import * as React from "react"

const MOBILE_BREAKPOINT = 768

export function useIsMobile() {
  const [isMobile, setIsMobile] = React.useState(undefined)

  React.useEffect(() => {
    const mql = window.matchMedia(`(max-width: ${MOBILE_BREAKPOINT - 1}px)`)
    const onChange = () => {
      setIsMobile(window.innerWidth < MOBILE_BREAKPOINT)
    }
    mql.addEventListener("change", onChange)
    setIsMobile(window.innerWidth < MOBILE_BREAKPOINT)
    return () => mql.removeEventListener("change", onChange);
  }, [])

  return !!isMobile
}

```

---

## File: `src/hooks/use-size.jsx`

```text
import * as React from "react"

export function useSize(ref) {
  const [size, setSize] = React.useState(null)

  // useLayoutEffect (not useEffect): the initial measurement must land before
  // the browser paints, so consumers can render their real content on the
  // very first painted frame instead of a guess. A ResizeObserver's first
  // callback arrives too late for that — by then an <img> src guess has
  // already been dispatched to the network.
  React.useLayoutEffect(() => {
    const element = ref.current
    if (!element) return

    const rect = element.getBoundingClientRect()
    setSize({ width: rect.width, height: rect.height })

    const observer = new ResizeObserver(([entry]) => {
      const { width, height } = entry.contentRect
      setSize({ width, height })
    })

    observer.observe(element)
    return () => observer.disconnect()
  }, [ref])

  return size
}

```

---

## File: `src/api/base44Client.js`

```text
import { createClient } from '@base44/sdk';
import { appParams } from '@/lib/app-params';

const { appId, token, functionsVersion, appBaseUrl } = appParams;

//Create a client with authentication required
export const base44 = createClient({
  appId,
  token,
  functionsVersion,
  serverUrl: '',
  requiresAuth: false,
  appBaseUrl
});

```

---

## File: `src/lib/PageNotFound.jsx`

```text
import { useLocation } from 'react-router-dom';
import { base44 } from '@/api/base44Client';
import { useQuery } from '@tanstack/react-query';


export default function PageNotFound({}) {
    const location = useLocation();
    const pageName = location.pathname.substring(1);

    const { data: authData, isFetched } = useQuery({
        queryKey: ['user'],
        queryFn: async () => {
            try {
                const user = await base44.auth.me();
                return { user, isAuthenticated: true };
            } catch (error) {
                return { user: null, isAuthenticated: false };
            }
        }
    });
    
    return (
        <div className="min-h-screen flex items-center justify-center p-6 bg-slate-50">
            <div className="max-w-md w-full">
                <div className="text-center space-y-6">
                    {/* 404 Error Code */}
                    <div className="space-y-2">
                        <h1 className="text-7xl font-light text-slate-300">404</h1>
                        <div className="h-0.5 w-16 bg-slate-200 mx-auto"></div>
                    </div>
                    
                    {/* Main Message */}
                    <div className="space-y-3">
                        <h2 className="text-2xl font-medium text-slate-800">
                            Page Not Found
                        </h2>
                        <p className="text-slate-600 leading-relaxed">
                            The page <span className="font-medium text-slate-700">"{pageName}"</span> could not be found in this application.
                        </p>
                    </div>
                    
                    {/* Admin Note */}
                    {isFetched && authData.isAuthenticated && authData.user?.role === 'admin' && (
                        <div className="mt-8 p-4 bg-slate-100 rounded-lg border border-slate-200">
                            <div className="flex items-start space-x-3">
                                <div className="flex-shrink-0 w-5 h-5 rounded-full bg-orange-100 flex items-center justify-center mt-0.5">
                                    <div className="w-2 h-2 rounded-full bg-orange-400"></div>
                                </div>
                                <div className="text-left space-y-1">
                                    <p className="text-sm font-medium text-slate-700">Admin Note</p>
                                    <p className="text-sm text-slate-600 leading-relaxed">
                                        This could mean that the AI hasn't implemented this page yet. Ask it to implement it in the chat.
                                    </p>
                                </div>
                            </div>
                        </div>
                    )}
                    
                    {/* Action Button */}
                    <div className="pt-6">
                        <button 
                            onClick={() => window.location.href = '/'} 
                            className="inline-flex items-center px-4 py-2 text-sm font-medium text-slate-700 bg-white border border-slate-200 rounded-lg hover:bg-slate-50 hover:border-slate-300 transition-colors duration-200 focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-slate-500"
                        >
                            <svg className="w-4 h-4 mr-2" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                                <path strokeLinecap="round" strokeLinejoin="round" strokeWidth={2} d="M3 12l2-2m0 0l7-7 7 7M5 10v10a1 1 0 001 1h3m10-11l2 2m-2-2v10a1 1 0 01-1 1h-3m-6 0a1 1 0 001-1v-4a1 1 0 011-1h2a1 1 0 011 1v4a1 1 0 001 1m-6 0h6" />
                            </svg>
                            Go Home
                        </button>
                    </div>
                </div>
            </div>
        </div>
    )
}
```

---

## File: `src/lib/app-params.js`

```text
const isNode = typeof window === 'undefined';
const windowObj = isNode ? { localStorage: new Map() } : window;
const storage = windowObj.localStorage;

const toSnakeCase = (str) => {
	return str.replace(/([A-Z])/g, '_$1').toLowerCase();
}

const getAppParamValue = (paramName, { defaultValue = undefined, removeFromUrl = false } = {}) => {
	if (isNode) {
		return defaultValue;
	}
	const storageKey = `base44_${toSnakeCase(paramName)}`;
	const urlParams = new URLSearchParams(window.location.search);
	const searchParam = urlParams.get(paramName);
	if (removeFromUrl) {
		urlParams.delete(paramName);
		const newUrl = `${window.location.pathname}${urlParams.toString() ? `?${urlParams.toString()}` : ""
			}${window.location.hash}`;
		window.history.replaceState({}, document.title, newUrl);
	}
	if (searchParam) {
		storage.setItem(storageKey, searchParam);
		return searchParam;
	}
	if (defaultValue) {
		storage.setItem(storageKey, defaultValue);
		return defaultValue;
	}
	const storedValue = storage.getItem(storageKey);
	if (storedValue) {
		return storedValue;
	}
	return null;
}

const getAppParams = () => {
	if (getAppParamValue("clear_access_token") === 'true') {
		storage.removeItem('base44_access_token');
		storage.removeItem('token');
	}
	return {
		appId: getAppParamValue("app_id", { defaultValue: import.meta.env.VITE_BASE44_APP_ID }),
		token: getAppParamValue("access_token", { removeFromUrl: true }),
		fromUrl: getAppParamValue("from_url", { defaultValue: window.location.href }),
		functionsVersion: getAppParamValue("functions_version", { defaultValue: import.meta.env.VITE_BASE44_FUNCTIONS_VERSION }),
		appBaseUrl: getAppParamValue("app_base_url", { defaultValue: import.meta.env.VITE_BASE44_APP_BASE_URL }),
	}
}


export const appParams = {
	...getAppParams()
}

```

---

## File: `src/lib/forgeBridge.js`

```text
const KEY = "forge_bridge_config";

export const getBridgeConfig = () => {
  try {
    return JSON.parse(localStorage.getItem(KEY)) || { url: "", token: "", cfId: "", cfSecret: "" };
  } catch {
    return { url: "", token: "", cfId: "", cfSecret: "" };
  }
};

export const saveBridgeConfig = (cfg) => localStorage.setItem(KEY, JSON.stringify(cfg));

export const isBridgeConfigured = () => Boolean(getBridgeConfig().url);

const authHeaders = () => {
  const { token, cfId, cfSecret } = getBridgeConfig();
  return {
    ...(token ? { Authorization: `Bearer ${token}` } : {}),
    ...(cfId ? { "CF-Access-Client-Id": cfId } : {}),
    ...(cfSecret ? { "CF-Access-Client-Secret": cfSecret } : {}),
  };
};

export const bridgeFetch = async (path, options = {}) => {
  const { url } = getBridgeConfig();
  if (!url) throw new Error("Bridge not configured — set your Forge URL in settings.");
  const res = await fetch(url.replace(/\/$/, "") + path, {
    ...options,
    headers: {
      "Content-Type": "application/json",
      ...authHeaders(),
      ...(options.headers || {}),
    },
  });
  if (!res.ok) throw new Error(`Bridge ${res.status}: ${await res.text()}`);
  return res.json();
};

// SSE over fetch — EventSource can't carry the Cloudflare Access headers, a fetch stream can.
// Returns an abort function.
export const openFeed = (onEvent, onStatus) => {
  const { url } = getBridgeConfig();
  if (!url) {
    onStatus("unconfigured");
    return () => {};
  }
  const controller = new AbortController();
  (async () => {
    try {
      const res = await fetch(url.replace(/\/$/, "") + "/feed", {
        headers: authHeaders(),
        signal: controller.signal,
      });
      if (!res.ok || !res.body) {
        onStatus("disconnected");
        return;
      }
      onStatus("live");
      const reader = res.body.getReader();
      const decoder = new TextDecoder();
      let buffer = "";
      while (true) {
        const { done, value } = await reader.read();
        if (done) break;
        buffer += decoder.decode(value, { stream: true });
        const chunks = buffer.split("\n\n");
        buffer = chunks.pop();
        for (const chunk of chunks) {
          const line = chunk.split("\n").find((l) => l.startsWith("data: "));
          if (line) onEvent(line.slice(6));
        }
      }
      onStatus("disconnected");
    } catch (e) {
      if (e.name !== "AbortError") onStatus("disconnected");
    }
  })();
  return () => controller.abort();
};
```

---

## File: `src/lib/connectionVault.js`

```text
// Secrets keychain — tokens live ONLY in this browser (localStorage), never in the database.
const KEY = "forge_conn_vault";

const readVault = () => {
  try { return JSON.parse(localStorage.getItem(KEY)) || {}; } catch { return {}; }
};

export function getConnSecrets(id) {
  return readVault()[id] || { token: "", cfId: "", cfSecret: "" };
}

export function saveConnSecrets(id, secrets) {
  const vault = readVault();
  vault[id] = secrets;
  localStorage.setItem(KEY, JSON.stringify(vault));
}

export function deleteConnSecrets(id) {
  const vault = readVault();
  delete vault[id];
  localStorage.setItem(KEY, JSON.stringify(vault));
}

export function hasConnSecrets(id) {
  const s = readVault()[id];
  return !!(s && (s.token || s.cfSecret));
}
```

---

## File: `src/lib/utils.js`

```text
import { clsx } from "clsx"
import { twMerge } from "tailwind-merge"

export function cn(...inputs) {
  return twMerge(clsx(inputs))
} 


export const isIframe = window.self !== window.top;

```

---

## File: `src/lib/query-client.js`

```text
import { QueryClient } from '@tanstack/react-query';


export const queryClientInstance = new QueryClient({
	defaultOptions: {
		queries: {
			refetchOnWindowFocus: false,
			retry: 1,
		},
	},
});
```

---

## File: `src/lib/AuthContext.jsx`

```text
import React, { createContext, useState, useContext, useEffect } from 'react';
import { base44 } from '@/api/base44Client';
import { appParams } from '@/lib/app-params';
import { createAxiosClient } from '@base44/sdk/dist/utils/axios-client';

const AuthContext = createContext();

export const AuthProvider = ({ children }) => {
  const [user, setUser] = useState(null);
  const [isAuthenticated, setIsAuthenticated] = useState(false);
  const [isLoadingAuth, setIsLoadingAuth] = useState(true);
  const [isLoadingPublicSettings, setIsLoadingPublicSettings] = useState(true);
  const [authError, setAuthError] = useState(null);
  const [authChecked, setAuthChecked] = useState(false);
  const [appPublicSettings, setAppPublicSettings] = useState(null); // Contains only { id, public_settings }

  useEffect(() => {
    checkAppState();
  }, []);

  const checkAppState = async () => {
    try {
      setIsLoadingPublicSettings(true);
      setAuthError(null);
      
      // First, check app public settings (with token if available)
      // This will tell us if auth is required, user not registered, etc.
      const appClient = createAxiosClient({
        baseURL: `/api/apps/public`,
        headers: {
          'X-App-Id': appParams.appId
        },
        token: appParams.token, // Include token if available
        interceptResponses: true
      });
      
      try {
        const publicSettings = await appClient.get(`/prod/public-settings/by-id/${appParams.appId}`);
        setAppPublicSettings(publicSettings);
        
        // If we got the app public settings successfully, check if user is authenticated
        if (appParams.token) {
          await checkUserAuth();
        } else {
          setIsLoadingAuth(false);
          setIsAuthenticated(false);
          setAuthChecked(true);
        }
        setIsLoadingPublicSettings(false);
      } catch (appError) {
        console.error('App state check failed:', appError);
        
        // Handle app-level errors
        if (appError.status === 403 && appError.data?.extra_data?.reason) {
          const reason = appError.data.extra_data.reason;
          if (reason === 'auth_required') {
            setAuthError({
              type: 'auth_required',
              message: 'Authentication required'
            });
          } else if (reason === 'user_not_registered') {
            setAuthError({
              type: 'user_not_registered',
              message: 'User not registered for this app'
            });
          } else {
            setAuthError({
              type: reason,
              message: appError.message
            });
          }
        } else {
          setAuthError({
            type: 'unknown',
            message: appError.message || 'Failed to load app'
          });
        }
        setIsLoadingPublicSettings(false);
        setIsLoadingAuth(false);
      }
    } catch (error) {
      console.error('Unexpected error:', error);
      setAuthError({
        type: 'unknown',
        message: error.message || 'An unexpected error occurred'
      });
      setIsLoadingPublicSettings(false);
      setIsLoadingAuth(false);
    }
  };

  const checkUserAuth = async () => {
    try {
      // Now check if the user is authenticated
      setIsLoadingAuth(true);
      const currentUser = await base44.auth.me();
      setUser(currentUser);
      setIsAuthenticated(true);
      setIsLoadingAuth(false);
      setAuthChecked(true);
    } catch (error) {
      console.error('User auth check failed:', error);
      setIsLoadingAuth(false);
      setIsAuthenticated(false);
      setAuthChecked(true);
      
      // If user auth fails, it might be an expired token
      if (error.status === 401 || error.status === 403) {
        setAuthError({
          type: 'auth_required',
          message: 'Authentication required'
        });
      }
    }
  };

  const logout = (shouldRedirect = true) => {
    setUser(null);
    setIsAuthenticated(false);
    
    if (shouldRedirect) {
      // Use the SDK's logout method which handles token cleanup and redirect
      base44.auth.logout(window.location.href);
    } else {
      // Just remove the token without redirect
      base44.auth.logout();
    }
  };

  const navigateToLogin = () => {
    // Use the SDK's redirectToLogin method
    base44.auth.redirectToLogin(window.location.href);
  };

  return (
    <AuthContext.Provider value={{ 
      user, 
      isAuthenticated, 
      isLoadingAuth,
      isLoadingPublicSettings,
      authError,
      appPublicSettings,
      authChecked,
      logout,
      navigateToLogin,
      checkUserAuth,
      checkAppState
    }}>
      {children}
    </AuthContext.Provider>
  );
};

export const useAuth = () => {
  const context = useContext(AuthContext);
  if (!context) {
    throw new Error('useAuth must be used within an AuthProvider');
  }
  return context;
};

```

---

## File: `src/utils/index.ts`

```text
export function createPageUrl(pageName: string) {
    return '/' + pageName.replace(/ /g, '-');
}
```

---

## File: `base44/config.jsonc`

```text
{
  "name": "untitled",
  "site": {
    "installCommand": "npm install",
    "buildCommand": "npm run build",
    "serveCommand": "npm run dev",
    "outputDirectory": "./dist"
  }
}
```

---

## File: `base44/connectors/github.jsonc`

```text
{
  "type": "github",
  "scopes": [
    "repo"
  ]
}
```

---

## File: `base44/connectors/googleslides.jsonc`

```text
{
  "type": "googleslides",
  "scopes": [
    "https://www.googleapis.com/auth/presentations",
    "email"
  ]
}
```

---

## File: `base44/connectors/googledocs.jsonc`

```text
{
  "type": "googledocs",
  "scopes": [
    "https://www.googleapis.com/auth/documents",
    "email"
  ]
}
```

---

## File: `base44/connectors/googlesheets.jsonc`

```text
{
  "type": "googlesheets",
  "scopes": [
    "https://www.googleapis.com/auth/spreadsheets",
    "email"
  ]
}
```

---

## File: `base44/connectors/hugging_face.jsonc`

```text
{
  "type": "hugging_face",
  "scopes": [
    "inference-api"
  ]
}
```

---

## File: `base44/connectors/googledrive.jsonc`

```text
{
  "type": "googledrive",
  "scopes": [
    "https://www.googleapis.com/auth/drive.readonly",
    "email"
  ]
}
```

---

## File: `base44/entities/ConnectionEvent.jsonc`

```text
{
  "name": "ConnectionEvent",
  "type": "object",
  "properties": {
    "connection_id": {
      "type": "string"
    },
    "connection_name": {
      "type": "string"
    },
    "kind": {
      "type": "string"
    },
    "status": {
      "type": "string",
      "enum": [
        "ok",
        "fail"
      ],
      "default": "ok"
    },
    "detail": {
      "type": "string"
    }
  },
  "required": [
    "connection_name",
    "status"
  ]
}
```

---

## File: `base44/entities/FileReview.jsonc`

```text
{
  "name": "FileReview",
  "type": "object",
  "properties": {
    "file_name": {
      "type": "string"
    },
    "overall_grade": {
      "type": "string",
      "enum": [
        "GREEN",
        "YELLOW",
        "RED",
        "PURPLE",
        "ORANGE"
      ],
      "default": "YELLOW"
    },
    "code_grade": {
      "type": "string",
      "enum": [
        "GREEN",
        "YELLOW",
        "RED",
        "PURPLE",
        "ORANGE"
      ]
    },
    "structure_grade": {
      "type": "string",
      "enum": [
        "GREEN",
        "YELLOW",
        "RED",
        "PURPLE",
        "ORANGE"
      ]
    },
    "security_grade": {
      "type": "string",
      "enum": [
        "GREEN",
        "YELLOW",
        "RED",
        "PURPLE",
        "ORANGE"
      ]
    },
    "install_grade": {
      "type": "string",
      "enum": [
        "GREEN",
        "YELLOW",
        "RED",
        "PURPLE",
        "ORANGE"
      ]
    },
    "summary": {
      "type": "string"
    },
    "review": {
      "type": "string"
    },
    "how_tos": {
      "type": "array",
      "items": {
        "type": "string"
      }
    },
    "preinstall_issues": {
      "type": "array",
      "items": {
        "type": "string"
      }
    },
    "next_bricks": {
      "type": "array",
      "items": {
        "type": "string"
      }
    }
  },
  "required": [
    "file_name"
  ]
}
```

---

## File: `base44/entities/User.jsonc`

```text
{
  "properties": {
    "role": {
      "type": "string",
      "description": "The role of the user in the app",
      "enum": [
        "admin",
        "user"
      ]
    }
  },
  "required": [
    "role"
  ],
  "name": "User",
  "type": "object"
}
```

---

## File: `base44/entities/ForgeTask.jsonc`

```text
{
  "name": "ForgeTask",
  "type": "object",
  "properties": {
    "title": {
      "type": "string"
    },
    "detail": {
      "type": "string"
    },
    "source": {
      "type": "string",
      "description": "What triggered this task (e.g. bridge offline, section fault)"
    },
    "status": {
      "type": "string",
      "enum": [
        "open",
        "done"
      ],
      "default": "open"
    }
  },
  "required": [
    "title"
  ]
}
```

---

## File: `base44/entities/ForgeControl.jsonc`

```text
{
  "name": "ForgeControl",
  "type": "object",
  "properties": {
    "name": {
      "type": "string"
    },
    "kind": {
      "type": "string",
      "enum": [
        "slider",
        "toggle",
        "button"
      ],
      "default": "toggle"
    },
    "section": {
      "type": "string",
      "default": "Fabric"
    },
    "color": {
      "type": "string",
      "enum": [
        "cyan",
        "magenta",
        "amber",
        "green",
        "violet"
      ],
      "default": "cyan"
    },
    "value": {
      "type": "number",
      "default": 0
    },
    "min": {
      "type": "number",
      "default": 0
    },
    "max": {
      "type": "number",
      "default": 100
    },
    "step": {
      "type": "number",
      "default": 1
    },
    "description": {
      "type": "string"
    }
  },
  "required": [
    "name",
    "kind"
  ]
}
```

---

## File: `base44/entities/ForgePiece.jsonc`

```text
{
  "name": "ForgePiece",
  "type": "object",
  "properties": {
    "order": {
      "type": "number"
    },
    "name": {
      "type": "string"
    },
    "piece_type": {
      "type": "string",
      "enum": [
        "Code",
        "Concept"
      ],
      "default": "Concept"
    },
    "grade": {
      "type": "string",
      "enum": [
        "GREEN",
        "YELLOW",
        "RED",
        "PURPLE",
        "ORANGE"
      ],
      "default": "YELLOW"
    },
    "what_it_is": {
      "type": "string"
    },
    "serves": {
      "type": "string"
    },
    "gaps": {
      "type": "string"
    },
    "next_brick": {
      "type": "string"
    }
  },
  "required": [
    "name"
  ]
}
```

---

## File: `base44/entities/BridgeConnection.jsonc`

```text
{
  "name": "BridgeConnection",
  "type": "object",
  "properties": {
    "name": {
      "type": "string"
    },
    "kind": {
      "type": "string",
      "enum": [
        "wsl",
        "forge",
        "github",
        "cloudflare",
        "gpu",
        "database",
        "custom"
      ],
      "default": "custom"
    },
    "url": {
      "type": "string"
    },
    "notes": {
      "type": "string"
    },
    "pinned": {
      "type": "boolean",
      "default": false
    },
    "approved": {
      "type": "boolean",
      "default": true
    },
    "last_status": {
      "type": "string",
      "enum": [
        "ok",
        "fail",
        "unknown"
      ],
      "default": "unknown"
    },
    "last_connected": {
      "type": "string"
    },
    "times_connected": {
      "type": "number",
      "default": 0
    }
  },
  "required": [
    "name"
  ]
}
```