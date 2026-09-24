## Wilder Molyneux

Enterprise Architect and hands-on engineer in Seattle. Twenty years spent
making large systems agree with each other, across aerospace,
telecommunications, consumer products, and commercial real estate.

Currently pursuing a Master of Science in Computer Science (MSCS) at the
University of Texas at Austin, focused on deep learning.

Certified in The Open Group Architecture Framework (TOGAF 9), with a
certificate in Enterprise Architecture from Carnegie Mellon University and the
Graduate Certificate in Software Design and Development (GCSDD) from the
University of Washington Bothell.

---

### Latest project: Falling Into Scepter Valley

[![Falling Into Scepter Valley, a Mandelbrot deep zoom](https://img.youtube.com/vi/b2cpUL_xEc4/maxresdefault.jpg)](https://youtu.be/b2cpUL_xEc4)

A renderer that descends 33 decades into the Mandelbrot set and comes back
with a three minute film. Written in Rust and WebGPU Shading Language (WGSL),
running on graphics processing units (GPUs) from one source tree.

The interesting part is not that it is fast. It is that it stopped rendering
frames, computing the plane once instead of once per frame it appears in. That
cut the render from 408 GPU-hours to roughly 32, for a deeper zoom.

It also stopped running on one machine. Work is sharded across a multi-cloud
fleet: local Apple Silicon and rented GPUs on both Google Cloud Platform
(GCP) and Amazon Web Services (AWS), split by cost rather than evenly. Every
host runs a ninety-second preflight before it is given work and terminates
itself when it finishes or stalls, so a bad node fails loudly instead of
billing quietly. Shard output is verified bit-identical to a local render
rather than assumed equivalent.

**[Watch the film](https://youtu.be/b2cpUL_xEc4)** &nbsp;·&nbsp;
**[Read the code](https://github.com/Wilder101/mandelbrot-deep-zoom)**

---

### Applied AI Pipeline Architecture

A written record of running generative artificial intelligence in production
across three small commercial ventures: how the model and the vendor were
chosen on measured cost and risk, how intellectual property and data licensing
are handled, and how "good enough to ship" is decided by measurement rather
than by taste.

Eight architecture decision records, several of which retract something I had
already written down as fact. The through-line is that the useful boundary is
not whether a model is involved, but whether the output's correctness is
checkable. Where work is judged, a model is the right tool and a human is the
gate. Where it makes verifiable claims about the world, the gate has to be
mechanical. One of the three ventures now runs with no generative model in its
pipeline at all.

**[Read the records](https://github.com/Wilder101/applied-ai-pipeline-architecture)**

---

### Also here

Four C++ programs written as prerequisite coursework for the GCSDD program at
the University of Washington Bothell: batch inventory processing, a hangman
engine, a stack-based search through a cave graph, and a Sieve of
Eratosthenes.

**[Browse them](https://github.com/Wilder101/GCSDDprereqsWeb)**

---

### Elsewhere

[wilder101.github.io](https://wilder101.github.io/) &nbsp;·&nbsp;
[LinkedIn](https://www.linkedin.com/in/wildermolyneux/)
