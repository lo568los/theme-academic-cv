---
title: MQ based identification signatures
summary: We study the construction security and implementation aspects of MQDSS, a MQ-based signature scheme based of the MQ-based identification scheme
tags:
  - Other
date: '2024-04-27T00:00:00Z'

# Optional external URL for project (replaces project detail page).
external_link: ''

image:
  caption: Photo taken from https://arxiv.org/abs/2207.07305
  focal_point: Smart


url_code: ''
url_pdf: 'https://drive.google.com/file/d/1y5foFk6FANbj9RVxUMK07AcDQwrEuxBi/view?usp=sharing'
#url_slides: ''
#url_video: ''

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: ""
---

This project is a part of an term paper project in my 4th semester course E0 213 (Quantum safe cryptography) instructed by Prof. Sanjit Chatterjee at IISc Bangalore. It is a joint report with Shubh Prakash, a senior student at IISc. A small abstract is presented below:

"MQDSS (Multivariate Quadratic Digital Signature Scheme) is a cryptographic signature scheme based on the hardness of solving multivariate quadratic (MQ) equations, a problem considered resistant to attacks by quantum computers. Unlike traditional cryptographic methods, which rely on number-theoretic problems like factoring or discrete logarithms, MQDSS leverages the difficulty of solving systems of quadratic equations over finite fields, making it a strong candidate for post-quantum cryptography.

MQDSS is particularly notable for its efficiency and compactness, offering relatively small signature sizes compared to other post-quantum signature schemes. It utilizes a Fiat-Shamir transform applied to an identification scheme based on the MQ problem, which ensures security by reducing the signature verification process to checking the validity of a quadratic equation system. Due to its robust security guarantees and efficiency, MQDSS is a promising candidate for securing communications in the post-quantum era, where quantum-resistant cryptographic methods will be essential."



