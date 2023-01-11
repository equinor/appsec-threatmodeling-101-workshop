<!-- markdownlint-disable MD033 -->

# Threat Modeling the SDLC</br>∞

SDLC = Software/System Development Life Cycle<!-- .element: style="font-size:0.8em"-->

---

## Current Threat Modeling effort

- Most "security effort" is going into security for the systems that</br> we have deployed, the applications we develop
- We spend a lot less time on threat modeling </br>how we work - our SDLC
- Supply chain attacks are in the wind
- The SDLC contains many attack vectors

---

## A traditional view of a SDLC

<img src="./content/images/tm-example-sdlc.png">

<hr>

"This looks easy enough"

---

## A more realistic view of a SDLC

<img src="./content/images/tm-example-sdlc-real.png" width="70%" height="auto" display="block" margin-left="auto" margin-right="auto">

<hr>

This example is by no means exhaustive, reality is often much more complex.</br> "All models are wrong. Some models are useful"<!-- .element: style="font-size:0.7em"-->

---

## Threat Modeling our SDLC

<div style="display: grid;grid-column-gap: 1%; grid-auto-columns: 50% 50%;">
 <div  style="grid-area: 1 / 1;font-size:0.7em"">

### What could possibly go wrong?

1. Scope - which part/information flow of the SDLC are we focusing on?
2. Code is information, follow the code.
3. What can go wrong?
4. What are we going to do about it?
5. Did we do a good job?

 </div>
<div  style="grid-area: 1 / 2; font-size:0.7em"">

<img src="./content/images/tm-example-sdlc-real.png" width="100%" height="auto" display="block" margin-left="auto" margin-right="auto">

</div>

</div>

---

## Getting started

<div><!-- .element: style="font-size:0.8em"-->

- Identify and document security requirements.<!-- .element: class="fragment" data-fragment-index="1" -->
- Document SDLC (How we work, develop)<!-- .element: class="fragment" data-fragment-index="2" -->
- Document runbook (How we operate)<!-- .element: class="fragment" data-fragment-index="3" -->
- Select threat model strategy<!-- .element: class="fragment" data-fragment-index="4" -->
  - Part(s)/component(s) of the SDLC<!-- .element: class="fragment" data-fragment-index="5" -->
  - Information flow - follow the code<!-- .element: class="fragment" data-fragment-index="6" -->
- Apply STRIDE (what could go wrong?)<!-- .element: class="fragment" data-fragment-index="7" -->
- Discuss & prioritise mitigations (what are we going to do about it?)<!-- .element: class="fragment" data-fragment-index="8" -->
- Assess approach/results from SDLC threat modeling in team retrospective<!-- .element: class="fragment" data-fragment-index="9" -->

</div>

<hr>

❗️Avoid the "perfect" document/model syndrome. Start small, iterate. This goes for security requirements, the SDLC documentation, the runbook etc. Think life cycle - what documentation do we intend to maintain and keep up to date?<!-- .element: style="font-size:0.8em"--><!-- .element: class="fragment" data-fragment-index="10" -->

<hr>

❓ Reflections<!-- .element: class="fragment" data-fragment-index="11" -->

---

## Exercise 4 - Threat modeling a SDLC

---

## EX-4: Example SDLC

<img src="./content/images/tm-example-system-sdlc.png" width="65%" height="auto" display="block" margin-left="auto" margin-right="auto">

---

## EX-4: Doing an <u>end-to-end</u> Threat Model

<hr>

<div align="left"><!-- .element: style="font-size:0.7em"-->

In this exercise we will apply the skills we have acquired in the previous exercises to a fictive SDLC.

Group tasks:

- Examine the system, the SLDC, the assumptions and security requirements
- Select a <u>flow/part</u> of the example SDLC 👇
- Create a DFD diagram
- Identify threats using STRIDE or brainstorming
- Document assumptions and issues
- For threats, select strategy, identify mitigations
- Take a picture of your DFD and documents, share on Slack </br>and prepare to present the model to the class

The person in the group which last joined an Software Development Conference becomes group lead for this exercise.

<hr>

⏰ Time boxed schedule (40m):

- 10 + 10 + 10 + 10= 40 to threat model

</div>

---

## EX-4: Presentations

Each group present their results

<hr>

❓Reflections, Observations, Learning
