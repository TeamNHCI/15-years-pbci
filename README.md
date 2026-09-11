# 15 Years of Passive BCI: Foundations and Frontiers

> **Repository accompanying the respective workshop at the 10th BCI Graz conference · 14 September 2026** <br>
> Workshop hosts: Thorsten Zander, Marius Klug | Chair for Neuroadaptive Human–Computer Interaction, BTU Cottbus–Senftenberg, Germany

---

## Table of Contents

1. [Motivation](#1-motivation)
2. [Mapping Core Challenges](#2-mapping-core-challenges)
   1. [Challenge Clusters](#21-challenge-clusters)
   2. [Interconnectedness](#22-interconnectedness)
   3. [Call for Change of Perspective](#23-call-for-a-change-of-perspective)
3. [Workshop: Challenge Synthesis](#3-workshop-challenge-synthesis)
4. [Next Steps](#4-next-steps)
5. [How to Work With This Repository](#5-how-to-work-with-this-repository)

---

## 1. Motivation

This repository was created in the scope of the workshop, but it is meant to serve a broader and longer-lasting purpose: **to connect labs working on passive BCI and to help the field advance together**.

Our shared goal is to move passive BCIs from the lab toward *meaningful* real-world applications. This is an inherently interdisciplinary endeavour — one that is best undertaken by combining the competencies of labs across Europe and beyond.

With *"meaningful"* we imply two requirements: First, the neural signal must make a unique, **non-substitutable** contribution - the same information cannot be obtained (more easily) from other measures such as eye tracking or overt behaviour. Second, the resulting system must **add value in a real-world task for real end users**.

To that end, the repository serves two main purposes:

1. **Shared knowledge.** It communicates possible next steps and open challenges for the field while they are still being discussed. What follows is a substantiated draft, not a definitive document: it is meant to be read as something to build on, question, and extend.
2. **A place for exchange.** It offers a space for interaction and feedback with the community.

> A kind note on the scope of this repo: while the workshop spans both the *foundations* and the *frontiers* of passive BCI, this document concentrates on the latter.

---

## 2. Mapping Core Challenges 

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

<p align="center">
  <img src="/vision-meeting-brainstorming.jpeg" alt="Brainstorming kick-off to gather challenges" width="50%">
</p>
<p align="center"><em>Brainstorming of issues in the pBCI field. Each card represents a challenge, cards are sorted into different topical bins. © Felix Schröder</em></p>


### 2.1 Challenge Clusters

Through further discussions we grouped the individual challenges and organized them according to the following metaphor that emerged in the process: there are some challenges that form the basis of our work which, if addressed, will be beneficial to all other challenges. And then there are strands or *pillars* resting on this *foundation* that are necessary to achieve the goal of a meaningfully applied passive BCI. 

<p align="center">
  <img src="/foundation-pillars.svg" alt="Overview of challenges clustered based on the foundation and pillar logic introduced above." width="80%">
</p>
<p align="center"><em>Fig. 1: Overview of broad challenge clusters.</em></p>


#### 2.1.1 Foundation "Common standards"

These challenges concern how research is conducted and connected, thereby defining the quality and impact of our output.

**a) Scientific rigor** — Ensuring sound methodology, valid ground truth, reproducibility, and robust evaluation, so that findings hold up and transfer beyond a single study.

*Example:* While cross-validation is widely accepted to validate classifier outputs, the visualization of neurophysiological patterns informing the classifiers is not, eventhough valuable insights can be gained (e.g. distinguishing brain from muscle sources). The field might benefit from widely accepted gold standards to validate results. 

**b) Community building** — Building connections between labs, sharing methods and standards, and broadening the range of expertise involved.

*Example:* Standards can only be widely accepted and communicated if a solid network of labs exists that fosters such exchange. We think a network, potentially formalized through a society, would overcome silo-effects while also increasing quality and impact of our research.

#### 2.1.2 Pillar I "Neural engineering"

The technical challenges of acquiring, processing, and decoding brain signals reliably. The focus is on turning raw neural activity into usable, generalizable information.

**a) Signal processing** — Acquiring, cleaning, and decoding brain signals reliably and in real time, under realistic noise and hardware constraints.

*Example:* To apply EEG in real-world contexts, we will most likely work with low-density form factors to record brain activation. Current artifact handling methods, such as ICA, rely on full head coverage. Therefore we must compare and find solutions that work reliably with low density setups and that, ideally, are form factor-agnostic. 

**b) Cognitive neuroscience** — Understanding the mental states and underlying neural processes that passive BCIs aim to detect.

*Example:* So far we don't have a clear understanding about the transferability of classifiers, that is how well a classifier trained on a specific mental state can be applied in different scenarios eliciting the same mental state (cross-task, within subject). We believe a deeper understanding of the cognitive and neural underpinnings is a crucial step in order to achieve reliable cross-task classifiers. 

**c) Universality** — Achieving generalization across users, sessions, tasks, and devices, while reducing calibration effort and improving transfer.

*Example:* For some real-world scenarios, it will be a challenge or impossible to derive event markers. How can we build classifiers then, that can be applied continuously, without markers?

#### 2.1.3 Pillar II "Human factors"

The challenges of applying passive BCI meaningfully and responsibly in real-world settings. The focus is on who the technology is for and how its use affects people.

**a) Stakeholders and use cases** — Identifying who passive BCI is for and which real-world problems it should address, grounding development in concrete, realistic application scenarios.

*Example:* The (rare) studies that test paradigms with real users in real settings, usually come from a neural engineering angle (does the classifier work in a realisitc scenario?). Whereas, the user's perspective on the technology is mostly disregarded. We think it's inevitable to understand how the interface should be designed or which concerns/expectations/beliefs users hold if we really aim for a real-world integration of the technology. 

**b) Ethics and legal** — Addressing privacy, informed consent, data protection, responsible use, and the evolving regulatory landscape.

*Example:* Developing interfaces that can potentially extrapolate pre-cognitive states raises a whole set of ethical concerns because an individual, by definition, can't be in control of that information. Just to name one example. We as researchers should be involved in developing ethical guidelines that serve as guardrails for the community and that can ultimately inform policy makers. 

### 2.2 Interconnectedness 

Of course, our categorization is a simplification, as any model is. The boundaries between clusters are overlapping, and most work touches more than one at a time. *Within a pillar* the overlaps are especially prevalent — signal processing and universality, for example, are hard to disentangle, since a classifier is only ever as general as its ability to handle noise and the variability from one session to the next. But overlaps exist *between pillars* too: how much universality we actually need depends on the use case we have in mind, and the moment we can decode something about a person, we are faced with questions of ethics and privacy. And all of it rests on the *foundation* — we can only trust a claim about a mental state as far as we trust its ground truth, and we will only build trustworthy classifiers if we agree on standards and verify them across shared data bases.

*We plan to add a figure that represents the interconnections more clearly.* 

### 2.3 Call for a Change of Perspective

Taken together, the clusters and their entanglement lead us to one conclusion: a shift in perspective is warranted — away from viewing the work narrowly, and toward recognizing that whatever specific challenge we tackle, we are ultimately working on an *interface*. Improving an interface means embracing a more holistic picture of it, one that includes the user, the system, and the loop between them.

Concretely, we see this as a shift from passive BCI as a **decoding problem** — reading a state out of the brain — to **Neuroadaptive Technology (NAT)**, where we use BCIs as technology to adapt a machine to the user's state. It changes the question we ask from "how accurately can we classify this state?" to "how should the system respond, and how do human and machine co-adapt over time?" Therefore, we want to invite researchers to frame their work with respect to the whole interface rather than the signal alone.

---

## 3. Workshop: Challenge Synthesis

> _[Placeholder — content will be synthesized and updated after the workshop.]_


---

## 4. Next Steps

After the workshop we plan to pursue the following steps:

1. **Synthesize the workshop.** The results of the workshop will be synthesized and uploaded here.
2. **Merge internal and expert insights.** We will combine the insights we developed internally (see [Section 2](#2-mapping-core-challenges)) with the expert perspectives gained at the workshop, to pinpoint blind spots, shifts in emphasis, and overlaps.
3. **Work toward a published guideline.** Ultimately, we aim to develop a published guideline for the field — one that specifically targets the question of how meaningful integration of passive BCIs into real-world contexts can be realized within the next ten years.

---

## 5. How to Work With This Repository

There are three main ways to engage with this repository:

- **Share it.** Pass it on to researchers and colleagues who work on — or are curious about — passive BCI and neuroadaptive technology.
- **Give feedback.** Share your thoughts, comments, and corrections — including anything you think is missing or wrong. The easiest way is to open an issue.
- **Become a contributor.** If you'd like to get more closely involved in the project, get in touch — we welcome new collaborators.

---
