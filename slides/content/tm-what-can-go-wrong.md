<!-- markdownlint-disable MD033 -->

# What can go wrong? </br>💥

---

## Introducing [STRIDE](https://en.wikipedia.org/wiki/STRIDE_(security))

STRIDE is a model for identifying computer security threats. It provides the following mnemonic: <!-- .element: style="font-size:0.65em"-->

 <table><!-- .element: style="font-size:0.60em"-->
  <tr>
    <th>Threat</th>
    <th>Violates</th>
    <th>Definition</th>
    <th>Example</th>
  </tr>
  <tr>
    <td>Spoofing</td>
    <td>Authentication</td>
    <td>Impersonating someone or something</td>
    <td>Pretending to be you manager, a CFO, bankid.no, ntdll.dll, expressJs</td>
  </tr>
  <tr>
    <td>Tampering</td>
    <td>Integrity</td>
    <td>Modify data and code</td>
    <td>Modifying a file, changing code in a NPM repo, change a packet as it traverses the network, change a binary</td>
  </tr>
  <tr>
    <td>Repudiation</td>
    <td>Non-repudiation </br>Accountability</td>
    <td>Claiming to not have performed an action</td>
    <td>"I did not send that email", "I did not make that change"</td>
  </tr>
  <tr>
    <td>Information disclosure</td>
    <td>Confidentiality</td>
    <td>Exposing information to someone not authorised to see it</td>
    <td>Publish a list of customers to a web site, allowing someone to read source code</td>
  </tr>
  <tr>
    <td>Denial of service</td>
    <td>Availability</td>
    <td>Deny or degrade service to users</td>
    <td>Crashing a web site, eat all memory for a program, route packages to void</td>
  </tr>
  <tr>
    <td>Elevation of privilege</br>(Expansion of Authority)</td>
    <td>Authorization</td>
    <td>Gain capabilities without proper authorization</td>
    <td>Allowing a remote internet user to run commands, XSS, SQL Injection, RCE, going from limited to admin user</td>
  </tr>  
</table>

---

## How to use STRIDE?

<div><!-- .element: style="font-size:0.7em"-->

- Use mnemonic to identify threats to system<!-- .element: class="fragment" data-fragment-index="1" -->
- Ask: How could this S,T,R,I,D,E impact the system?<!-- .element: class="fragment" data-fragment-index="2" -->
- Ways to use:<!-- .element: class="fragment" data-fragment-index="3" -->
  - Follow a story through the diagram,<!-- .element: class="fragment" data-fragment-index="4" --> </br>look for STRIDE threats, iterate<!-- .element: class="fragment" data-fragment-index="4" -->
  - Focus on an element, component, parts of a system </br>and apply STRIDE<!-- .element: class="fragment" data-fragment-index="5" -->
  - Looping the diagram:<!-- .element: class="fragment" data-fragment-index="6" -->
    - For elements in diagram -> for each threat (STRIDE) -> specify how threat to element works<!-- .element: class="fragment" data-fragment-index="7" -->
    - For threat in (STRIDE) -> for element in diagram -> specify how threat to element works<!-- .element: class="fragment" data-fragment-index="8" --> 
- As you learn -> iterate<!-- .element: class="fragment" data-fragment-index="9" -->

</div>

<hr>

❗️There are quite a few alternatives to STRIDE. We choose to focus on STRIDE when introducing Threat Modeling to teams. It has proven to be useful in many relevant scenarios.<!-- .element: style="font-size:0.7em"--><!-- .element: class="fragment" data-fragment-index="10" -->

---

## STRIDE per element

<table><!-- .element: style="font-size:0.8em"-->
    <tr>
        <th>Part</th>
        <th>Spoof</th>
        <th>Tamper</th>
        <th>Repudiation</th>
        <th>Info disclosure</th>
        <th>Deny Service</th>
        <th>EoP</th>
    </tr>
    <tr>
        <td>External entity</td>
        <td align="center">X</td>
        <td align="center"></td>
        <td align="center">X</td>
        <td align="center"></td>
        <td align="center"></td>
        <td align="center"></td>
    </tr>
    <tr>
        <td>Process</td>
        <td align="center">X</td>
        <td align="center">X</td>
        <td align="center">X</td>
        <td align="center">X</td>
        <td align="center">X</td>
        <td align="center">X</td>
    </tr>
    <tr>
        <td>Data store</td>
        <td align="center"></td>
        <td align="center">X</td>
        <td align="center">?</td>
        <td align="center">X</td>
        <td align="center">X</td>
        <td align="center"></td>
    </tr>
    <tr>
        <td>Dataflow</td>
        <td align="center"></td>
        <td align="center">X</td>
        <td align="center"></td>
        <td align="center">X</td>
        <td align="center">X</td>
        <td align="center"></td>
    </tr>

