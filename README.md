# Hi, I'm kassyi 

Working on **G# (GSharp)**, a C# → CUDA C++ AOT transpiler built on Roslyn source generators (private while in development).<br>
C# / .NET · CUDA · compilers · multi-precision arithmetic

## Featured

**[Kassyi.Generators.DependencyProperty](https://github.com/kassyi/DependencyPropertyGenerator)** [![NuGet](https://img.shields.io/nuget/vpre/Kassyi.Generators.DependencyProperty)](https://www.nuget.org/packages/Kassyi.Generators.DependencyProperty/) [![Stars](https://img.shields.io/github/stars/kassyi/DependencyPropertyGenerator)](https://github.com/kassyi/DependencyPropertyGenerator/stargazers)

The predecessor of G# and the first of my zero-allocation series: a Roslyn incremental source generator for dependency properties, routed events and weak events (WPF / UWP / WinUI / Uno / Avalonia / MAUI).

- Zero Gen2 GC and up to 30% faster generation than upstream, so the IDE does not lag while typing
- Streams formatted code through `ref struct` scopes instead of building and normalizing syntax trees
- Reports invalid callbacks as compile-time errors instead of failing silently

**[ThumbHash Optimized](https://github.com/kassyi/ThumbHashOptimized)**

A rewrite of the ThumbHash image placeholder encoder and decoder in TypeScript, benchmarked against the original in the browser.

- Encode about 6.3x and decode about 13.6x faster than the original (Chrome, Ryzen 9 7900X)
- Folds the DCT by symmetry, processes color channels separately, packs channels into one register (SWAR) and uses lookup tables
- Generates the unrolled hot loops from TypeScript generators and EJS templates, so the source stays readable

**[N3-PDF](https://github.com/kassyi/n3-pdf)** ([open the app](https://kassyi.github.io/n3-pdf/))

A web app that lays out addresses for Nagagata 3 (長形3号, the standard Japanese business envelope, 120 × 235 mm) and outputs a print-ready PDF in the browser.

- Live PDF preview while typing (React 19, TypeScript, `@react-pdf/renderer`)
- Fills in the address from the postal code
- Converts numbers and hyphens for vertical Japanese writing

<p align="center">
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/csharp/csharp-original.svg" height="36" alt="C#" />&nbsp;&nbsp;
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/dotnetcore/dotnetcore-original.svg" height="36" alt=".NET" />&nbsp;&nbsp;
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/cplusplus/cplusplus-original.svg" height="36" alt="C++" />&nbsp;&nbsp;
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/typescript/typescript-original.svg" height="36" alt="TypeScript" />&nbsp;&nbsp;
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/react/react-original.svg" height="36" alt="React" />&nbsp;&nbsp;
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/nodejs/nodejs-original.svg" height="36" alt="Node.js" />&nbsp;&nbsp;
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/git/git-original.svg" height="36" alt="Git" />
</p>

<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://streak-stats.demolab.com/?user=kassyi&hide_border=true&theme=github-dark-blue" />
    <img height="170" src="https://streak-stats.demolab.com/?user=kassyi&hide_border=true" alt="Contribution streak" />
  </picture>
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://github-profile-summary-cards.vercel.app/api/cards/most-commit-language?username=kassyi&theme=github_dark" />
    <img height="170" src="https://github-profile-summary-cards.vercel.app/api/cards/most-commit-language?username=kassyi&theme=default" alt="Top languages by commit" />
  </picture>
</p>

<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://github-profile-summary-cards.vercel.app/api/cards/productive-time?username=kassyi&theme=github_dark&utcOffset=9" />
    <img height="170" src="https://github-profile-summary-cards.vercel.app/api/cards/productive-time?username=kassyi&theme=default&utcOffset=9" alt="Productive time (JST)" />
  </picture>
</p>

<p align="center">
  <img width="100%" src="https://ghchart.rshah.org/40c463/kassyi" alt="Contribution chart" />
</p>

## Setup

| | |
| :- | :- |
| CPU | AMD Ryzen 9 9900X (12 cores) |
| GPU | NVIDIA GeForce RTX 3070 Ti (8 GB), the CUDA target for G# |
| Memory | 64 GB DDR5-5600 |
| Storage | 3 × 1 TB SSD + 2 TB HDD |
| Displays | 2 × 4K + 2 × Full HD |
| OS | Windows 11 Pro, with WSL for Linux builds |

The benchmarks in the projects above were measured on a Ryzen 9 7900X, which this CPU replaced.
