---
title: Magic of finite-temparature eigenstates in quantum chaotic Hamiltonians
summary: We use Scrooge ensemble to provide robust numerical match with finite-temparature eigenstate magic, utilizing Gaussian distribution ansatzes to motivate our results analytically.
tags:
  - QInfo
date: '2025-10-15T00:00:00Z'

# Optional external URL for project (replaces project detail page).
external_link: ''

image:
  caption: Photo taken from https://doi.org/10.1103/PhysRevX.14.041051
  focal_point: Smart


url_code: 'https://github.com/lo568los/DeepTherm'
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

This project is a part of a collaboration with Dariel Mok, a PhD student at John Preskill's group in Caltech, and Tobias Haug. Recent results on deep thermalization and exploring metric of non-stabilizeress (magic) and entanglement entropy of eigenstates of quantum chaotic Hamiltonians motivated our question to utilize a thermal Scrooge ensemble (a minimal information setting) and argue that it should be able to reproduce stabilizer Renyi entropies for eigenstates away from the middle of the spectrum (finite-temparature eigenstates). We are able to confirm these results with robust exact diagonalization data for up to N = 14 qubits, considering a mixed-field Ising model. Utilizing weingarten calculus allowed me to provide some analytical expressions as well about distributions of Pauli spectrum over the Scrooge ensemble. Another approach considered is comparing Pauli spectrum distributions across eigenstates and Scrooge ensembles and finding that it ultimately converges to Gaussian distributions. We are preparing these results in a manuscript.