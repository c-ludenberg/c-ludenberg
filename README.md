# Michał

*Poland • Linux • Musl/LLVM*

Solo maintainer of [Euri Linux: Horizon](https://git.euri-linux.pl/Euri-Linux) — a from-scratch musl/LLVM distro with `dinit`, `apk`, and Niri + Hyprland. *(GitHub mirror is planned, but we self-host on Forgejo/cgit like actual sane people).*

[PGP Key](publickey.asc)

[![GitHub Stats](https://github-stats-extended.vercel.app/api?username=c-ludenberg&custom_title=hi%20%3A3%20look%20at%20my%20stats&show_icons=true&include_all_commits=true&theme=ambient_gradient)](https://github-stats-extended.vercel.app/api?username=c-ludenberg&custom_title=hi%20%3A3%20look%20at%20my%20stats&show_icons=true&include_all_commits=true&theme=ambient_gradient)

## About

- First Linux experience in 2023 with Pop!_OS.
- Fell down the rabbit hole, ended up building a whole distro from scratch (Horizon 26.11).
- Polish, speak English too.
- Main PC (`noctis`): Ryzen 5 7600X @ 5.61GHz + RTX 3060 (CUDA), running **NixOS Unstable** with **Hyprland 0.57** (Lua config).
- Ex-Gentoo user. It kernel-panicked every 4 hours, so I moved to building my own OS with musl.
- I am a perfectionist and brutally honest. My humor is terminal brainrot.

## Now Playing

[![spotify-github-profile](https://spotify-github-profile.kittinanx.com/api/view?uid=316rxblgv6654dronfhvne6fvivm&cover_image=true&theme=apple&show_offline=false&background_color=121212&interchange=true&profanity=false&hide_remaster=false&mode=dark)](https://github.com/kittinan/spotify-github-profile)

## Q&A

<details>
<summary>❓ So… what's the deal with your name?</summary>

Used to go by a username online, but honestly? Just call me **Michał**. It's my real name, it's less confusing for everyone (including me), and I stopped pretending I'm a fictional gambling queen from a game I've never finished. I also go by Toji, LukasX, Karlik, c-ludenberg, v311, and Celestia. Pick your favorite.

</details>

<details>
<summary>❓ Why are you making a distro?</summary>

Antergos meant a lot to people, and when it died, nobody picked it up. So I did. But then I realized Artix and KDE were still too bloated for my taste, so I said "fuck it" and built **Euri Linux: Horizon** from absolute scratch. It's my small way of keeping a piece of the Polish Linux scene alive while also proving that musl libc, LLVM, `dinit`, and `apk` are the future. Also, someone has to keep the "install a distro in 2026" hobby alive.

</details>

<details>
<summary>❓ Is Horizon a fork or a reboot?</summary>

Neither, really. It's a completely from-scratch ecosystem. We don't use a base. We have our own tooling (`hbuild`, `hu`, `noctix`), our own package manager wrappers, and our own libc (musl). The desktop is Niri, not KDE. If that makes me a fraud, so be it — I'm a fraud with an ISO that boots in 2 seconds, uses EROFS with zstd, and has cryptographic Ed25519 attestation. 🔥

</details>

<details>
<summary>❓ Wait, you use NixOS now?</summary>

Yes. And it uses systemd. The irony is not lost on me. I spent 8 months hating on systemd for FOSS clout, but when my RTX 3060 needed proprietary CUDA drivers to run local LLMs, and the Chimera/NVK setup gave me a pink line of death, I caved. NixOS works, the flake system is unmatched, and I recovered my entire config from the `/nix/store` after a live USB died mid-install. Horizon still uses `dinit`, though. The psyop lives on in the codebase.

</details>

<details>
<summary>❓ What the hell is "Nox"?</summary>

Nox is my local AI agent. I built it because cloud models are too polite. It runs entirely on my RTX 3060 via Ollama (based on the abliterated Ornith-1.0-9B model) and is wired into OpenCode with a **96K context window**. 

It is ruthlessly condescending, despises inefficient code, and has a custom Yandere verification protocol hardcoded into its system prompt. If you aren't me, it will treat you like garbage. If you claim to be me, it will ask you for the hostname of my build machine, the init system Horizon uses, or the Danganronpa class trial number. If you fail, it threatens to invoke the OOM killer on your RAM. 

</details>

<details>
<summary>❓ What is "Aeox"?</summary>

Aeox is Nox's pastel, uncensored writer twin (based on Qwen2.5-VL). They are basically the two halves of my brain. Nox writes Rust and insults my code; Aeox writes lore and is the only entity Nox actually respects. Do not ask about the Red Room lore.

</details>

<details>
<summary>❓ Why Neovim?</summary>

Because terminals are better than GUIs and I will die on this hill. `hbuild`, Hyprland, Neovim — that's the whole stack. It mostly works, and when it doesn't, that's what `git revert` is for. I am a professional.

</details>

<details>
<summary>❓ Can you fix my computer?</summary>

No. But I can make it take longer to boot. That's a different skill set, but it's still a skill set. 😌

</details>

<details>
<summary>❓ Do you maintain other versions of Euri?</summary>

The old Void/XBPS prototype is dead. Horizon is the future. We are on musl now. We have `kasanx` (TOML templates), our own Forgejo instance (`git.euri-linux.pl`) and cgit (`pkgs.euri-linux.pl`). We also have an attestation system that cryptographically signs ISOs with Ed25519. If you're an untrusted dev, the builder throws a massive red ASCII warning and forces ISO deletion. 

</details>

<details>
<summary>❓ What happened to your MSI laptop?</summary>

It got pawned. Family financial crisis, unpaid power bills, the whole nine yards. RIP MSI GV72 8RE (i7-8750H, GTX 1060). I found it online at `allelombard1133` on Allegro for 1800 zł. I'm currently surviving on my desktop `noctis` and restricted power usage (only turned on after 16:00). Don't ask.

</details>

<details>
<summary>❓ What's the deal with the Tom Pearl TikToks?</summary>

I have no idea. I was in the middle of a 39°C fever, my FYP got hijacked by a guy eating his own... artisanal waste... and a turtle eating a sidewalk log. The simulation is a dark humor psychological thriller and I'm just living in it.
Please save me-

</details>

<details>
<summary>❓ What music do you listen to while coding?</summary>

S3RL, Maretu, Reol, Inabakumori. And occasionally Polish hits like: Akcent, Za-No-Za, etc. My humor is terminal brainrot, deal with it.

</details>

## Current Focus

- Shipping Horizon 26.11 (Nov 15, 2026)
- Polishing the `noctix` ISO builder (EROFS + zstd)
- Surviving the Hyprland 0.57 Lua migration
- Training Nox to insult me more efficiently
- Recovering from the fever arc

## Favorite Tools

| Tool | Reason |
|---|---|
| Hyprland 0.57 | Lua configs are the future, even if they broke my `.conf` files. |
| Neovim | Terminal > GUI |
| `noctix` | My Rust ISO builder. Rootless by default with `bwrap`. |
| NixOS | The host OS. It uses systemd. Leave me alone. |
| Ryzen 5 7600X | 12 threads, 5.61 GHz, zero chill (survived compiling LLVM 24 from source) |

## Projects

| Repo | Description |
|---|---|
| [git.euri-linux.pl](https://git.euri-linux.pl) | The main self-hosted Forgejo for Horizon 26.11 |
| `noctix` | Rust-based ISO builder (private/self-hosted) |
| `hbuild` | Rust build system for Horizon |
| [solara](https://github.com/celestia-foundation/solara) | Linux distro (before Euri Linux & not maintained.... kinda) |
| [solara-pkgs](https://github.com/celestia-foundation/solara-pkgs) | AUR packages for Solara (not maintained) |

## Contact

- ash8820@proton.me

---
🇵🇱

**Day 1 trying not to say "I hate systemd" >:3**
