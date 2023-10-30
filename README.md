# ZKCamp's Aleo Course

## About Aleo
Aleo is a Layer-1 blockchain that supports privacy-preserving applications using zero-knowledge technology. Leo, Aleo's zero-knowledge programming language, makes writing private-by-default applications easy by compiling circuits down to low-level Aleo instructions. It provides powerful, blockchain-native syntax and robust error-handling, giving developers the perfect combination of performance, reliability, and security.

## About ZKCamp
[ZKCamp](www.zkcamp.xyz) is a ZK education company. ZKCamp's primary offering is a live cohort-based course that teaches ZKPs and their underlying mathematical and cryptographic principles using hands-on examples and engaging assessments. The course is tailored for engineers who do not have a math or cryptography background but are eager to learn it. Through a structured curriculum and live sessions with instructors, participants will have the opportunity to learn and engage with the material in a collaborative environment. Upon completion of the course, participants will have the knowledge and skills necessary to build decentralized applications based on ZKPs.


## What is this course about?

Zero-knowledge cryptography has seen rapid progress in recent years and is used today for both scalability and privacy purposes in blockchains.

Aleo is leveraging the zero knolwedge cryptography to build a privacy-first blockchain that is also programmble. Thsi makes it significantly easier for developers to buidl and deploy private and decentralized blockchains.
Most ZK frameworks require advanced cryptography expertise, but Aleo with the Leo language and Aleo instructions abstracts away much of the complexity to open up zkApp development to the broader pool of web 3.0 developers.

The shift from traditional development to building ZKP applications on Aleo introduces a new set of concepts and tools that may seem overwhelming at first. Aleo collaborated with ZKCamp.xyz to launch the first live cohort to teach building on the Aleo platform to a set of 20 developers durind Oct 08-28, 2023. 

 The course, led by the instructors at ZKCamp and sponsored by Aleo, is tailored for engineers who do not have a math or cryptography background but are eager to learn it. Through a structured curriculum and live sessions with instructors, participants had the opportunity to learn and engage with the material in a collaborative environment. 

## Prerequisites

