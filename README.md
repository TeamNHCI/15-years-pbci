# 15 Years of Passive BCI: Foundations and Frontiers

> **Repository accompanying the respective workshop at the 10th BCI Graz conference · 14 September 2026** <br>
> Workshop hosts: Thorsten Zander, Marius Klug | Chair for Neuroadaptive Human–Computer Interaction, BTU Cottbus–Senftenberg, Germany

---

## Table of Contents

1. [Motivation](#1-motivation)
2. [Mapping the challenges](#2-mapping-the-challenges)
   1. [Challenge clusters](#21-challenge-clusters)
   2. [Interconnectedness](#22-interconnectedness)
   3. [A Change of Perspective: From pBCI to NAT](#23-a-change-of-perspective-from-pbci-to-nat)
3. [Workshop: Challenge Synthesis](#3-workshop-challenge-synthesis)
4. [Next Steps](#4-next-steps)
5. [How to Work With This Repository](#5-how-to-work-with-this-repository)

---

## 1. Motivation

This repository was created in the scope of the workshop, but it is meant to serve a broader and longer-lasting purpose: to connect labs working on passive BCI and to help the field advance together.

Our shared goal is to move passive BCIs from the lab toward meaningful real-world applications. This is an inherently interdisciplinary endeavour — one that is best undertaken by combining the competencies of labs across Europe and beyond.

We use *meaningful* in a specific sense, with two conditions. First, the neural signal must make a unique, **non-substitutable** contribution — the same information cannot be obtained (more easily) from other measures such as eye tracking or overt behaviour. Second, the resulting system must **add value in a real-world task for real end users** — for example, supporting pilots as they operate an aircraft.

To that end, the repository serves two main purposes:

1. **Shared knowledge.** It communicates possible next steps and open challenges for the field while they are still being discussed. What follows is a substantiated draft, not a definitive document: it is meant to be read as something to build on, question, and extend.
2. **A place for exchange.** It offers a space for interaction and feedback with the community.

> A kind note on the scope of this repo: while the workshop spans both the *foundations* and the *frontiers* of passive BCI, this document concentrates on the frontiers, the open challenges.

---

## 2. Mapping the challenges 

The challenges outlined in the following were derived from recurrent, in-depth working sessions of our group — the **Neuroadaptive Human–Computer Interaction (NHCI)** group at **BTU Cottbus–Senftenberg** prior to the workshop. The core team consisted of:

1. Thorsten Zander (PI | BCI and NAT)
2. Marius Klug (group leader | cognitive neuroscience, signal processing, BCI)
3. David Trocellier (Postdoc | deep learning)
4. Gabriel Ivucic (Postdoc | signal processing)
5. Felix Schröder (Postdoc | cognitive neuroscience)
6. Atique Ahmed (PhD candidate | artificial intelligence)
7. Lucija Mihić Zidar (PhD candidate | cognitive neuroscience)
8. Lea Rabe (PhD candidate | human factors)

**The process began with a brainstorming session during which we collected the most pressing challenges for the field of passive BCI.** Each of us wrote down issues off the top of our heads. The raw issues were then discussed and clustered.

![Diagram of the challenge clustering process](images/challenge-clustering.png)

<!-- TODO: replace images/challenge-clustering.png with the actual image file committed to the repo, and update the alt text / caption -->
*From the brainstormed issues to the seven clusters.*

### 2.1 Challenge clusters

Through further discussions we grouped the individual challenges and organized them according to the following metaphor that emerged in the process: there are some challenges that form the basis of our work which, if addressed, will be beneficial to all other challenges. And then there are strands or *pillars* resting on this *foundation*. 

#### 2.1.1 Foundation "Common standards"

These challenges concern how research is conducted and connected, thereby defining the quality and impact of our output.

**Scientific rigor** — Ensuring sound methodology, valid ground truth, reproducibility, and robust evaluation, so that findings hold up and transfer beyond a single study.

*Examples:* _[add concrete examples here]_

**Community building** — Building connections between labs, sharing methods and standards, and broadening the range of expertise involved.

*Examples:* _[add concrete examples here]_

#### 2.1.2 Pillar I "Neural engineering"

The technical challenges of acquiring, processing, and decoding brain signals reliably. The focus is on turning raw neural activity into usable, generalizable information.

**Signal processing** — Acquiring, cleaning, and decoding brain signals reliably and in real time, under realistic noise and hardware constraints.

*Examples:* _[add concrete examples here]_

**Cognitive neuroscience** — Understanding the mental states and underlying neural processes that passive BCIs aim to detect.

*Examples:* _[add concrete examples here]_

**Universality** — Achieving generalization across users, sessions, tasks, and devices, while reducing calibration effort and improving transfer.

*Examples:* _[add concrete examples here]_

#### 2.1.3 Pillar II "Human factors"

The challenges of applying passive BCI meaningfully and responsibly in real-world settings. The focus is on who the technology is for and how its use affects people.

**Stakeholders and use cases** — Identifying who passive BCI is for and which real-world problems it should address, grounding development in concrete, realistic application scenarios.

*Examples:* _[add concrete examples here]_

**Ethics and legal** — Addressing privacy, informed consent, data protection, responsible use, and the evolving regulatory landscape.

*Examples:* _[add concrete examples here]_

### 2.2 Interconnectedness 

This clustering simplifies: the boundaries are porous, and a single piece of work rarely sits in just one cluster. A few examples:

- **Within a pillar** — signal processing and universality are hard to separate, since a decoding pipeline is only as general as its handling of noise and session-to-session variability.
- **Across pillars** — how much universality a system needs is set by its intended use case, and whatever it can decode raises questions of ethics and privacy.
- **Down to the foundation** — a claim about a mental state is only as trustworthy as its ground truth (scientific rigor), and generalizing across labs and datasets depends on shared standards and data (community building).

The clusters are not sealed compartments, but a way to locate a piece of work and see what it touches.

### 2.3 A Change of Perspective: From pBCI to NAT

Taken together, the clusters and their entanglement lead us to one conclusion: passive BCI cannot be advanced piecemeal. We think a shift in perspective is warranted — away from viewing the work narrowly, and toward recognizing that whatever specific challenge we tackle, we are ultimately working on an *interface*. Improving an interface, we would argue, means embracing a more holistic picture of it, one that includes the user, the system, and the loop between them.

Concretely, we see this as a shift from passive BCI as a **decoding problem** — reading a state out of the brain — to **Neuroadaptive Technology (NAT)**, where the brain-derived state is fed back into a system that *adapts* to the user in a closed loop. It changes the question we ask from "how accurately can we classify this state?" to "how should the system respond, and how do human and machine co-adapt over time?" We would urge researchers to frame their work as the whole interface rather than the signal alone — it is what opens the door to implicit control, personalization, and systems that learn from the user during use.

---

## 3. Workshop: Challenge Synthesis

> _[Placeholder — content will be synthesized and updated after the workshop.]_


---

## 4. Next Steps

The work does not end with the workshop. The immediate next steps are:

1. **Synthesize the workshop.** The results of the workshop will be synthesized and uploaded here.
2. **Merge internal and expert insights.** We will combine the insights we developed internally (see [Section 2](#2-mapping-the-challenges)) with the expert perspectives gained at the workshop, to pinpoint blind spots, shifts in emphasis, and overlaps.
3. **Work toward a published guideline.** Ultimately, we aim to develop a published guideline for the field — one that specifically targets the question of how meaningful integration of passive BCIs into real-world contexts can be realized within the next ten years.

---

## 5. How to Work With This Repository

There are three main ways to engage with this repository:

- **Share it.** Pass it on to researchers and colleagues who work on — or are curious about — passive BCI and neuroadaptive technology.
- **Give feedback.** Share your thoughts, comments, and corrections — including anything you think is missing or wrong. The easiest way is to [open an Issue](../../issues).
- **Become a contributor.** If you'd like to get more closely involved in the project, get in touch — we welcome new collaborators.

> _[Placeholder — add a short feedback guideline here. For example: how to open an issue, what information to include, whether to label it, or an email address for those who prefer to reach out directly.]_

---

<!-- Optional footer: license, citation, acknowledgements, contact -->
