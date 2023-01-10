<!-- markdownlint-disable MD033 -->

# Threat modeling Introduction </br>🖖

---

## What is threat modeling?

From the Threat Modeling Manifesto:<!-- .element: style="font-size:0.8em"-->
> Threat modeling is analyzing representations of a system to highlight concerns about security and privacy characteristics.

Ideally, we want to identify weaknesses as early as possible.<!-- .element: class="fragment" data-fragment-index="1" -->

❗️Threat modeling "must" be a cyclic/continuous effort,</br> not a one off activity.<!-- .element: class="fragment" data-fragment-index="2" -->

---

## Why Threat modeling?

- Develop more secure systems (what we develop)<!-- .element: class="fragment" data-fragment-index="1" -->
- Develop more securely (how we develop)<!-- .element: class="fragment" data-fragment-index="2" -->
- Operate more securely (how we operate)<!-- .element: class="fragment" data-fragment-index="3" -->
- Recognize what can go wrong in a system<!-- .element: class="fragment" data-fragment-index="4" -->
- Pinpoint design and implementation issues<!-- .element: class="fragment" data-fragment-index="5" -->
- Enabled informed decisions on threats and mitigations.<!-- .element: class="fragment" data-fragment-index="6" -->
- Educate developers and teams, share knowledge<!-- .element: class="fragment" data-fragment-index="7" -->
- Have a systematic and consistent approach to security<!-- .element: class="fragment" data-fragment-index="8" -->

❗️Threat modeling will guide our designs </br>and help us make decisions with our eyes open.<!-- .element: class="fragment" data-fragment-index="9" -->

<hr>

❓ What are your<!-- .element: class="fragment" data-fragment-index="9" --> <u>current</u> reasons for wanting to Threat Model?<!-- .element: class="fragment" data-fragment-index="9" -->

---

## The 4 Key Questions of Threat modeling

- What are we working on?<!-- .element: class="fragment" data-fragment-index="1" -->
- What can go wrong?<!-- .element: class="fragment" data-fragment-index="2" -->
- What are we going to do about it?<!-- .element: class="fragment" data-fragment-index="3" -->
- Did we do a good job?<!-- .element: class="fragment" data-fragment-index="4" -->

<hr>

🕵🏻‍♂️ <!-- .element: class="fragment" data-fragment-index="5" -->[The Threat modeling Manifesto](https://www.threatmodelingmanifesto.org/)<!-- .element: class="fragment" data-fragment-index="5" -->

---

## On models

> "All models are wrong, some models are useful"</br> - [George Box](https://en.wikipedia.org/wiki/All_models_are_wrong).

We acknowledge that; models always fall short of the complexities of reality - but can still be useful nonetheless.

---

## It starts with security requirements

<div><!-- .element: style="font-size:0.75em"-->

- All systems must have documented security requirements (SR)!<!-- .element: class="fragment" data-fragment-index="1" -->
- SR will guide and inform our threat modeling.<!-- .element: class="fragment" data-fragment-index="2" -->
- In all/most organisations the governance</br> will be a good starting point for identifying SR<!-- .element: class="fragment" data-fragment-index="3" -->
- Legal and governmental requirements will also provide SR<!-- .element: class="fragment" data-fragment-index="3" -->
- Threat modeling will often trigger update of SR requirements<!-- .element: class="fragment" data-fragment-index="4" -->
- External sources for "inspiration"<!-- .element: class="fragment" data-fragment-index="5" -->
  - [OWASP ASVS](https://owasp.org/www-project-application-security-verification-standard/)<!-- .element: class="fragment" data-fragment-index="5" -->
  - [OWASP MASVS - Mobile AppSec](https://mas.owasp.org/)<!-- .element: class="fragment" data-fragment-index="5" -->
  - [OWASP Top-10](https://owasp.org/www-project-top-ten/)<!-- .element: class="fragment" data-fragment-index="5" -->
  - [OWASP API Top-10](https://owasp.org/www-project-api-security/)<!-- .element: class="fragment" data-fragment-index="5" -->
  - [OWASP SAAM](https://owaspsamm.org/model)<!-- .element: class="fragment" data-fragment-index="5" -->
  - [OpenSSF Scorecard](https://securityscorecards.dev/)<!-- .element: class="fragment" data-fragment-index="5" -->

</div>

<hr>

❓ What are typical security requirements in<!-- .element: class="fragment" data-fragment-index="7" --> <u>your context</u> ?<!-- .element: class="fragment" data-fragment-index="7" -->

---

## When to threat model?

<div style="display: grid;grid-column-gap: 1%; grid-auto-columns: 50% 50%;">

<div  style="grid-area: 1 / 1"><!-- .element: style="font-size:0.9em"-->

<hr>

- Threat Modeling of a system usually happens in the early phases of the SDLC (DevOps)
- Threat Modeling must include the system and the SDLC (The DevOps Cycle)
- Threat Modeling must be a continuous effort

</div>

<div  style="grid-area: 1 / 2"><img src="./content/images/devops.png" width="100%" height="auto" display="block" margin-left="auto" margin-right="auto">
</div>

</div>

<hr>

Threat modeling is much like brushing your teeth 🪥;</br> - daily short sessions -

---

## Basic terminology

- Weakness; is an underlying defect that modifies behaviour or functionality or allows unverified or incorrect access to data ([Common Weakness Enumeration](https://cwe.mitre.org/))
- Exploitability; is a measure of how easily an attacker can make use of a weakness to cause harm.
- Vulnerability; when a weakness is exploitable it is known as a vulnerability ([Common Vulnerability Enumeration](https://cve.mitre.org/))
- Severity; The potential damage and "blast radius" of a weakness to a system ([Common Vulnerability Scoring System](https://www.first.org/cvss/))
- Threat; A future problem, the possibility that something unwanted will happen

---

## Misconceptions

- "Think like an attacker" => </br>Who knows how an attacker think?</br>Focus on serious work, structure and consistency<!-- .element: class="fragment" data-fragment-index="1" -->
- "You never done threat modeling" => </br>You do it all the time!<!-- .element: class="fragment" data-fragment-index="2" -->
- "Threat modeling is easy" => </br>No, it requires continuos planned effort to build a muscle.<!-- .element: class="fragment" data-fragment-index="3" -->
- "Threat modeling is for specialists" => </br>No, every team role plays it's part, everyone should participate<!-- .element: class="fragment" data-fragment-index="4" -->
- "Threat modeling as ONE skill ..." => </br> Threat modeling is experience, techniques (DFD, STRIDE,.. ), repertoire, (tools, books, blogs) ... just like software development, it's more than knowing a development language<!-- .element: class="fragment" data-fragment-index="5" -->

---

## Rabbit holes

<div><!-- .element: style="font-size:0.8em"-->

- "Too much focus on "how-to" TM (tools, frameworks, )..." => </br>Just do it! Focus on people, skills, perspectives, development, operations ...<!-- .element: class="fragment" data-fragment-index="1" -->
- "Admiring the problem, going too deep" => </br>Maintain the bigger picture, avoid exaggerating attention on problem, adversaries, assets or techniques.<!-- .element: class="fragment" data-fragment-index="2" -->
- "Searching for the perfect model" => </br>It does not exist! The better approach is multiple smaller models representing multiple views?<!-- .element: class="fragment" data-fragment-index="4" -->

</div>

<hr>

❗️Threat modeling can be the most effective way to drive security through a product, service or system.<!-- .element: class="fragment" data-fragment-index="5" style="font-size:0.8em"- -->