</table>

<hr>

🕵🏻‍♂️ The [Elevation of Privileges game](https://github.com/adamshostack/eop) is helpful and fun. We plan a follow-up workshop on EoP.

---

## Tracking threats and assumptions

- Track issues as they are found<!-- .element: class="fragment" data-fragment-index="1" -->
- Track assumptions as they are discoverd<!-- .element: class="fragment" data-fragment-index="2" -->
- Issues and assumptions are input to<!-- .element: class="fragment" data-fragment-index="3" --> </br>"What are we going to do about it?"<!-- .element: class="fragment" data-fragment-index="3" -->
- Recommended practice:<!-- .element: class="fragment" data-fragment-index="4" -->
  - Appoint a note taker<!-- .element: class="fragment" data-fragment-index="5" -->
  - Record meetings / sessions<!-- .element: class="fragment" data-fragment-index="6" -->
  - Create a team strategy for how to </br>document, where to store etc...<!-- .element: class="fragment" data-fragment-index="7" -->

<hr>

❗️The best tools are the one that works for the people involved, for the project you are working on!<!-- .element: class="fragment" data-fragment-index="8" -->

---

## What could go wrong - brainstorming

(As an alternative/add-on to using STRIDE)<!-- .element: style="font-size:0.6em"-->

Some useful questions/statements:

- "What is The one thing you are worried about?"<!-- .element: class="fragment" data-fragment-index="1" -->
- "How would you attack your system?"<!-- .element: class="fragment" data-fragment-index="2" -->
- "Fortunately/unfortunately"<!-- .element: class="fragment" data-fragment-index="3" -->
- "Remember we have technical/security debt?"<!-- .element: class="fragment" data-fragment-index="4" -->
- "Last iteration we made this temporary solution ...."<!-- .element: class="fragment" data-fragment-index="5" -->

<hr>

❗️There are many guides and books available discussing the mechanics of threats. There are threats libraries available. It's usually a good idea to augment our threat modeling with these aids after we have reached a bit of maturity<!-- .element: class="fragment" data-fragment-index="6" -->

---

## Exercise 2 - Identifying threats

---

## EX-2: Applying STRIDE

<hr>

<div align="left"><!-- .element: style="font-size:0.8em"-->

Tasks:

For our example system, using your DFD for whats currently implemented:

- Apply STRIDE, document issues, assumptions and threats
- (Use the EoP Card Game?)
- Team decide scope, iterating as you learn is smart!
- Document in word/text-editor/paper (format suggested 👇)
- Prepare to present threats to class

<hr>

Time boxed schedule (35m):

- 30 minutes to apply STRIDE
- 5 minutes complete - wrap-up

<hr>

💡 Try to avoid rabbit holes. Stop early. Iterate

</div>

---

## EX-2: Document <u>example</u>

<table><!-- .element: style="font-size:0.65em"-->
    <tr>
        <th>Part</th>
        <th>STRIDE</th>
        <th>Threat action</th>
        <th>Impact</th>
        <th>#</th>
    </tr>
    <tr>
        <td>Web app</td>
        <td>Spoof</td>
        <td>Attacker steals session cookie</td>
        <td>Information disclosure, access to all emails</td>
        <td>1</td>
    </tr>
    <tr>
        <td>Token Cache</td>
        <td>Information disclosure</td>
        <td>Attacker is stealing O365 access tokens</td>
        <td>Information disclosure, system integrity, GDPR ...</td>
        <td>2</td>
    </tr>
    <tr>
        <td>..</td>
        <td align="center">..</td>
        <td align="center">..</td>
        <td align="center">..</td>
        <td align="center">3</td>
    </tr>
    <tr>
        <td>..</td>
        <td align="center">..</td>
        <td align="center">..</td>
        <td align="center">..</td>
        <td align="center">4</td>
    </tr>
</table>

<div align="left"><!-- .element: style="font-size:0.6em"-->

Assumptions:

- There are no key stores used
- Storage - VM discs are not encrypted

Issues:

- Should internal traffic be https as well?
- What about PKI infrastructure?
  
</div>

---

## EX-2: Presenting threats

Each group present their key assumptions, issues and threats

<hr>

❓Reflections, Observations, Learning