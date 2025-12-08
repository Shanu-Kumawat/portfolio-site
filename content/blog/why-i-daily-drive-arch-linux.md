+++
title = "Why I Daily Drive Arch Linux (And Why You Might Not Want To)"
date = 2024-10-28
draft = false

[taxonomies]
tags = ["linux", "arch", "workflow", "developer-tools"]

[extra]
reading_time = 5
+++

I use Arch Linux as my daily driver. Not because I'm elitist, but because it fits how I work. Here's the honest take.

<!-- more -->

## Let's Get This Out of the Way

Yes, I use Arch. No, I'm not going to tell you it's objectively superior to your OS. Yes, I've tried NixOS (more on that later). No, I don't think everyone should use Arch.

Cool? Cool.

## Why Arch?

### It Gets Out of My Way

This is the big one. Arch doesn't make decisions for me. It doesn't bundle software I don't want. It doesn't have opinions about how I should work.

Want to use Hyprland as your window manager? Cool, here's how.  
Want to run Neovim as your editor? No problem.  
Want to set up your system exactly how you like it? That's kind of the whole point.

I'm not fighting the OS. I'm configuring it once, then forgetting about it.

### The AUR Is Actually Good

Yeah, I said it. The Arch User Repository is legitimately one of the best things about the Linux ecosystem.

Need some obscure package? It's probably in the AUR.  
Want the latest version of something? AUR.  
Building from source? There's probably an AUR package that handles it.

Compare that to PPAs on Ubuntu or manually adding repos—the AUR just works. Most of the time.

### Rolling Release = Current Software

I'm a developer. I want current tools. Not "stable" versions from 2 years ago.

With Arch, I get:
- Latest kernel
- Latest drivers
- Latest development tools
- Latest everything

Yeah, there's a risk of things breaking. But in 2+ years of daily driving Arch? I've had maybe 3 issues. All fixable in minutes.

### It Taught Me How Linux Actually Works

This is underrated. Installing Arch forces you to understand:
- Partitioning
- Bootloaders
- Display servers
- Init systems
- Package management

You're not clicking "Next" through an installer. You're building your system piece by piece.

Is that necessary for everyone? No.  
Did it make me a better developer? Absolutely.

## The Hyprland Setup

I run Hyprland as my window manager. It's a Wayland compositor, tiling, smooth as butter.

Why Hyprland?
- Wayland native (better for modern laptops)
- Tiling by default (keyboard-driven workflow)
- Ridiculously smooth animations
- Highly configurable

I even built a [Quickshell Overview module](/projects/quickshell-overview) for it—a workspace switcher similar to macOS. That's the kind of thing you can do when your OS doesn't lock you in.

## The NixOS Experiment

I tried NixOS for a while. Loved the concept. Reproducible builds. Declarative configuration. Everything as code.

But...

### The Problem

Android development on NixOS is painful. The Flutter + Android SDK setup is way more complicated than it should be. Spending hours fighting your OS to install basic dev tools isn't productive.

So I went back to Arch. Not because NixOS is bad—it's brilliant—but because I needed something that worked *now*, not after 10 hours of debugging.

(I still use Nix for dev shells though. Best of both worlds.)

## Who Should Use Arch?

**You might like Arch if:**
- You want to understand how your system works
- You prefer configuring over accepting defaults
- You value bleeding-edge software
- You're comfortable with the terminal
- You don't mind reading documentation (the Arch Wiki is incredible)

**You probably shouldn't use Arch if:**
- You just want something that works out of the box
- You don't care about customization
- You're not comfortable troubleshooting
- You need 100% stability with zero maintenance

## My Actual Setup

Here's what I run:
- **OS**: Arch Linux (obviously)
- **WM**: Hyprland (Wayland compositor)
- **Editor**: Neovim (btw)
- **Terminal**: Alacritty
- **Shell**: Zsh with custom config
- **Dev**: Docker, Flutter, Rust, Python, Java

It boots fast. It runs fast. It looks good. It does what I need.

## The Honest Downsides

Let's not pretend it's perfect:

### 1. You Will Break Things

Not often. But it happens. Usually your fault. Sometimes not.

You need to be okay with that.

### 2. Setup Takes Time

My current setup took days to configure exactly how I want it. Was it worth it? Yes. Is everyone willing to invest that time? No.

### 3. Not Beginner-Friendly

If you're new to Linux, start with Ubuntu or Fedora. Seriously. Learn the basics first. Then, if you want, try Arch.

Jumping straight to Arch is like learning to code by building a compiler. Technically possible. Practically painful.

### 4. You'll Waste Time Ricing

"Ricing" = customizing your Linux setup to look cool.

I've spent way too many hours tweaking configs, trying new color schemes, adjusting Hyprland animations.

It's fun. It's also a productivity black hole. Be warned.

## Bottom Line

I use Arch because:
- It fits my workflow
- I learned a ton setting it up
- I like having control
- The AUR is great
- It's fast and minimal

Should you use Arch?

Maybe. If you're curious, willing to learn, and don't mind occasionally fixing things.

Or maybe not. Ubuntu is great. Fedora is solid. macOS works. Windows with WSL is fine.

Use what makes you productive. For me, that's Arch + Hyprland + Neovim.

For you? Could be something completely different.

And that's okay.

---

*Currently running Arch with Hyprland, ~4GB RAM usage at idle, boots in 8 seconds. No regrets.*
