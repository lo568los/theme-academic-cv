---
title: Design and benchmarks for emulating Kondo dynamics on a quantum chip
summary: We formulate a novel quantum circuit to emulate periodic time-dependent Kondo Physics and also solve for our system analytically using Bosonization.
authors:
- Soumyadeep Sarma
- Jukka I. Väyrynen
- Elio J. K\n̈ig
date: '2025-06-01'
publishDate: '2025-11-09T09:37:01.489621Z'
publication_types:
- article-journal
publication: '*Phys. Rev. B*'
doi: 10.1103/c864-5bbt
links:
- name: URL
  url: https://link.aps.org/doi/10.1103/c864-5bbt
featured: true
---

This project is a part of the DAAD Fellowship done under Prof. Elio Koenig from MPI Solid State Research. The first part of the project involved reading about Kondo physics, understanding its formulation as a quantum circuit via the Jordan-Wigner transformation and then utilizing Qiskit to form the circuit and obatain numerical data on observables of impurity magnetization, entanglement between impurity and fermionic sites and Hamiltonian heating as a function of time (i.e. circuit depth here) for different starting states. We utilize system sizes of 13 and 21 qubits for our analysis. These numerics have also been cross-checked using exact diagonalization (ED) for 13 quibts.

For the impurity magnetization, we observe an exponential decay into oscillations about a long-time asymptote, and these oscillations vanish in the thermodynamic limit giving the usual magnetization trend, and similar results are obtained for entanglement, mostly independent of the starting state. For Hamiltonian heating, our Fermi Sea starting state (which is the many-body ground state) leads to an increase in the energy of the system, while for excited states, we get random oscillations about 0.

In the second part, we utilized the periodic M-matrix formulation introduced by Heyl and Kehrein, alongside bosonization and refermionization to analytically obtain an expression for the impurity magnetization for the discrete (i.e. our Floquet circuit case) and the continuum case in the thermodynamic limit. We observe an excellent match in decay rates without any curve fitting and our trends for frequency of oscillations match as well. However, our analytics predict overdamped oscillations, while our numerics do not show this, which we attribute to finite size effects for our very small system sizes. The open access version is up on arXiv (https://arxiv.org/abs/2501.08499).
