---
title: Design and Benchmarks for Emulating Kondo dynamics on a Quantum Chip
summary: We formulate a novel quantum circuit to emulate periodic time-dependent Kondo Physics and also solve for our system analytically using Bosonization.
tags:
  - QInfo
  - QComp
date: '2025-01-15T00:00:00Z'

# Optional external URL for project (replaces project detail page).
external_link: ''

image:
  caption: Photo taken from our paper on arXiv https://arxiv.org/abs/2501.08499
  focal_point: Smart


url_code: 'https://github.com/lo568los/DAAD_Project'
url_pdf: ''
#url_slides: ''
#url_video: ''

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: ""
---

This project is a part of the DAAD Fellowship done under Prof. Elio Koenig from MPI Solid State Research. The first part of the project involved reading about Kondo physics, understanding its formulation as a quantum circuit via the Jordan-Wigner transformation and then utilizing Qiskit to form the circuit and obatain numerical data on observables of impurity magnetization, entanglement between impurity and fermionic sites and Hamiltonian heating as a function of time (i.e. circuit depth here) for different starting states. We utilize system sizes of 13 and 21 qubits for our analysis. These numerics have also been cross-checked using exact diagonalization (ED) for 13 quibts.

For the impurity magnetization, we observe an exponential decay into oscillations about a long-time asymptote, and these oscillations vanish in the thermodynamic limit giving the usual magnetization trend, and similar results are obtained for entanglement, mostly independent of the starting state. For Hamiltonian heating, our Fermi Sea starting state (which is the many-body ground state) leads to an increase in the energy of the system, while for excited states, we get random oscillations about 0.

In the second part, we utilized the periodic M-matrix formulation introduced by Heyl and Kehrein, alongside bosonization and refermionization to analytically obtain an expression for the impurity magnetization for the discrete (i.e. our Floquet circuit case) and the continuum case in the thermodynamic limit. We observe an excellent match in decay rates without any curve fitting and our trends for frequency of oscillations match as well. However, our analytics predict overdamped oscillations, while our numerics do not show this, which we attribute to finite size effects for our very small system sizes. The paper is up on arXiv (https://arxiv.org/abs/2501.08499).
