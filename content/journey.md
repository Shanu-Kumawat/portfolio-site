+++
title = "My Journey"
+++

Every developer's path is different. Mine started in computational mechanics, wound through SaaS experiments and system architecture deep dives, and led me to where I am now—building software that solves real problems. This is the story of how I got here, what I built, and what I learned along the way.

---

## The Unexpected Beginning

When I joined MNNIT Allahabad in August 2023, I came to study Engineering and Computational Mechanics. I expected to spend my years working on finite element analysis, modeling fluid flows, and running simulations in ANSYS. The curriculum delivered exactly that—Engineering Mechanics, Mechanics of Solids, Fluid Mechanics, Thermodynamics, Continuum Mechanics, Computational Fluid Dynamics, and Finite Element Methods.

These subjects taught me how to think about complex physical systems—how to break down problems mathematically, model reality through computation, and understand how systems behave under different conditions. I built a strong mathematical foundation through linear algebra, discrete mathematics, and applied computation. These courses shaped my analytical mindset, teaching me how to model problems, understand systems through equations and structure, and represent real-world phenomena through mathematical frameworks.

The computational side of my branch introduced me to data science and machine learning in mechanics, algorithms, and digital image processing. I worked with MATLAB for numerical computing and simulation environments like ANSYS and COMSOL. That's where I first saw the power of programming applied to real engineering problems.

But somewhere between fluid dynamics equations and stress tensors, I realized something important. While I enjoyed the mathematical elegance of modeling physical systems, what really excited me was writing the code that solved problems. The simulation tools were interesting, but I wanted to build the tools themselves. I didn't just want to simulate the world—I wanted to build in it.

---

## The Shift to Software

Outside the classroom, I started teaching myself what wasn't covered in the syllabus. I dove into data structures and algorithms, explored web development fundamentals, learned Git properly, and switched to Linux as my daily operating system. Those first few months were pure exploration—hours of coding, breaking things, fixing them, and trying to understand how real software systems worked.

I started with small projects—command-line utilities, simple scripts, automation tools. Each one taught me something new about how software works. I learned about managing state, handling errors, designing interfaces that make sense to users. I learned that building software is fundamentally different from solving computational mechanics problems, even though both require systematic thinking.

Looking back now, I don't see my branch choice as a mistake. Those computational mechanics courses gave me something valuable that most pure CS students don't have—a deep understanding of mathematical modeling, numerical methods, and how to think about systems that operate at scale. That foundation shows up in how I approach software problems today. When I'm optimizing performance or designing algorithms, I'm drawing on the same analytical thinking that goes into modeling physical systems.

---

## Building Real Things

As I learned more about software development, I started building projects that weren't just learning exercises—applications designed to solve actual problems.

AgriSage emerged from thinking about how machine learning could help farmers make better crop decisions based on local conditions. I integrated weather APIs, Google Maps Engine, and TensorFlow Lite to create something that could run on a mobile device and provide real value in agricultural contexts. The key architectural decision was running ML inference on-device rather than server-side, which ensures the app works in rural areas with limited connectivity—a critical requirement for the target users.

Beacon came from wanting to use technology to help people with accessibility needs. Building an AR-powered navigation app for visually impaired users meant solving hard problems—integrating object detection with voice guidance, handling real-time location data, optimizing for mobile performance. These weren't academic exercises. They were applications that required thinking about real users, edge cases, and how systems fail in the real world.

TradePulse let me apply my mathematical background to financial modeling. I implemented multiple prediction algorithms—LSTM networks, Random Forest, and Meta's Prophet—and built visualization tools to compare their performance. This project bridged my computational mechanics training with machine learning, showing me how the same analytical thinking applies across completely different domains.

Each project pushed me out of my comfort zone and taught me something new about building production software. I learned how to manage state in Flutter applications, integrate external APIs reliably, handle real-time data streams, and deploy applications that others could actually use. Most importantly, I learned that shipping something imperfect teaches you more than endlessly refining something no one sees.

---

## The SaaS Deep Dive

During the second half of 2024 and into early 2025, I decided I wanted to build my own SaaS product. This wasn't just about creating another app—I wanted to understand how real production systems work at scale. How do companies build, deploy, and maintain software that serves thousands of users reliably?

That question led me into a deep research phase. I learned about feature flags and remote configuration—how companies can change application behavior without deploying new versions. I studied deployment strategies and server administration, understanding how systems are kept running and how failures are handled. I explored backend frameworks, particularly drawn to Elixir Phoenix for its functional programming approach and built-in fault tolerance.

I experimented extensively with DevOps tools. I learned Docker for containerization, understanding how to package applications with all their dependencies. I worked with Nginx for web serving and reverse proxying. I even tried NixOS because I was fascinated by the concept of reproducible development environments. I started learning Rust to understand systems programming and what memory safety really means at a language level.

I connected with other builders on Reddit who were solving similar problems. They shared their experiences—what worked, what failed, what they wished they'd known earlier. I absorbed everything I could about how real companies operate, about market validation, about understanding user needs before building solutions.

