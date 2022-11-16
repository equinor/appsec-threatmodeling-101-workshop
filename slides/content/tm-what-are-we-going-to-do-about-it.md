<!-- markdownlint-disable MD033 -->

# What are we going to do about it? </br>🩺

Tactics, Strategies, Alignment, Prioritisation, Documentation<!-- .element: style="font-size:0.7em"-->

---

## Addressing threats

- Address each threat - decide on strategy/tactics, document<!-- .element: class="fragment" data-fragment-index="1" -->
- Strategies are: eliminate, accept, transfer or mitigate<!-- .element: class="fragment" data-fragment-index="3" -->
  - Eliminate; tactic:remove -> example: remove code, component...<!-- .element: class="fragment" data-fragment-index="4" -->
  - Accept; tactic: document acceptance, transfer risk to customer?<!-- .element: class="fragment" data-fragment-index="5" -->
  - Transfer; tactic: "UI,license,insurance,..", document and track<!-- .element: class="fragment" data-fragment-index="6" -->
  - Mitigate; tactic: add controls<!-- .element: class="fragment" data-fragment-index="7" -->
- Check/verify assumptions<!-- .element: class="fragment" data-fragment-index="8" -->

<hr>

💡Threat vs. Risk: A threat is a future problem. A risk is a threat with probability and impact. We do not need probability and impact to manage threats!<!-- .element: class="fragment" data-fragment-index="8" -->

---

## Mitigation

<div><!-- .element: style="font-size:0.8em"-->

- To mitigate means to add controls that address the threat<!-- .element: class="fragment" data-fragment-index="1" -->
- Controls are features or technologies<!-- .element: class="fragment" data-fragment-index="2" -->
  - Use technology before people or process!<!-- .element: class="fragment" data-fragment-index="2" -->
  - Protect, detect or respond to threats<!-- .element: class="fragment" data-fragment-index="3" -->
- Mitigation tactics could be<!-- .element: class="fragment" data-fragment-index="4" -->
  - Code by developers<!-- .element: class="fragment" data-fragment-index="5" -->
  - Signals to operations<!-- .element: class="fragment" data-fragment-index="6" -->
  - Products / services<!-- .element: class="fragment" data-fragment-index="7" -->
  - Complete or partial<!-- .element: class="fragment" data-fragment-index="8" -->
  - Strong or weak<!-- .element: class="fragment" data-fragment-index="9" -->
- The right tactics will always be situational/context dependent<!-- .element: class="fragment" data-fragment-index="10" -->
- Custom controls = New Security Tech - avoid?<!-- .element: class="fragment" data-fragment-index="11" -->
- Explore standard as the first choice<!-- .element: class="fragment" data-fragment-index="11" -->

<hr>

