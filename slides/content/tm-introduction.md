<!-- markdownlint-disable MD033 -->

# Threat modeling Introduction </br>🖖

---

## What is threat modeling?

> Threat modeling is the process of analysing a system to look for weaknesses that comes from less-desirable design choices. The goal is to identify the weaknesses before they are baked into the system and thus reduce risk in a system to an acceptable level.

We want to identify the weaknesses as early as possible.

❗️Threat modeling must be a cyclic/continuous effort, not a one off activity.

---

## Why Threat modeling?

- Develop more secure system<!-- .element: class="fragment" data-fragment-index="1" -->
- Develop more securely<!-- .element: class="fragment" data-fragment-index="2" -->
- Educate developers / teams, share knowledge<!-- .element: class="fragment" data-fragment-index="3" -->
- Have a systematic and consistent approach to security<!-- .element: class="fragment" data-fragment-index="4" -->

❗️Threat modeling will guide our designs </br>and help us make decisions with our eyes open.<!-- .element: class="fragment" data-fragment-index="5" -->

<hr>

❓ What are your<!-- .element: class="fragment" data-fragment-index="6" --> <u>current</u> reasons for wanting to Threat Model?<!-- .element: class="fragment" data-fragment-index="6" -->

---

## The 4 Questions of Threat modeling

- What are we working on?<!-- .element: class="fragment" data-fragment-index="1" -->
- What can go wrong?<!-- .element: class="fragment" data-fragment-index="2" -->
- What are we going to do about it?<!-- .element: class="fragment" data-fragment-index="3" -->
- Did we do a good job?<!-- .element: class="fragment" data-fragment-index="4" -->

<hr>

🕵🏻‍♂️ <!-- .element: class="fragment" data-fragment-index="5" -->[The Threat modeling Manifesto](https://www.threatmodelingmanifesto.org/)<!-- .element: class="fragment" data-fragment-index="5" -->

---

## On models

> "All models are wrong, some models are useful"</br> - [George Box](https://en.wikipedia.org/wiki/All_models_are_wrong).

We acknowledge that; models always fall short of the complexities of reality but can still be useful nonetheless.

---

## It starts with security requirements

- All systems should have defined and </br> documented security requirements (SR)!<!-- .element: class="fragment" data-fragment-index="1" -->
- SR will guide and inform our threat modeling.<!-- .element: class="fragment" data-fragment-index="2" -->
- In all/most organisations you can extract </br>security requirements from the governance<!-- .element: class="fragment" data-fragment-index="3" -->
- Threat modeling will trigger update of SR requirements<!-- .element: class="fragment" data-fragment-index="4" -->
- Additional sources for "inspiration"<!-- .element: class="fragment" data-fragment-index="5" -->
  - [OWASP SAAM](https://owaspsamm.org/)<!-- .element: class="fragment" data-fragment-index="5" -->
  - [OWASP ASVS](https://owasp.org/www-project-application-security-verification-standard/)<!-- .element: class="fragment" data-fragment-index="5" -->

<hr>

❓ What are typical security requirements in<!-- .element: class="fragment" data-fragment-index="7" --> <u>your context</u> ?<!-- .element: class="fragment" data-fragment-index="7" -->

---

## When to threat model?

- Threat Modeling of a system usually happens </br> **<u>in</u>** the early phases of the SDLC
- Threat modeling should include </br> every stage **<u>of</u>** the SDLC

<hr>

Threat modeling is much like brushing your teeth;</br> doing it often and in short sessions is the recommended way!
</br>(In case you wondered for brushing your teeth: 2x2)

---

## Basic terminology

- Weakness; is an underlying defect that modifies behaviour or functionality or allows unverified or incorrect access to data ([Common Weakness Enumeration](https://cwe.mitre.org/))
- Exploitability; is a measure of how easily an attacker can make use of a weakness to cause harm.
- Vulnerability; when a weakness is exploitable it is known as a vulnerability ([Common Vulnerability Enumeration](https://cve.mitre.org/))
- Severity; The potential damage and "blast radius" of a weakness to a system ([Common Vulnerability Scoring System](https://www.first.org/cvss/))

---

## Misconceptions

- "Think like an attacker" => </br>Serious work and structure<!-- .element: class="fragment" data-fragment-index="1" -->
- "You never done threat modeling" => </br>You do it all the time!<!-- .element: class="fragment" data-fragment-index="2" -->
- "Threat modeling is easy" => </br>Requires continuos planned effort to build a muscle.<!-- .element: class="fragment" data-fragment-index="3" -->
- "Threat modeling is for specialists" => </br> Every team role plays it's part, everyone should threat model<!-- .element: class="fragment" data-fragment-index="4" -->
- "Threat modeling as ONE skill ..." => </br> Threat modeling is experience, techniques (DFD, Stide,.. ), repertoire, (tools, books, blogs) ... just like software development<!-- .element: class="fragment" data-fragment-index="5" -->

---

## Rabbit holes

<div><!-- .element: style="font-size:0.8em"-->

- "Too much focus on how to TM (tools, frameworks, )..." => </br>Just do it! Focus on people, skills, perspectives, development, operations ...<!-- .element: class="fragment" data-fragment-index="1" -->
- "Admiring the problem" => </br> Go beyond and search for practical solutions<!-- .element: class="fragment" data-fragment-index="2" -->
- "Over focusing and going too deep" => </br>Maintain the bigger picture, avoid exaggerating attention on adversaries, assets or techniques.<!-- .element: class="fragment" data-fragment-index="3" -->
- "Searching for the perfect model" => </br>It does not exist! The better approach is multiple smaller models representing multiple views<!-- .element: class="fragment" data-fragment-index="4" -->

</div>

<hr>

❗️Threat modeling can be the most effective way to drive security through a product, service or system.<!-- .element: class="fragment" data-fragment-index="5" style="font-size:0.8em"- -->
