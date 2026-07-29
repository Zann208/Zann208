# Zann

**Information Systems & Network Engineering** — Faculty of Engineering, Chiang Mai University.

I'm interested in how networks are designed and kept running, and I learn best by building the tool I wish existed. Most of what's here started as "I don't understand this yet" and turned into something I could hand to someone else.

---

### Study consoles · [zann208.github.io/study](https://zann208.github.io/study)

Course material arrives as a pile of disconnected PDFs. So each semester I build one self-contained web app per course — the lectures, the labs and the practice all in a single HTML file that works offline.

| | Course | |
|---|---|---|
| **[netdes](https://github.com/Zann208/netdes)** | 261434 Computer Network Design & Management | [live ↗](https://zann208.github.io/netdes/) |
| **[wnet](https://github.com/Zann208/wnet)** | 269430 Wireless & Broadband Networks | [live ↗](https://zann208.github.io/wnet/) |
| **[algo](https://github.com/Zann208/algo)** | 269202 Algorithms for iSNE | [live ↗](https://zann208.github.io/algo/) |

The one I'm proudest of is inside **netdes**: a port-role solver that runs the real **802.1D spanning-tree algorithm** — root election by Bridge ID, shortest path by cost, then the four-step tie-break — so it can generate unlimited practice scenarios and mark them. I validated it against every hand-solved lab answer I had, then fuzzed it with 20,000 random topologies looking for a case where it broke the protocol's invariants. It didn't.

```
20000 random scenarios (7998 with tied priorities) — violations: 0
```

---

### How I build

Vanilla HTML, CSS and JavaScript. No framework, no build step, no dependencies — each console is one file you can open from a USB stick with the Wi-Fi off. That constraint is deliberate: it forces me to actually understand the DOM, Canvas and layout instead of reaching for a library.

Also comfortable with **C++** (data structures coursework), **Cisco IOS** configuration, Packet Tracer and GNS3.

---

### Currently

Studying for midterms, extending the consoles as each course goes on, and slowly turning my home lab into something worth documenting.

**[Portfolio](https://zann208.github.io)** · **[thuhtoozan_1@cmu.ac.th](mailto:thuhtoozan_1@cmu.ac.th)** · Chiang Mai, Thailand