💡<!-- .element: class="fragment" data-fragment-index="12" -->[OWASP Proactive Controls](https://owasp.org/www-project-proactive-controls/)<!-- .element: class="fragment" data-fragment-index="12" -->

</div>
---

## Managing "What are we going to do about it"

<div><!-- .element: style="font-size:0.7em"-->

- Document<!-- .element: class="fragment" data-fragment-index="2" -->
  - Write down and track (use teams tool chain)<!-- .element: class="fragment" data-fragment-index="2" -->
  - Track as bugs, features, security stories, security debt<!-- .element: class="fragment" data-fragment-index="2" -->
- Prioritize<!-- .element: class="fragment" data-fragment-index="3" -->
  - Align with reality, team, product owner<!-- .element: class="fragment" data-fragment-index="4" -->
  - Prioritization always includes effort to fix - and operate.<!-- .element: class="fragment" data-fragment-index="5" -->
  - Agree on severity categories: </br>example sev1 means fix ASAP, sev2 means within 7 days ....<!-- .element: class="fragment" data-fragment-index="6" -->
- Implement<!-- .element: class="fragment" data-fragment-index="7" -->
  - Add to team backlog<!-- .element: class="fragment" data-fragment-index="8" -->
  - Don't re-invent the wheel<!-- .element: class="fragment" data-fragment-index="9" -->
  - Assessing implementation will be a lot easier if</br> a larger part of team participate in threat modeling<!-- .element: class="fragment" data-fragment-index="10" -->
  - Code tests to identify - provoke - trigger controls, signals to operations etc.<!-- .element: class="fragment" data-fragment-index="11" -->

</div>

---

## Exercise 3 - Managing Threats

---

## EX-3: Threat management

<div align="left"> <!-- .element: style="font-size:0.7em"-->

<hr>

Tasks:

For some of the threats identified in the previous exercise:

- Select a strategy; at least a few should be "mitigation"
- Discuss realistic fix'es and document them (controls)
- Document format suggested (👇)
- Take a picture of your documents, share on Slack </br>and prepare to present the model to the class

<hr>

⏰ Time boxed schedule (20m):

- 20 minutes to discuss what to do about threats

</div>

---

## EX-3: Document <u>example</u>

<table><!-- .element: style="font-size:0.7em"-->
    <tr>
        <th>ID</th>
        <th>Threat #</th>
        <th>Threat summary</th>
        <th>Strategy</th>
        <th>Fix idea</th>
        <th>Pros/Cons</th>
    </tr>
    <tr>
        <td>1</td>
        <td>Stolen session cookie from front end</td>
        <td>An attacker is able to steal the session cookie of a valid user session</td>
        <th>Mitigate</th>
        <td>Assess terminating session if sudden change in access ip</td>
        <td>Pro: Could fix the problem</br>Con:May introduce errors if user is access from multiple clients</td>
    </tr>
    <tr>
        <td>2</td>
        <td>Token cache exposure</td>
        <td>An attacker is able to access token cache on the back-end and thus access service impersonation a user/service</td>
        <th>Mitigate</th>
        <td>Move token cache to external service, encrypt, add logging of all access, lock down permissions</td>
        <td>Pro: Would reduce the risk</br>Con: Adds complexity, cost and skills need in team</td>
    </tr>
    <tr>
        <td>3</td>
        <td align="center">..</td>
        <td align="center">..</td>
        <td align="center">..</td>
        <td align="center">..</td>
        <td align="center">..</td>
    </tr>
    <tr>
        <td>4</td>
        <td align="center">..</td>
        <td align="center">..</td>
        <td align="center">..</td>
        <td align="center">..</td>
        <td align="center">..</td>
    </tr>
</table>

<div align="left">

---

## EX-3: Presentations

Each group present their threats

- Threats
  - Strategies
  - Fix ideas
  - Pros/Cons
- How were the Security Requirements used?

<hr>

❓Reflections, Observations, Learning

---

## How to prioritise threats?

<div><!-- .element: style="font-size:0.9em"-->

Threat vs. Risk:

- A threat is a future problem.<!-- .element: class="fragment" data-fragment-index="1" -->
- A risk as a threat with probability and impact.<!-- .element: class="fragment" data-fragment-index="1" -->
- We do not need probability and impact to manage threats!<!-- .element: class="fragment" data-fragment-index="1" -->

<hr>

- Some threats should be prioritized by the team (a team decision)<!-- .element: class="fragment" data-fragment-index="5" -->
  - Find guidance in the security requirements<!-- .element: class="fragment" data-fragment-index="5" -->
- Some threats MUST involve the business/product owner in prioritising<!-- .element: class="fragment" data-fragment-index="6" -->
- Business/Product Owner, Team and potentially other support should be involved with "identifying" threats<!-- .element: class="fragment" data-fragment-index="6" -->
- Important to know "who owns the risk and can accept it on behalf of the company?"<!-- .element: class="fragment" data-fragment-index="7" -->

<hr>

❓ Reflections<!-- .element: class="fragment" data-fragment-index="8" -->

<div>