1. Read this [blog](https://www.zkcamp.xyz/blog/what-is-a-zkp-anyway) to make sure you have a basic understanding of what zero-knowledge proofs are all about.
2. Zero-knowledge proofs are based on certain mathematical primitives. Read the blogs below to get a basic understanding of the underlying mathematics

    * [Polynomials](https://www.zkcamp.xyz/blog/you-cant-understand-zkps-without-understanding-polynomials)

    * [Modular Math](https://www.zkcamp.xyz/blog/why-we-use-modular-math-for-zero-knowledge-proofs)

3. Read this [blog](https://www.zkcamp.xyz/blog/information-theory) to get an introduction to Information Theory.


## Lectures & course materials
Lectures are of 90 min each. Each of the items below has the lecture recording, slides, quizzes and assignments associated with the lecture

<details>
<summary><b>&nbsp;Lecture 1 - Cohort Introduction & ZKP Fundamentals</b></summary>
<br/>
The first lecture reviews the curriculum and covers some of the Zero-Knowledge Proofs fundamentals that will be useful for future lectures. The lecture ends with a meet and greet session amongst the ZKCampers in the cohort.

<br/>
<li><a href = "https://drive.google.com/file/d/18bdm2DZHROAq2s4S7cdjySC3DI-S4WbQ/view?usp=sharing">Recording</a></li>
<li><a href = "https://drive.google.com/file/d/1Himv0ABiYFoOroX75EBxonc9l3MhRN-I/view?usp=sharing">Slides</a></li>
<li><a href = "https://rose-fedora-226.notion.site/ZKP-Fundamentals-Quiz-d26816a306ba4e99ae88ad25a6482fcd?pvs=4">ZKP Fundamentals Quiz</a></li>
</details>

<details>
<summary><b>&nbsp;Lecture 2 - Introduction to the Aleo Ecosystem</b></summary>
<br/>
In this lecture, Caleb Curry, from developer relations at Aleo, provides an introduction to the Aleo ecosystem. The lecture touches upon Aleo's core features, its emphasis on privacy, and its utilization of zkSNARKs. The lecture also explores how zero-knowledge proofs are employed within Aleo by diving into the architecture of the platform.

<br/>
<li><a href = "https://drive.google.com/file/d/1eJFaHUrkzSnwm6b7HAOSc8iB4Nclnnaf/view?usp=sharing">Recording</a></li>
<li><a href = "https://drive.google.com/file/d/1BjdihKqeFXCBMo0t4bS6maBZAhrLhgUb/view?usp=sharing">Slides</a></li>
<li><a href = "https://rose-fedora-226.notion.site/Aleo-Fundamentals-Quiz-870f3c9fc9f04845b84be6c9d3fbbc92?pvs=4">Aleo Fundamentals Quiz</a></li>
</details>

<details>
<summary><b>&nbsp;Lecture 3 - zkSNARKs - Mathematical and Cryptography Primitives</b></summary>
<br/>
This and the next 2 lectures focus on zkSNARKs, the building blocks of the Aleo blockchain. In this lecture, students are introduced to the mathematical and cryptographic primitives that are essential for understanding how zkSNARKs word under the hood. The lectures starts by explanining the anatomy of a zkSNARK system and dives deeper into Polynomials and their properties that are useful in context of the zkSNARK systems. The last topic covered is Finite Field arithmetic and its usefulness in building cryptograhpic systems in general and zkSNARK systems in particular.

<br/>
<li><a href = "https://drive.google.com/file/d/1iJ23MO13lEotLT4LNYWU0a0HpGrMD0N9/view?usp=sharing">Recording</a></li>
<li><a href = "https://drive.google.com/file/d/1foKxWcKaOZUtebA6jUyDGq4nzQXUaiI2/view?usp=sharing">Slides</a></li>
<li><a href = "https://tarry-spur-32f.notion.site/Polynomials-Quiz-0ca8a325759b44b293a0234b5070b36e?pvs=4">Polynomials Quiz</a></li>
<li><a href = "https://rose-fedora-226.notion.site/Modular-Arithmetic-Quiz-ef788ad032e0404c907abb0f2d6c8740">Modular Math Quiz</a></li>
<li><a href = "https://github.com/ZKCamp/aleo-lagrange-assignment/tree/main">Lagrange Polynomial Assignment</a></li>
<li><a href = "https://github.com/ZKCamp/aleo-lagrange-assignment/tree/solution">Lagrange Polynomial Assignment Solution</a></li>

</details>

<details>
<summary><b>&nbsp;Lecture 4 - zkSNARKs - Arithmetization</b></summary>
<br/>
Arithmetization is the technique by which high level programs are converted into a system of mathematical constraints using polynomials. In this lecture, we look at various steps in Arithmetization of programs and deep dive into the R1CS Arithmetization technique used by the zkSNARK proof system used by Aleo. We conclude the lectue by taking a pen and paper example to understand Arithemtization at an implementation level.

<br/>
<li><a href = "https://drive.google.com/file/d/1d2VJm6UdcIf3ZkadKUcU7TiZZy1zqsXP/view?usp=sharing">Recording</a></li>
<li><a href = "https://drive.google.com/file/d/1a_j2fCnnaBy0Y7lwMLkqkus-wTylwW1R/view?usp=sharing">Slides</a></li>
<li><a href = "https://gist.github.com/shubham-kanodia/dc9590531a3df230fc8063e499443932">Arithmetization example from lecture</a></li>
<li><a href = "https://rose-fedora-226.notion.site/Arithmetization-Quiz-e2edb41563e345f9b594fb13f72ddba7">Arithmetization Quiz</a></li>
<li><a href = "https://github.com/ZKCamp/aleo-qap-assignment">Arithmetization Assignment</a></li>
<li><a href = "https://github.com/ZKCamp/aleo-qap-assignment/tree/solution">Arithmetization Assignment Solution</a></li>

</details>

<details>
<summary><b>&nbsp;Lecture 5 - zkSNARKs - Elliptic Curves, KZG and Marlin</b></summary>
<br/>
<br/>
<li><a href = "https://drive.google.com/file/d/1SeTvO3qCHXnst9kSVKldHMLR581wi2XB/view?usp=sharing">Recording</a></li>
<li><a href = "https://drive.google.com/file/d/1asUU8VJL6mNvw7q_xBs70ncTWyj5uya4/view?usp=sharing">Slides</a></li>
<li><a href = "https://rose-fedora-226.notion.site/Elliptic-Curves-Quiz-6fc3b5b6b2c443d184646957b6a879c0">Elliptic Curves Quiz</a></li>
</details>

<details>
<summary><b>&nbsp;Lecture 6 - Leo Language Fundamentals</b></summary>
<br/>
<br/>
<li><a href = "https://drive.google.com/file/d/11wA3RjEk97eOpGlNGQ9zXpyjmmOG5TKJ/view?usp=sharing">Recording</a></li>
<li><a href = "https://drive.google.com/file/d/1XTzaZhWZ5iTY5laTZ-aD34bs6cXoYWR8/view?usp=sharing">Slides</a></li>
<li><a href = "https://github.com/ZKCamp/aleo-store-assignment">Store Assignment</a></li>
<li><a href = "https://github.com/ZKCamp/aleo-store-assignment/blob/solution/src/main.leo">Store Assignment Solution</a></li>
</details>

<details>
<summary><b>&nbsp;Lecture 7 - Building a ZK App on Aleo</b></summary>
<br/>
<br/>
<li><a href = "https://drive.google.com/file/d/1Oo5zYddYOTuAEu4KOxkXmTacRTYkSmxC/view?usp=sharing">Recording</a></li>
<li><a href = "https://drive.google.com/file/d/1yqESYb5QlUI4i25JcdthQXAmHfoWnTXu/view?usp=sharing">Slides</a></li>
</details>

<details>
<summary><b>&nbsp;Lecture 8 - Advanced Aleo</b></summary>
<br/>
<br/>
<li><a href = "https://drive.google.com/file/d/1stEtHt-HsrFx3TNFNzfPqwbaa5tylGio/view?usp=sharing">Recording</a></li>
<li><a href = "https://drive.google.com/file/d/1fm0Z6fdZC2PFr-3YJIQ_qZI3ADqGPq_T/view?usp=sharing">Slides</a></li>
</details>

<details>
<summary><b>&nbsp;Demo Day</b></summary>
<br/>
<br/>
<li><a href = "https://drive.google.com/file/d/1PhWL5vqLINHvFdoprDBeWE-yPCMfyKXU/view?usp=sharing">Recording</a></li>
</details>


<br/>
