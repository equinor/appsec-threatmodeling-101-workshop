<!-- markdownlint-disable MD033 -->

# What are we working on? </br> 🏗

---

## Exercise 0

❓ What pops into your head about "windows"? <!-- .element: class="fragment" data-fragment-index="1" -->

- Write it down silently (1 minute) <!-- .element: class="fragment" data-fragment-index="1" -->
- What did you write down? <!-- .element: class="fragment" data-fragment-index="2" -->

---

## Purpose of ™️Models / Diagrams

- Diagrams expose thinking and triggers discussions<!-- .element: class="fragment" data-fragment-index="1" -->
- Diagrams are scoping tools </br>(what's in, out, boundaries)<!-- .element: class="fragment" data-fragment-index="2" -->
- Scope may be this sprint, this story,</br> this project, this feature, .....<!-- .element: class="fragment" data-fragment-index="3" -->

<hr>

🏁 Pick up a pen and start drawing, </br>tell a story, show data flow and boundaries<!-- .element: class="fragment" data-fragment-index="4" -->

---

## DFD (Data Flow Diagrams)

- Threats often follow data => Data Flow Diagrams
- DFD are simple, easy to learn and sketch
- Whiteboards are excellent tools

<hr>

❗️We use data flow diagrams because they provide us with a simple representation of how data, and thus threats, flow through a system.

---

## DFD components

<img src="./content/images/dfd.png">

---

## DFD - An Example

<img src="./content/images/dfd-example.png">

---

## Trust boundaries

<div><!-- .element: style="font-size:0.8em"-->

- Trust boundaries is where entities/principals<!-- .element: class="fragment" data-fragment-index="1" --> <a style="color:red">with different privileges</a> interact, talk to each other<!-- .element: class="fragment" data-fragment-index="1" -->
- A<!-- .element: class="fragment" data-fragment-index="2" --> [principal](https://en.wikipedia.org/wiki/Principal_(commercial_law)<!-- .element: class="fragment" data-fragment-index="2" --> (a noun): Someone, something that is authorized to act as an agent/representative. It could be users, UID's, apps, service principals, devices, deployment instances, physical data centers .... <!-- .element: class="fragment" data-fragment-index="2" -->
- A principal is often the smallest unit you can name in a policy (iam object in access policies, UID's on a desktop/server) <!-- .element: class="fragment" data-fragment-index="3" -->
- Trust boundaries needs to be explicit about what, where, how. <!-- .element: class="fragment" data-fragment-index="4" -->
- Trust boundaries needs info/agreements on the mechanism that isolates them, on how to enforce, configure and test them <!-- .element: class="fragment" data-fragment-index="5" -->
- Trust boundaries should be labeled <!-- .element: class="fragment" data-fragment-index="6" -->

<hr>

💡 Examples: File permission - enforced by kernel, network hosts - enforced by firewall, app permissions - enforced by IAM and app <!-- .element: class="fragment" data-fragment-index="7" -->

</dev>

---

## What artifacts/models do we  record/store?

<div><!-- .element: style="font-size:0.8em"-->

- Think lifecycle and maintenance for models and artifacts,</br> store some for the records - some for keeping up-to-date?<!-- .element: class="fragment" data-fragment-index="1" -->
- Effort grows with formality, <!-- .element: class="fragment" data-fragment-index="2" --></br> legal requirements, regulations, GDPR, ++ <!-- .element: class="fragment" data-fragment-index="2" -->
- Store with code, in separate repos, in sharepoint, ...? </br>Explore options. Some data could be sensitive<!-- .element: class="fragment" data-fragment-index="5" -->

<hr>

Examples:<!-- .element: class="fragment" data-fragment-index="5" -->

- Whiteboard => Pictures or Drawings (draw.io) stored with project<!-- .element: class="fragment" data-fragment-index="5" -->
- Collaborative tools like Miro could be ok<!-- .element: class="fragment" data-fragment-index="6" -->
  - Don't underestimate the learning curve and the "tool trap"!<!-- .element: class="fragment" data-fragment-index="6" -->
  - Provide some Miro training before starting to TM<!-- .element: class="fragment" data-fragment-index="6" -->
  - Remember information sensitivity!
- External systems like<!-- .element: class="fragment" data-fragment-index="7" --> [Irus Risk](https://www.iriusrisk.com/)<!-- .element: class="fragment" data-fragment-index="7" -->, [OWASP Threat Dragon](https://owasp.org/www-project-threat-dragon/)<!-- .element: class="fragment" data-fragment-index="7" -->, [Draw.io](https://draw.io)<!-- .element: class="fragment" data-fragment-index="7" -->

</div>

---

## Exercise 1 - Creating a model

---

## Organizing groups and work

- We form groups (4-5 persons)
- The group will stay together for all exercises
- The exercises build on each other
- We draw on A3 sheets (boards, flip-overs or similar)
- We use thick-✏️ when drawing (it's easier to read) 
- We make notes on paper
- Groups take a picture of drawings and notes and share in Slack channel [#appsec-threatmodeling-workshop](https://equinor.slack.com/archives/C046T5B84P4) before presenting
  - We will delete most of these posts from the Slack channel after the workshop
- Make sure to take a short round of introduction in the groups 🤝

🚶🏼Reshuffle groups now if needed 🚶🏿‍♀️

---

## Our example system

<img src="./content/images/tm-example-system.png">

---

## EX-1: Drawing a data flow diagram

<div><!-- .element: style="font-size:0.7em;text-align:left"-->

<hr>

Tasks:

For our [example system](content/images/tm-example-system.png)

- Examine the system, the assumptions and security requirements
- <a style="color:red">Draw a DFD for the system</a>
- <a style="color:red">Document any assumptions you make</a>
- Take a picture of your DFD, share on Slack </br>and prepare to present the model to the class

The person in the group which has the next birthday becomes group lead for this exercise.

<hr>

⏰ Time boxed schedule (20m):

- 3 minutes to discuss and clarify system
- 15 minutes to create DFD
- 2 minutes to take picture and share on Slack

<hr>

Remember: "All models are wrong. Some models are useful"

</div>

---

## EX1: Presenting models

Each group present their DFD along with assumptions

<hr>

❓Reflections, Observations, Learning
