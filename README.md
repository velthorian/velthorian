<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0d1117,35:0a0e1a,65:0d1421,100:0d1117&height=160&section=header&text=VELTHORIAN&fontSize=40&fontFamily=JetBrains+Mono&fontColor=4A7FBF&fontAlignY=58&animation=fadeIn&desc=software+engineer+%2F+self-hosted+infrastructure&descSize=12&descAlignY=75&descAlign=50&descColor=3a5a7a" width="100%"/>

<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=300&size=12&duration=3500&pause=1200&color=4A7FBF&center=true&vCenter=true&width=580&lines=Full-stack+developer+%E2%80%94+Node.js+%2F+React+19;Self-hosted+infra+%E2%80%94+multi-VPS+%2B+dedicated+%2B+RPi+%2B+Arduino;Discord+bots+%2F+streaming+%2F+file+sharing+%2F+ops;Building+things+that+actually+work." />

<br/>

![](https://img.shields.io/badge/Self--hosted-0d1421?style=flat-square&logo=raspberry-pi&logoColor=4A7FBF&labelColor=0d1421)
![](https://img.shields.io/badge/Node.js_ESM-0d1421?style=flat-square&logo=node.js&logoColor=4A7FBF&labelColor=0d1421)
![](https://img.shields.io/badge/Nginx_·_Cloudflare-0d1421?style=flat-square&logo=nginx&logoColor=4A7FBF&labelColor=0d1421)
![](https://img.shields.io/badge/Always_shipping-0d1421?style=flat-square&logo=github-actions&logoColor=4A7FBF&labelColor=0d1421)
![](https://img.shields.io/badge/PM2_·_Docker-0d1421?style=flat-square&logo=docker&logoColor=4A7FBF&labelColor=0d1421)

</div>

<br/>

---

## `~/ecosystem`

> Services web self-hostés interconnectés — déployés derrière Nginx + Cloudflare sur une infrastructure multi-machines.

<br/>

<table>
<thead>
<tr>
<th align="left" width="195">Projet</th>
<th align="left">Description</th>
<th align="left">Stack</th>
<th align="center">Status</th>
</tr>
</thead>
<tbody>
<tr>
<td><strong>VelthorianFlix</strong></td>
<td>Plateforme de streaming vidéo privée — bibliothèque SQLite, metadata TMDB, range-request streaming, watch history, transcoding GPU externe, panel admin</td>
<td><code>React 19</code> <code>Vite</code> <code>Express</code> <code>SQLite</code> <code>JWT</code></td>
<td align="center"><img src="https://img.shields.io/badge/●_actif-0a3d1f?style=flat-square&labelColor=0a3d1f&color=0a3d1f&logoColor=4ade80"/></td>
</tr>
<tr>
<td><strong>VelthorianDrop</strong></td>
<td>Partage de fichiers sécurisé — drag & drop XHR, tokens JWT one-shot, SHA-256, expiry / password / limite de téléchargements, panel admin</td>
<td><code>Node.js</code> <code>Express</code> <code>JWT</code> <code>SQLite</code></td>
<td align="center"><img src="https://img.shields.io/badge/●_actif-0a3d1f?style=flat-square&labelColor=0a3d1f&color=0a3d1f"/></td>
</tr>
<tr>
<td><strong>VelthorianPulse</strong></td>
<td>Page de statut publique — health checks HTTP, historique 90 jours, gestion d'incidents, alertes Discord webhook</td>
<td><code>Node.js</code> <code>Express</code> <code>SQLite</code> <code>Discord</code></td>
<td align="center"><img src="https://img.shields.io/badge/●_actif-0a3d1f?style=flat-square&labelColor=0a3d1f&color=0a3d1f"/></td>
</tr>
<tr>
<td><strong>VelthorianOps</strong></td>
<td>Dashboard opérationnel unifié — analytics Cloudflare (GraphQL), monitoring PM2 avec stream SSE, cron manager SQLite, alertes Discord</td>
<td><code>React 19</code> <code>Vite</code> <code>Express</code> <code>PM2 API</code> <code>SQLite</code></td>
<td align="center"><img src="https://img.shields.io/badge/●_actif-0a3d1f?style=flat-square&labelColor=0a3d1f&color=0a3d1f"/></td>
</tr>
<tr>
<td><strong>VelthorianGate</strong></td>
<td>Portail d'authentification centralisé — SSO, gestion de projets, tableau de bord admin</td>
<td><code>Node.js</code> <code>JWT</code> <code>bcrypt</code> <code>SQLite</code></td>
<td align="center"><img src="https://img.shields.io/badge/●_en_dev-3d2000?style=flat-square&labelColor=3d2000&color=3d2000"/></td>
</tr>
<tr>
<td><strong>VelthorianRythm</strong></td>
<td>Bot Discord de musique — slash commands, Lavalink v4, 9 filtres audio, playlists SQLite persistées, site compagnon</td>
<td><code>Discord.js v14</code> <code>Lavalink v4</code> <code>Node.js</code> <code>SQLite</code></td>
<td align="center"><img src="https://img.shields.io/badge/●_actif-0a3d1f?style=flat-square&labelColor=0a3d1f&color=0a3d1f"/></td>
</tr>
<tr>
<td><strong>Portfolio</strong></td>
<td>Site personnel — scroll reveals, mouse-tracking spotlight, count-up stats, scroll-stack showcase, design system cohérent</td>
<td><code>HTML</code> <code>CSS</code> <code>JS</code> <code>Nginx</code></td>
<td align="center"><img src="https://img.shields.io/badge/●_actif-0a3d1f?style=flat-square&labelColor=0a3d1f&color=0a3d1f"/></td>
</tr>
</tbody>
</table>

<br/>

---

## `~/architecture`

```
                              INTERNET
                                  │
                    ┌─────────────▼─────────────┐
                    │         CLOUDFLARE         │
                    │  CDN · WAF · DNS · DDoS    │
                    │  TLS 1.3 · Bot protection  │
                    └─────────────┬─────────────┘
                                  │
╔═════════════════════════════════▼═════════════════════════════════╗
║                                                                   ║
║   ░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░   ║
║   ░░                    B L A C K   B O X                  ░░   ║
║   ░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░   ║
║                                                                   ║
║  ┌────────────────────────────────────────────────────────────┐  ║
║  │              Nginx  —  reverse proxy layer                 │  ║
║  │       SSL termination · rate limiting · static cache       │  ║
║  └──┬──────┬──────┬──────┬──────┬──────┬──────┬─────┬───────┘  ║
║     │      │      │      │      │      │      │     │           ║
║     ▼      ▼      ▼      ▼      ▼      ▼      ▼     ▼           ║
║  [Flix] [Drop] [Gate] [Pulse] [Ops] [Rythm]  ···   ···          ║
║  Node   Node   Node   Node    Node   Node    bots  static       ║
║     │      │      │      │      │      │                        ║
║     └──────┴──────┴──────┴──────┴──────┘                        ║
║                          │                                       ║
║                   ┌──────▼───────┐   ┌──────────────┐           ║
║                   │    SQLite    │   │  File storage │           ║
║                   │  per-service │   │  (Drop/Flix)  │           ║
║                   └─────────────┘   └──────────────┘           ║
║                                                                   ║
║  ┌─────────────────────────────────────────────────────────────┐ ║
║  │                      compute mesh                           │ ║
║  │                                                             │ ║
║  │  ┌──────────────┐  ┌──────────────┐  ┌───────────────────┐ │ ║
║  │  │    VPS × n   │  │    Dédié     │  │    RPi cluster    │ │ ║
║  │  │   Debian 12  │  │  (home lab)  │  │                   │ │ ║
║  │  │   cloud      │  │  bare metal  │  │  ┌───┐  ┌───┐     │ │ ║
║  │  │   ×n nodes   │  │  24/7 uptime │  │  │Pi5│  │Pi │     │ │ ║
║  │  └──────────────┘  └──────────────┘  │  └───┘  └───┘     │ │ ║
║  │                                       │         ···        │ │ ║
║  │                                       └────────────┬───────┘ │ ║
║  └────────────────────────────────────────────────────┼─────────┘ ║
║                                                       │           ║
║                                          ┌────────────▼─────────┐ ║
║                                          │      Arduino × n     │ ║
║                                          │  GPIO · I²C · UART   │ ║
║                                          │  sensors · actuators │ ║
║                                          └─────────────────────┘ ║
║                                                                   ║
║  ┌─────────────────────────────────────────────────────────────┐ ║
║  │  Discord layer                                              │ ║
║  │  [music bot] ── [trading bot] ── [monitor] ── [webhooks]   │ ║
║  │  Components V2 · slash commands · Canvas · SQLite           │ ║
║  └─────────────────────────────────────────────────────────────┘ ║
║                                                                   ║
╚═══════════════════════════════════════════════════════════════════╝
```

<br/>

---

## `~/stack`

<div align="center">

<img src="https://skillicons.dev/icons?i=js,ts,react,vite,nodejs,express,sqlite,docker,nginx,linux,bash,raspberrypi,git,discord,vscode&theme=dark&perline=8" />

</div>

<br/>

<table width="100%">
<tr>
<td valign="top" width="25%">

**Frontend**
```
React 19 · Vite 5
HTML · CSS · JS
Recharts · Canvas
```

</td>
<td valign="top" width="25%">

**Backend**
```
Node.js ESM · Express
better-sqlite3 · JWT
bcrypt · node-cron
```

</td>
<td valign="top" width="25%">

**Infra / Ops**
```
Nginx · Cloudflare
PM2 · Docker
Lavalink v4
```

</td>
<td valign="top" width="25%">

**Embedded**
```
Raspberry Pi OS
Arduino · GPIO
I²C · UART · USB
```

</td>
</tr>
</table>

<br/>

---

## `~/stats`

<div align="center">

<img height="155" src="https://github-readme-stats.vercel.app/api?username=Velthorian&show_icons=true&theme=transparent&hide_border=true&title_color=4A7FBF&icon_color=4A7FBF&text_color=6e8098&bg_color=0d1117&rank_icon=github&include_all_commits=true" />
&nbsp;
<img height="155" src="https://github-readme-stats.vercel.app/api/top-langs/?username=Velthorian&layout=compact&theme=transparent&hide_border=true&title_color=4A7FBF&text_color=6e8098&bg_color=0d1117&langs_count=6&hide=html,css" />

</div>

<br/>

---

<div align="center">

<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=200&size=10&duration=5000&pause=3000&color=1d3a5c&center=true&vCenter=true&width=500&lines=//+everything+runs+somewhere+you+can't+see" />

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0d1117,35:0a0e1a,65:0d1421,100:0d1117&height=100&section=footer" width="100%"/>

</div>
