<!-- markdownlint-disable MD033 -->

# Threat modeling the SDLC</br>∞

SDLC = Software Development Life Cycle<!-- .element: style="font-size:0.8em"-->

---

# Threat modeling effort

- Most effort is going into security for the systems that</br> we have deployed, the applications in production
- What about the various components/parts of our SDLC? </br>Supply chain attacks are in the wind - there are many more attack vectors.

---

## A traditional view of a SDLC

<img src="./content/images/tm-example-sdlc.png">

<hr>

"This looks easy enough"

---

## A more realistic view of a SDLC

<img src="./content/images/tm-example-sdlc-real.png" width="70%" height="auto" display="block" margin-left="auto" margin-right="auto">

<hr>

This example is by no means exhaustive, reality is more complex.</br> All models are wrong. Some models are useful<!-- .element: style="font-size:0.7em"-->

---

## Threat modeling our SDLC

<div style="display: grid;grid-column-gap: 1%; grid-auto-columns: 50% 50%;">
 <div  style="grid-area: 1 / 1;font-size:0.7em"">

### What could possibly go wrong?

1. Which part/information flow of the SDLC </br>are we focusing on? Follow the code?
2. What can go wrong?
3. What are we going to do about it?
4. Did we do a good job?

 </div>
<div  style="grid-area: 1 / 2; font-size:0.7em"">

<img src="./content/images/tm-example-sdlc-real.png" width="100%" height="auto" display="block" margin-left="auto" margin-right="auto">

</div>

</div>

---

## Getting started

<div><!-- .element: style="font-size:0.8em"-->

- Identify and document security requirements.<!-- .element: class="fragment" data-fragment-index="1" -->
- Document SDLC (How we work)<!-- .element: class="fragment" data-fragment-index="2" -->
- Document runbook (How we operate, monitor)<!-- .element: class="fragment" data-fragment-index="3" -->
- Select threat model strategy<!-- .element: class="fragment" data-fragment-index="4" -->
  - Part(s)/component(s) of the SDLC<!-- .element: class="fragment" data-fragment-index="5" -->
  - Information flow - follow the code<!-- .element: class="fragment" data-fragment-index="6" -->
- Apply STRIDE (what could go wrong?)<!-- .element: class="fragment" data-fragment-index="7" -->
- Discuss & prioritise mitigations (what are we going to do about it?)<!-- .element: class="fragment" data-fragment-index="8" -->
- Assess approach/results from SDLC threat modeling in team retrospective<!-- .element: class="fragment" data-fragment-index="9" -->

</div>

<hr>

❗️Avoid the "perfect" document/model syndrome. Start small, iterate. This goes for security requirements, the SDLC documentation, the runbook etc. Think life cycle - what documentation do we intend to maintain and keep up to date?<!-- .element: style="font-size:0.8em"--><!-- .element: class="fragment" data-fragment-index="10" -->

❓ Reflections<!-- .element: class="fragment" data-fragment-index="10" -->

---

## Exercise 4 - Threat modeling a SDLC

---

## EX-4: Doing an <u>end-to-end</u> threat model

<hr>

<div align="left"><!-- .element: style="font-size:0.7em"-->

In this exercise we will apply the skills we have acquired in the previous exercises and apply them to the SDLC.

Group tasks:

- Select a <u>flow/part</u> of the example SDLC 👇
- Create a DFD diagram
- Identify threats using STRIDE (one or more parts - ex Tampering)
- For threats, select strategy, identify mitigations
- Document assumptions and security requirements
- Prepare to present results to class

<hr>

Time boxed schedule (45m):

- 5 minutes to organize
- 10 + 10 + 10 + 5= 35 to threat model
- 5 minutes complete - wrap-up

</div>

---

## EX-4: Example system

<img src="./content/images/tm-example-system-sdlc.png" width="65%" height="auto" display="block" margin-left="auto" margin-right="auto">

---

## EX-4: Presentations

Each group present their results

<hr>

❓Reflections, Observations, Learning