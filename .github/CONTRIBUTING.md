# Contributing to GamingTweaks

Thanks for helping! Bug reports, test results from different PCs and well-reasoned tweak suggestions are all welcome.

## Reporting a bug

[Open a bug report](https://github.com/FiTH-g1gGLe/GamingTweaks/issues/new?template=bug_report.yml) and include:

- your GamingTweaks version (shown in the window title)
- Windows version, CPU and GPU (the **PC info** button shows all of this)
- what you clicked, and what happened
- the newest `log-*.txt` from `C:\GamingTweaks`

## Suggesting a tweak

Good suggestions explain **what** the tweak changes, **why** it helps games, and **what it could break**.
GamingTweaks has a few rules every tweak must follow:

1. **It must be reversible** — the original value is backed up and `Revert everything` restores it.
2. **It must not break** the Microsoft Store, Xbox / Game Pass, sign-in, notifications or anti-cheat.
3. **Risky tweaks are opt-in** and clearly marked.
4. **No placebo** — tweaks with no measurable benefit, or known downsides, are left out
   (see *Left out on purpose* in the README).

## Changing the code

- Everything lives in `GamingTweaks.ps1` and must run on **Windows PowerShell 5.1**.
- Keep the file **plain ASCII** (no emoji or special characters) — PowerShell 5.1 can misread them.
- Change settings through `Set-Reg` / `Set-Svc` so they are backed up automatically.
- Every pull request is checked automatically (parser + PSScriptAnalyzer). Please test on a real PC or VM
  and say what you tested in the pull request.
