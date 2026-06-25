<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0d1117,40:0d1421,80:111827,100:0d1117&height=150&section=header&text=VELTHORIAN&fontSize=36&fontFamily=JetBrains+Mono&fontColor=4A7FBF&fontAlignY=58&animation=fadeIn" width="100%"/>

<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=300&size=13&duration=3500&pause=1200&color=4A7FBF&center=true&vCenter=true&width=560&lines=Full-stack+developer+%E2%80%94+Node.js+%2F+React+19;Self-hosted+infrastructure+%E2%80%94+Raspberry+Pi+%2B+VPS;Discord+bots+%2F+streaming+%2F+file+sharing+%2F+ops;Building+things+that+actually+work." alt="Typing SVG" />

<br/>

![](https://img.shields.io/badge/Self--hosted-0d1421?style=flat-square&logo=raspberry-pi&logoColor=4A7FBF&labelColor=0d1421)
![](https://img.shields.io/badge/ESM--first-0d1421?style=flat-square&logo=node.js&logoColor=4A7FBF&labelColor=0d1421)
![](https://img.shields.io/badge/Nginx_/_Cloudflare-0d1421?style=flat-square&logo=nginx&logoColor=4A7FBF&labelColor=0d1421)
![](https://img.shields.io/badge/Always_shipping-0d1421?style=flat-square&logo=github-actions&logoColor=4A7FBF&labelColor=0d1421)

</div>

<br/>

---

## `~/ecosystem`

> Ensemble de services self-hostés interconnectés, déployés derrière Nginx + Cloudflare sur une infrastructure personnelle.

<br/>

<table>
<thead>
<tr>
<th align="left" width="200">Projet</th>
<th align="left">Description</th>
<th align="left">Stack</th>
<th align="center">Status</th>
</tr>
</thead>
<tbody>

<tr>
<td><strong>VelthorianFlix</strong></td>
<td>Plateforme de streaming vidéo privée — bibliothèque SQLite, metadata TMDB, range-request streaming, watch history, transcoding externe GPU, panel admin</td>
<td><code>React 19</code> <code>Vite</code> <code>Express</code> <code>SQLite</code> <code>JWT</code></td>
<td align="center"><img src="https://img.shields.io/badge/actif-0a3d1f?style=flat-square&color=0a3d1f&labelColor=0a3d1f&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCA4IDgiPjxjaXJjbGUgY3g9IjQiIGN5PSI0IiByPSI0IiBmaWxsPSIjNGFkZTgwIi8+PC9zdmc+&logoColor=4ade80"/></td>
</tr>

<tr>
<td><strong>VelthorianDrop</strong></td>
<td>Partage de fichiers sécurisé — drag & drop, progression XHR, tokens JWT one-shot, SHA-256, expiry/password/limite de téléchargements, panel admin</td>
<td><code>Node.js</code> <code>Express</code> <code>JWT</code> <code>SQLite</code></td>
<td align="center"><img src="https://img.shields.io/badge/actif-0a3d1f?style=flat-square&color=0a3d1f&labelColor=0a3d1f&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCA4IDgiPjxjaXJjbGUgY3g9IjQiIGN5PSI0IiByPSI0IiBmaWxsPSIjNGFkZTgwIi8+PC9zdmc+&logoColor=4ade80"/></td>
</tr>

<tr>
<td><strong>VelthorianPulse</strong></td>
<td>Page de statut publique — health checks HTTP, historique 90 jours, gestion d'incidents, alertes Discord webhook</td>
<td><code>Node.js</code> <code>Express</code> <code>SQLite</code> <code>Discord</code></td>
<td align="center"><img src="https://img.shields.io/badge/actif-0a3d1f?style=flat-square&color=0a3d1f&labelColor=0a3d1f&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCA4IDgiPjxjaXJjbGUgY3g9IjQiIGN5PSI0IiByPSI0IiBmaWxsPSIjNGFkZTgwIi8+PC9zdmc+&logoColor=4ade80"/></td>
</tr>

<tr>
<td><strong>VelthorianOps</strong></td>
<td>Dashboard opérationnel unifié — analytics Cloudflare (GraphQL API), monitoring PM2 avec stream de logs SSE, cron job manager SQLite, alertes Discord</td>
<td><code>React 19</code> <code>Vite</code> <code>Express</code> <code>SQLite</code> <code>PM2 API</code></td>
<td align="center"><img src="https://img.shields.io/badge/actif-0a3d1f?style=flat-square&color=0a3d1f&labelColor=0a3d1f&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCA4IDgiPjxjaXJjbGUgY3g9IjQiIGN5PSI0IiByPSI0IiBmaWxsPSIjNGFkZTgwIi8+PC9zdmc+&logoColor=4ade80"/></td>
</tr>

<tr>
<td><strong>VelthorianGate</strong></td>
<td>Portail d'authentification — SSO, gestion de projets, tableau de bord admin avec suivi localStorage</td>
<td><code>Node.js</code> <code>JWT</code> <code>bcrypt</code> <code>SQLite</code></td>
<td align="center"><img src="https://img.shields.io/badge/en_dev-3d2000?style=flat-square&color=3d2000&labelColor=3d2000&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCA4IDgiPjxjaXJjbGUgY3g9IjQiIGN5PSI0IiByPSI0IiBmaWxsPSIjZjVhNjIzIi8+PC9zdmc+"/></td>
</tr>

<tr>
<td><strong>VelthorianRythm</strong></td>
<td>Bot Discord de musique — slash commands, Lavalink v4, 9 filtres audio, playlists SQLite, site compagnon</td>
<td><code>Discord.js v14</code> <code>Lavalink v4</code> <code>Node.js</code> <code>SQLite</code></td>
<td align="center"><img src="https://img.shields.io/badge/actif-0a3d1f?style=flat-square&color=0a3d1f&labelColor=0a3d1f&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCA4IDgiPjxjaXJjbGUgY3g9IjQiIGN5PSI0IiByPSI0IiBmaWxsPSIjNGFkZTgwIi8+PC9zdmc+&logoColor=4ade80"/></td>
</tr>

<tr>
<td><strong>Portfolio</strong></td>
<td>Site personnel — IntersectionObserver scroll reveals, mouse-tracking spotlight, count-up stats, scroll-stack project showcase</td>
<td><code>HTML</code> <code>CSS</code> <code>JS</code> <code>Nginx</code></td>
<td align="center"><img src="https://img.shields.io/badge/actif-0a3d1f?style=flat-square&color=0a3d1f&labelColor=0a3d1f&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCA4IDgiPjxjaXJjbGUgY3g9IjQiIGN5PSI0IiByPSI0IiBmaWxsPSIjNGFkZTgwIi8+PC9zdmc+&logoColor=4ade80"/></td>
</tr>

</tbody>
</table>

<br/>

---

## `~/architecture`

```
                         ┌──────────────────────┐
                         │     Cloudflare        │
                         │  CDN · WAF · DNS      │
                         └──────────┬────────────┘
                                    │ HTTPS / :443
                    ┌───────────────▼───────────────┐
                    │        Nginx Reverse Proxy     │
                    │   SSL · Cache · Rate Limiting  │
                    └──┬─────┬─────┬─────┬─────┬───┘
                       │     │     │     │     │
             ┌─────────┘  ┌──┘  ┌──┘  ┌─┘  ┌──┘
             │            │     │     │     │
             ▼            ▼     ▼     ▼     ▼
          [Flix]       [Drop] [Pulse][Gate][Ops]
          Node.js      Node   Node   Node  Node
          :xxxx        :xxxx  :xxxx  :xxxx :xxxx
             │                              │
             │                    ┌─────────┘
             ▼                    ▼
          [SQLite]            [PM2 Daemon]──[Cron runner]
          per-service              │
                              [Discord webhooks]

  ┌─────────────────────────────────────────────────────┐
  │  Infra : Raspberry Pi 5 (primary) + Debian 12 VPS   │
  │  Process manager : PM2  ·  Reverse proxy : Nginx     │
  │  Storage : SQLite per service  ·  Auth : JWT / bcrypt│
  └─────────────────────────────────────────────────────┘
```

<br/>

---

## `~/stack`

<div align="center">

<img src="https://skillicons.dev/icons?i=js,ts,react,vite,nodejs,express,sqlite,docker,nginx,linux,bash,raspberrypi,git,discord,vscode&theme=dark&perline=8" />

</div>

<br/>

<table>
<tr>
<td valign="top" width="33%">

**Frontend**
```
React 19 · Vite
HTML / CSS / JS
Recharts · Framer
```

</td>
<td valign="top" width="33%">

**Backend**
```
Node.js ESM · Express
better-sqlite3
JWT · bcrypt · PM2
```

</td>
<td valign="top" width="33%">

**Infra / Ops**
```
Nginx · Cloudflare
Docker · Raspberry Pi
Discord.js v14
```

</td>
</tr>
</table>

<br/>

---

## `~/stats`

<div align="center">

<img height="160" src="https://github-readme-stats.vercel.app/api?username=Velthorian&show_icons=true&theme=transparent&hide_border=true&title_color=4A7FBF&icon_color=4A7FBF&text_color=8b949e&bg_color=0d1117" />
<img height="160" src="https://github-readme-stats.vercel.app/api/top-langs/?username=Velthorian&layout=compact&theme=transparent&hide_border=true&title_color=4A7FBF&text_color=8b949e&bg_color=0d1117&langs_count=6" />

</div>

<br/>

---

<div align="center">

<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=300&size=11&duration=4000&pause=2000&color=1a3a5c&center=true&vCenter=true&width=400&lines=self-hosted+%2F+self-maintained+%2F+self-sufficient" />

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0d1117,40:0d1421,80:111827,100:0d1117&height=100&section=footer" width="100%"/>

</div>