But eventually, I realized something crucial. I was treating preparation as the product. I was so focused on learning the "right way" to build things that I wasn't actually building anything. I was researching market fit instead of putting a minimum viable product in front of real users to see what they actually wanted.

That lesson changed everything. Software development isn't about having perfect knowledge before you start—it's about building, learning from what breaks, and iterating. Done is better than perfect. Market validation matters more than technical elegance. The best way to learn is by shipping and seeing how real users interact with what you've built.

Those months of research weren't wasted, though. They built my understanding of production systems, infrastructure, and scale in ways that inform everything I build now. When I'm making architectural decisions about backends or planning deployment strategies, I'm drawing on that research about how systems scale and where they typically fail. When I'm designing APIs or thinking about state management, I understand the trade-offs because I spent time studying how production systems handle these challenges. The knowledge is valuable—I just learned that knowledge needs to be applied, not accumulated.

---

## Tools and Workflow

Through all this exploration, I've developed strong opinions about my development environment. I use Arch Linux daily, not because I enjoy tinkering for its own sake, but because Linux gives me control over my workflow in ways other operating systems don't. I use Neovim as my primary editor, which has taught me to think carefully about efficiency and automation.

When something in my workflow feels clunky, I can usually fix it or adapt existing solutions to work better. That's what led to my Quickshell Overview project. I was originally using illogical-impulse dotfiles for Hyprland, which included an excellent workspace overview widget with live previews and drag-and-drop functionality. When I switched to caelestia dotfiles for better customization, I discovered the overview widget was tightly integrated into illogical-impulse's architecture and couldn't simply be transferred. Rather than giving up the feature, I extracted the widget and refactored it into a standalone module that could work independently of any specific dotfiles setup. This meant understanding the Hyprland socket protocol, decoupling the widget from its original dependencies, and restructuring it to be self-contained while maintaining its functionality. It taught me valuable lessons about working with existing code, understanding architectural coupling, and making useful tools more modular and accessible.

I've built a reproducible Nginx development environment using Nix because I care about deployment consistency. I use Docker for containerization, Git for version control, and I'm always looking for ways to make my development workflow more efficient. These aren't just tools I've learned—they're part of how I think about building software.

---

## Where I Am Now

I'm now in my third year, maintaining a 7.63 CPI while balancing coursework in computational mechanics with my software development projects. I'm currently focusing on data structures and algorithms in Java—I chose Java specifically because of its strong presence in the Indian tech industry and its use in many large-scale production systems I want to work with.

I have technical skills across mobile development, backend systems, machine learning, and DevOps. I've shipped six projects that solve real problems. I understand both the theoretical foundations from my computational mechanics training and the practical realities of building production software. I know how to learn new technologies quickly, and more importantly, I know when to ship instead of continuing to optimize.

What I don't have yet is real industry experience. I haven't worked on a professional development team. I haven't seen how production systems are maintained at scale, how releases are managed, or experienced the constraints and trade-offs that come from shipping software that real users depend on. That's what I'm looking for now—an internship where I can work with experienced developers, contribute to products that serve real users, and learn how professional teams build and maintain software.

---

## What Drives Me Forward

When I look back at the path I've walked—from computational mechanics to software projects to exploring system architecture—I don't see wasted time or wrong choices. I see a journey where I learned by doing, built real things, and discovered what excites me about technology.

I'm drawn to problems that require scalable, efficient solutions. I love the challenge of building systems that can grow from serving ten users to serving ten thousand. Whether I'm exploring a new backend framework, diving deeper into DevOps, or optimizing a Flutter application's performance, I'm always thinking about how things work in production and how they could work better.

I'm not a master of any single technology yet. But I have curiosity, a habit of learning by building, and a track record of shipping projects that solve real problems. I understand that software development is as much about knowing when to ship as knowing how to code. And I'm ready to bring these skills and this mindset to a team that's building something meaningful.

---

## 📅 Timeline Summary

| Period | Focus | Key Activities & Takeaways |
|--------|-------|----------------------------|
| **Aug 2023 - Dec 2023** (Sem 1) | Foundation in computational mechanics | Studied Engineering Mechanics, Mathematics, began MATLAB. Built mathematical and analytical foundations. |
| **Jan 2024 - Jun 2024** (Sem 2) | Self-learning & software exploration | Learned DSA, web development, Git, switched to Linux. Started building small projects and utilities. |
| **Aug 2024 - Dec 2024** (Sem 3) | Building real projects | Built AgriSage, Beacon, TradePulse. Learned mobile development, ML integration, API design, deployment. |
| **Jan 2025 - Jun 2025** (Sem 4) | SaaS research & system architecture | Deep dive into backend frameworks (Elixir Phoenix), DevOps (Docker, Nginx), infrastructure, deployment strategies. Learned execution > perfection. |
| **Aug 2025 - Present** (Sem 5) | Workflow optimization & fundamentals | Built Quickshell Overview, Nginx Nix environment. Focused on DSA in Java for interview preparation. Seeking internships. |

---

*This is the path that brought me here—a mix of curiosity, systems thinking, and a habit of building to learn. The journey continues.*