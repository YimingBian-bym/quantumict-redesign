---
permalink: /research/
title: "Research"
author_profile: false
classes: wide
toc: false
---

<style>
/*
  Research page:
  Keep the original Academic Pages / Markdown feeling,
  while making the desktop reading area wider and more comfortable.
*/

.research-simple {
  max-width: 1080px;
  margin: 0 auto;
  color: #243247;
}

.research-simple .research-intro {
  max-width: 980px;
  margin: 0 0 3.2rem;
  color: #56657a;
  font-size: 1.08rem;
  line-height: 1.85;
}

.research-simple h2 {
  margin-top: 3.8rem;
  margin-bottom: 1.15rem;
  padding-bottom: 0.65rem;
  color: #17355f;
  font-size: 1.72rem;
  font-weight: 650;
  letter-spacing: -0.02em;
  border-bottom: 1px solid #d9e1eb;
}

.research-simple h2.research-section-title {
  display: flex;
  align-items: center;
  gap: 1rem;
  width: 100%;
  font-size: 1.72rem !important;
  line-height: 1.2;
}

.research-simple .research-section-title__text {
  display: block;
  min-width: 0;
  color: inherit;
  font-size: inherit !important;
  font-weight: inherit;
  line-height: inherit;
  letter-spacing: inherit;
}

.research-simple h3 {
  margin-top: 2rem;
  margin-bottom: 0.75rem;
  color: #244a7c;
  font-size: 1.12rem;
  font-weight: 650;
}

.research-simple p {
  max-width: none;
  margin: 0 0 1.2rem;
  font-size: 1.02rem;
  line-height: 1.86;
}

.research-simple ul {
  margin: 0.5rem 0 1.5rem 1.25rem;
}

.research-simple li {
  margin-bottom: 0.55rem;
  padding-left: 0.25rem;
  font-size: 1rem;
  line-height: 1.7;
}

.research-simple .research-number {
  display: block;
  flex: 0 0 3.35rem;
  min-width: 3.35rem;
  margin: 0;
  color: #2f6fbd;
  font-size: 1.52rem;
  font-weight: 720;
  letter-spacing: 0.05em;
  line-height: 1;
  text-align: left;
}


.research-simple .research-links {
  margin-top: 3.5rem;
  padding-top: 1.4rem;
  border-top: 1px solid #d9e1eb;
}

.research-simple .research-links a {
  font-weight: 650;
}

@media (max-width: 768px) {
  .research-simple {
    max-width: 100%;
  }

  .research-simple .research-intro {
    margin-bottom: 2.4rem;
  }

  .research-simple h2 {
    margin-top: 3rem;
    font-size: 1.48rem;
  }

  .research-simple h2.research-section-title {
    gap: 0.7rem;
    font-size: 1.48rem !important;
  }

  .research-simple .research-number {
    flex-basis: 2.85rem;
    min-width: 2.85rem;
    font-size: 1.3rem;
  }

  .research-simple p,
  .research-simple li {
    font-size: 0.98rem;
  }
}
</style>

<div class="research-simple" markdown="1">

Our research focuses on the development and application of computational methods for chemistry, materials science, and complex physical systems. We combine first-principles theory, high-performance computing, kinetic simulation, quantum algorithms, and data-driven techniques to extend simulations toward larger systems, higher accuracy, and longer time scales.

{: .research-intro }

<h2 class="research-section-title"><span class="research-number">01</span><span class="research-section-title__text">High-Performance Computing</span></h2>

Large-scale scientific simulation depends not only on computing hardware, but also on efficient numerical algorithms and carefully designed scientific software. Our group develops high-performance computational approaches for electronic-structure calculations, atomistic simulation, spectroscopy, quantum chemistry, and related scientific applications.

A major goal is to improve scalability on modern computing platforms. This includes reducing communication and memory costs, organizing large numerical workloads efficiently, and adapting scientific algorithms to parallel and heterogeneous architectures.

### Main topics

- Massively parallel scientific algorithms
- High-performance electronic-structure calculations
- Heterogeneous CPU and accelerator computing
- Distributed numerical linear algebra and tensor operations
- Performance analysis and scientific software optimization
- Large-scale simulation of molecular and materials systems

<h2 class="research-section-title"><span class="research-number">02</span><span class="research-section-title__text">First-Principles Methods</span></h2>

First-principles methods provide a predictive description of molecules and materials from the basic laws of quantum mechanics. Our research includes the development, implementation, and application of electronic-structure methods for studying microscopic interactions and observable physical properties.

We are interested in methods that improve both accuracy and computational efficiency. By connecting theoretical formulation with numerical implementation, we aim to make advanced calculations practical for increasingly complex systems.

### Main topics

- Density-functional and electronic-structure methods
- First-principles method development and implementation
- Lattice dynamics and vibrational properties
- Electron–phonon interactions
- Raman and related spectroscopy simulation
- Response properties of molecules and materials
- Numerical methods for large-scale quantum-mechanical calculations

<h2 class="research-section-title"><span class="research-number">03</span><span class="research-section-title__text">Kinetic Monte Carlo and Multiscale Simulation</span></h2>

Many physical and chemical processes occur over time scales that are difficult to reach with direct atomistic dynamics. Kinetic Monte Carlo methods describe such processes through elementary events and transition rates, allowing simulations to access long-time evolution and large event spaces.

Our work considers efficient kinetic algorithms, rare-event processes, transition networks, and links between microscopic calculations and long-time behavior. Multiscale strategies help connect electronic, atomistic, and kinetic descriptions of complex systems.

### Main topics

- Kinetic Monte Carlo method development and implementation
- Rare-event and transition-rate simulation
- Diffusion and activated processes
- Long-time atomistic evolution
- Large reaction and transition networks
- Multiscale computational workflows
- Data-assisted kinetic model construction

## Related Research Themes

Several topics connect the three main research directions and provide additional tools for method development and scientific simulation.

### Quantum Algorithms

We explore quantum-computing approaches to chemistry and many-body problems, together with classical simulation and emulation methods for studying quantum algorithms on high-performance computing platforms.

### Artificial Intelligence for Scientific Computing

Machine-learning and data-driven methods can complement physical models, accelerate computational workflows, improve sampling, and assist in the construction of complex scientific models.

### Scientific Software

Method development and software implementation are closely connected. We aim to translate theoretical and numerical advances into reliable computational tools that can be applied to real scientific problems.


<div class="research-links">
  For research articles and related results, please visit the
  <a href="{{ '/publications/' | relative_url }}">Publications</a> page.
</div>

</div>
