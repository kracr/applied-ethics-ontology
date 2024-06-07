# applied-ethics-ontology
## Overview

This repository holds the [Applied Ethics (ApplE)](https://purl.org/appliedethicsontology/documentation) ontology, which captures ethical information using two modules: an [applied ethics module](#appliedethics) and an [event context module](#eventcontext). To enhance the reusability of this resource, this README file contains information about the [methodology](#method) used to develop the ontology, along with a [tutorial](#tut) to demonstrate its various applications. The associated [queries](https://github.com/kracr/applied-ethics-ontology/blob/main/tests/CQs%20and%20Queries.xlsx), [SWRL rules](https://github.com/kracr/applied-ethics-ontology/blob/main/tests/SWRL%20rules%20sheet.xlsx), [visual representations](https://github.com/kracr/applied-ethics-ontology/tree/main/images), and [documentation](https://github.com/kracr/applied-ethics-ontology/blob/main/Paper%20Submission.pdf) are also enclosed within this repository.  

Further information regarding the ApplE ontology may be accessed at the following:
- [ApplE Ontology](https://purl.org/appliedethicsontology)
- [Documentation](https://purl.org/appliedethicsontology/documentation)
- [Apache License 2.0](https://www.apache.org/licenses/LICENSE-2.0)

# Table of Contents:
1. [Introduction](#intro)
2. [Methodology](#method)
3. [ApplE Ontology](#onto)

   3.1. [Applied Ethics Module](#appliedethics)

   3.2. [Event Context Module](#eventcontext)
   
4. [Resource Specifications](#resourcespec)
5. [Repository Details](#repo)

   5.1. [ApplE Ontology](#5onto)
   
   5.2. [ApplE Website](#5web)

   5.3. [Miscellaneous](#5other)
   
6. [Tutorial](#tut)
   
   6.1. [How to - Reuse Desirable Entities](#a)

   6.2. [How to - Extrapolate to Domain-Specific Use Case](#b)

   6.3. [How to - Dataset Development (New)](#c)

7. [Metaethics Research (for philosophy nerds)](#meta)
8. [Resource Maintenance](#maintenance)

<a name="intro"></a>
## 1. Introduction

Applied ethics is ubiquitous in most domains and requires much deliberation due to its philosophical nature. This leads to conflicting courses of action where ethical dilemmas become challenging to resolve. The major driving forces in such a decision can be discretized and simplified to provide an indicative answer regarding the morality of an action. 

Knowledge representation and reasoning (KRR) offer an efficient way to explicitly translate abstract ethical concepts into applicable principles within the context of an event. To achieve this, we propose [ApplE](http://150.146.207.114/lode/extract?url=https%3A%2F%2Fraw.githubusercontent.com%2Fkracr%2Fapplied-ethics-ontology%2Fmain%2FApplE%2520Ontology%2Fapple.owl&lang=en), an Applied Ethics ontology that captures applied ethics theory and event context to holistically describe the morality of an action. The development process adheres to a modified version of the [Simplified Agile Methodology for Ontology Development (SAMOD)](https://essepuntato.it/samod/) and utilizes standard design and publication practices. 

Using ApplE, we model a use case from the [bioethics](https://plato.stanford.edu/entries/theory-bioethics/) domain that demonstrates our ontology’s social and scientific value. Apart from the ontological reasoning and quality checks, ApplE is also evaluated using the three-fold testing process of SAMOD. ApplE follows [FAIR principles](https://www.nature.com/articles/sdata201618) and aims to be a viable resource for applied ethicists and ontology engineers.

![alt text](https://github.com/kracr/applied-ethics-ontology/blob/main/images/upper%20level%20ontology.png?raw=true)

<a name="method"></a>
## 2. Methodology

The ApplE ontology was developed in accordance with the [SAMOD](https://essepuntato.it/samod/) and the [Spiral Software Development Methodology](https://www.sciencedirect.com/science/article/abs/pii/B9780080515748500315). This customized methodology borrows from agile development and supports quick, iterative cycles of development catered towards ontologies with fewer axioms. SAMOD describes the involvement of a domain expert (DE), in our case, an applied ethicist, who outlined the classes to be considered for the ontology in a taxonomy. The ontology engineers (OEs) implemented these entities. Although SAMOD recommends the involvement of the DE to be limited to the initial development phase, we deviated from this by involving the DE twice: once at the beginning to develop the initial modelet and then to model a domain-specific use case.

![alt text](https://github.com/kracr/applied-ethics-ontology/blob/main/images/methodology.jpg?raw=true)

Steps to building ApplE:
1. Developing the domain taxonomy with the involvement of the DE. In the second pass, we developed the use cases.
2. Formalizing the domain in a modelet.
3. Merge the modelet to any previous milestone.
4. Refactor the new ontology to ensure semantic integrity.

During the initial phase, informal competency questions were created to gauge the quality of the ontology. A glossary of terms was also built in order to discretize the abstract philosophical terms that ApplE call for. The testing phase involves three-fold testing as the model, data, and query level. More on this has been discussed in our paper. Please see the 'tests' folder for some related artifacts, such as competency questions and SWRL rules.

**Brief Glossary of Terms:**

- Applied Ethics Module
   - Ethics: A discipline concerned with studying what is morally right, wrong, good, or bad.

   - Applied Ethics: A discipline concerned with the application of ethics in real-world events.

   - Applied Ethics Philosophy: A theory or ideology that stems from normative ethics and is applied to real-world events.

   - Ethical Principle: A concept that defends the morality of an action at an intrinsic level.

   - Ethical Issue: A situation where an ethical conflict may arise.
- Event Context Module

   - Context: The circumstances in which an event occurs.

   - Event: Something that happens.

   - Agent: An entity capable of doing and receiving actions (eg: Person, Company, Animal, Government, etc.).

   - Action: Something that is done.

   - Consequence: The outcome of an action.

   - Moral Intention: The intention of an agent with regard to a moral action.

<a name="onto"></a>
## 3. ApplE Ontology

The ApplE ontology consists of two modules which each categorize the various factors required to make an ethically-informed decision. More details are provided in our [paper submission](https://github.com/kracr/applied-ethics-ontology/blob/main/Paper%20Submission.pdf).

<a name="appliedethics"></a>
### 3.1 Applied Ethics Module

![alt text](https://github.com/kracr/applied-ethics-ontology/blob/main/images/ethics%20module_updated.png?raw=true)

<a name="eventcontext"></a>
### 3.2 Event Context Module

![alt text](https://github.com/kracr/applied-ethics-ontology/blob/main/images/context%20module.png?raw=true)

<a name="resourcespec"></a>
## 4. Resource Specifications

- [FAIR Compliance](https://www.nature.com/articles/sdata201618) and Persistent Availability: The ApplE ontology is FAIR compliant and available on [GitHub](https://github.com/kracr/applied-ethics-ontology) and is easily findable via a [permanent locator](https://raw.githubusercontent.com/kracr/applied-ethics-ontology/main/ApplE%20Ontology/apple.owl). It falls under the [Apache 2.0 license](https://www.apache.org/licenses/LICENSE-2.0). 
- Ontology Validation: The ontology has been validated using SAMOD's three-fold evaluation process and has been checked for inconsistencies and pitfalls using the [OOPs Pitfall Scanner](https://oops.linkeddata.es/) and the [HermiT reasoner](http://www.hermit-reasoner.com/).
- Documentation: The documentation for the ontology is available for public access via a [PURL locator](https://purl.org/appliedethicsontology/documentation) and uses the standard [Live OWL Documentation Environment (LODE)](https://essepuntato.it/lode/) documentation format for ease of readability.
- Resource Maintenance and Sustainability Plan: The ontology is to be maintained on this GitHub repository and will be available for public use. A tutorial section has been provided below for users to effectively utilize the ApplE ontology for future works. Currently, the authors of this ontology are exploring methods to use this resource for some neurosymbolic techniques. This will allow us and other users to engage with the ApplE ontology in a constructive and useful way. 

<a name="repo"></a>
## 5. Repository Details

This repository consists of the ApplE ontology and related artifacts.

<a name="5onto"></a>
### 5.1. ApplE Ontology

The ontology is presented in the [OWL](https://www.w3.org/OWL/) format for ease of accessibility. It may be accessed via [Protege](https://protege.stanford.edu/). For reference, the authors used Protege Version 5.5.0 for running this version of ApplE on an 11th Gen i7 64-bit system with a Windows 11 Home Version 23H2. The ontology yields no pitfalls and is consistent and coherent. It passed all model tests and is semantically sound. Further tests were completed via data and query testing, which are also included in this repository.

<a name="5web"></a>
### 5.2. ApplE Website

The ApplE website was developed as a customized version using the automatically generated Live OWL Documentation Environment (LODE) software. This repository allows us to host the html file and other associated files via a permanent uniform resource locator ([PURL](https://purl.org/appliedethicsontology/documentation)) for easy access to the documentation.  

<a name="5other"></a>
### 5.3. Miscellaneous 

A folder contains the [images](https://github.com/kracr/applied-ethics-ontology/tree/main/images) that are useful for the documentation of this ontology. The images are either high-quality original visual representations of the ontology or screenshots of experiments or validations. The [tests](https://github.com/kracr/applied-ethics-ontology/tree/main/tests) folder consists of the competency questions used, the associated queries, and the badge proving the quality of ApplE from the [OOPS Pitfall Scanner](https://oops.linkeddata.es/).

![alt text](https://github.com/kracr/applied-ethics-ontology/blob/main/images/OOPS%20Pitfall%20Scanner_No%20Pitfalls%20Detected%20-%20Badge.png?raw=true)

<a href="http://oops.linkeddata.es"> 
	<img src="images/conformance/oops_free.png" 
	alt="Free of pitfalls" height="69.6" width="100" /></a>

<a name="tut"></a>
## 6. Tutorial
This tutorial describes methods of application where the ApplE ontology may be used as a resource for applied ethics information. 

<a name="a"></a>
###  6.1. How to - Reuse Desirable Entities

The ontology is available for anyone to access via this repository and the PURL locator. We will suggest the ApplE ontology to the [Linked Open Vocabulary](https://lov.linkeddata.es/dataset/lov/) as a resource since the platform does not contain any ontology or ODP that is dedicated to Applied Ethics, Ethics, or Ethics Theory. 

A user may import the ApplE ontology into their own and reuse the entities they would like. This is usually recommended when a user may like to expand on our ontology for a specific use case, or use many entities.

Alternatively, a user may use the IRI of the entity they choose and directly import it via that identifier. This is recommended when the number of desired entities from the ApplE ontology are few.

<a name="b"></a>
###  6.2. How to - Domain-Specific Use Case

One may apply the ontology to a specific use case and use the given entities and properties to infer semantically appropriate information from the scenario. A user may plug in the user-required values in the form of instances for as many classes as they can (provided that the information regarding the scenario is known to them) and let the ontology do the rest.

The instances will then add to a knowledge graph that would represent the domain-specific use case via the ApplE ontology.

For example, given the following real-world motivation scenario:

_This case refers to the mass addiction to opioid-based painkillers in the US in the early 2000s. Bioethics features an applied ethics philosophy called Principlism, which favors the principles of justice, nonmaleficence, beneficence, and autonomy. Consider this. A doctor, with good intentions, prescribed to a teenage patient thirty tablets of Oxycontin, a powerful painkiller containing oxycodone, a powerful opioid, for post-dental surgery pain. They were not fully aware of its addictive nature when taken over prolonged periods of time, and yet prescribed a large dose of the drug against policy so the patient would not have to come to the clinic multiple times. However, the continuous intake of the drug led to Opioid Use Disorder (OUD) [45] in the patient. Given that the good, short-term consequence was mild (relieving pain), but the bad, long-term consequence was significant (addiction to drugs), the doctor was at fault regardless of his good intentions. The doctor violated the principles of responsibility and nonmaleficence while upholding the principle of beneficence. They were responsible for fully knowing the drug before prescribing it and following their duties without breaching any policy._

The following competency questions may be asked via the ApplE ontology:

**CQ:** Which active agent prescribes the opioid painkiller?

**Associated DL Query:** ActiveAgent and doesAction some {PrescribeOpioidPainkiller}

**Result:** Doctor


**CQ:** What is the consequence of the action done by the Doctor?

**Associated DL Query:** Consequence and inverse hasConsequence some (Action and inverse doesAction some {Doctor})

**Result:** OpioidUseDisorder, PainRelief

In addition to this, we may model the use case using the ApplE ontology by instantiating the details from the real-world scenario. The user may use the provided SWRL rules to recognize whether the action done by the active agent in this particular scenario is leaning towards morally grey, right, or wrong. This may be viewed in the image below.

![alt text](https://github.com/kracr/applied-ethics-ontology/blob/main/images/usecasemodeling.png?raw=true)

As we can see, the information provided to the ApplE ontology triggers one of the provided SWRL rules and is able to give the answer in asociation with this bioethics use case.

<a name="c"></a>
###  6.3 How to - Dataset Development (New)

The ApplE ontology may be used to drive the development of Knowledge Graphs and Datasets. The taxonomy this ontology is built upon was created in collaboration with a domain expert, in our case, an Applied Ethicist. In our current work, we have used the ontology to develop a dataset for real-world scenarios in various domains where an ethical concern/dilemma is present. This dataset, the ApplE dataset, would be a work that expands on [Hendrycks' ETHICS dataset](https://github.com/hendrycks/ethics). 

The data is scraped from 25 subreddits which include AITA, AITAFiltered, AITJ, Am I the Angel, Tales from Retail, etc. This raw data was then preprocessed and cleaned, before being plugged into the GPT-4 LLM for summarization. The information from the ApplE ontology was provided to the LLM to recognize entities that were to be used as headers for the datasets, and what the semantic connections between these entities were. Using this information from ApplE, the LLM was able to summarize each case (Post Text from the Subreddits) and also infer the values for the headers provided.

A screengrab from the ontology-aided ApplE dataset is shown below:

![alt text](https://github.com/kracr/applied-ethics-ontology/blob/main/images/split.png?raw=true)

<a name="meta"></a>
## 7. Metaethics Research (for philosophy nerds)

This resource is an ontology type in the Semantic Web technologies context, but is also an ontology in a [philosophical sense](https://plato.stanford.edu/entries/logic-ontology/). An ontology is a study of what there is, regarding the existence of a concept; there exists, for some, or at least one. Such a philosophical concept is associated with many philosophical questions, such as Hume's is-ought problem and the question of God's existence. 

An ontology describes what there is and the characteristics of what there is, which is easy enough to do when considering simple objects or beings that are more apparent in the real world, such as household items, musical bands, political figures and [pizza](https://protege.stanford.edu/ontologies/pizza/pizza.owl). However, this philosophical discipline is more complex when applied to abstract concepts and begins with meta-questions such as 'does ethical AI exist?', 'can ethical AI exist?' 'can ethics be adequately captured by an AI system?', and 'what does it even mean to be adequately ethical?', amongst many other questions that are raised in the ontological study of developing an applied ethics taxonomy catered towards making inherently ethical AI systems.

The ApplE ontology is a resource contribution that is rooted in this philosophy, and builds on these questions lying at the intersection of ethics and technology. Various authors such as [Savulescu and Malsen](https://link.springer.com/chapter/10.1007/978-3-319-09668-1_6), [Brozek and Janik](https://d1wqtxts1xzle7.cloudfront.net/108112753/j.newideapsych.2018.12.00220231130-1-hrrtor-libre.pdf?1701376857=&response-content-disposition=inline%3B+filename%3DCan_artificial_intelligences_be_moral_ag.pdf&Expires=1717746862&Signature=gOBv03MsL4NzQjjppODQEnWY5fMr8XNL-xULlukfmFhUqhRXhnpn-R1oVkAt5eHyI0y3FRVVycaipqOzV0rUoWC2SDvB4faSvcwjNLaXfzuNNDiID14OYMIzIPE2dmRaEhQrdq1MavYwRMCEYudsSahlpufboAwHGcX8FixxE9V5aNDkk4Pfyp8lRBAAnm713lyhuJ2r4csB~4TFoJ6amejomGu5uz1zmoW4viFqsqwmmBZ1bKP9k5AuDnujCGm-ui0AnFueRnMn7UJRlUyQjfu4ymTvzSIAoA36ICgA9Tfxg95peFZIpgIADbes3W36JmpjLTlQIBbgs~t~hjF-ZA__&Key-Pair-Id=APKAJLOHF5GGSLRBV4ZA), [Pana](https://triple-c.at/index.php/tripleC/article/view/43/42), and [Liao](https://www.google.co.in/books/edition/Ethics_of_Artificial_Intelligence/2ST3DwAAQBAJ?hl=en&gbpv=1&dq=artificial+moral+intelligence&pg=PA480&printsec=frontcover) have penned their thoughts on artificial morality and the capacity for ethical decision-making in AI systems. With reference to these and more, we have formulated an Applied Ethics taxonomy that is built on the way human beings make decisions that may have associated ethical dilemmas. However, as humans are predisposed to their background and upbringing which, for the most part, dictates how they make their decisions, AI systems do not have to carry those biases and preconditioning to make decisions.

Initially, we began this research project with the intention to discretize ethical concepts, solely. However, due to this finding regarding ethical decision-making being heavily influenced by background factors (apart from contextual factors), we realized that simply working with ethical concepts would be a challenge: which school of thought should the AI system pick? To resolve this concern, we switched to the representation of Applied Ethics, where, after decades of discourse, there is some understanding and consensus about the ethical theories that are usually applied in specific domains. 

This is why the ApplE Ontology may fuel not only technological research but also metaethics research, as we can run and test neurosymbolic models built upon this resource to truly gauge (in real-time) the applicability of specific theories (for example, [principlism](https://d1wqtxts1xzle7.cloudfront.net/73154189/Physicians_and_Patients_in_Relation_Clin20211019-24187-z1m6s4-libre.pdf?1634653881=&response-content-disposition=inline%3B+filename%3DPhysicians_and_Patients_in_Relation_Clin.pdf&Expires=1717747572&Signature=TOASBoxVguD82Ls0IN7Pk709mjZ6REr03xu-v1UJCYrgYlSkZo9lwo6aBpecjlYJtFnysVo18-6xCJaoulJOs8kVSLDHyH4H7vNo6SIWqV8LS9sST7DzA87JtUoOkmNZgXGLE-1wgM0kavpzmHxhHm5PdvfHBjtED57eTDoNZUdYUvPf08Xs760BYJypeX9X~hY8P8ks1nDa2HGVUHVNcBH5qlgneBR-qqsgTfiPHrLcHkvFBoR4bw3zYGFXmbXU7XOR95ofIxJdAWnLhkHUBXFK7KKN7IdJh5pShGV9mmky00Z5PZFv0y3~9PpM-ZoNwzY8E3cbxzmgH5YrkooRYw__&Key-Pair-Id=APKAJLOHF5GGSLRBV4ZA#page=64) from our bioethics example) to some domain-specific use cases. Not only would this improve upon the technology deployed, but also our own understanding of what works best in certain situations, aided by the study of casuistry.

As a resource, the ApplE ontology has various impacts in the technical and social space, and we hope it is utilized to the fullest.

<a name="maintenance"></a>
### 8. Resource Maintenance

With regard to the maintenance of the ApplE ontology, this was a concern that was considered at the point of selecting the methodology. The SAMOD methodology is perfect for ontology developers who wish to build an ontology that is easy to maintain. From the insistence on clear naming, well-documented glossaries, and iterative, modular development, the methodology is a great way to ensure a sustainable development plan. With our customized version of SAMOD that includes the Spiral Development methodology as well, we also take into account newer developments in the field of applied ethics, the inclusion of which would result in yet another development cycle. 

- Modular Ontology Design: The ApplE ontology is designed in a modular format to allow easy maintenance. One module may be updated without affecting the other.
- Corrections and Updates: As more developments are made in this area, the ontology would be updated accordingly on this publicly available repository and on the [permanent locator](http://150.146.207.114/lode/extract?url=https%3A%2F%2Fraw.githubusercontent.com%2Fkracr%2Fapplied-ethics-ontology%2Fmain%2FApplE%2520Ontology%2Fapple.owl&lang=en) as well. 
- Adapting to new requirements: It is imperative to anticipate various domains where this resource may be applied, and ontologies may be created by the extension of ApplE. Our ontology is open to such extensions, and will be documented here and on all related sources.
- Resource Distribution: We aim to increase the reach of this resource for various interdisciplinary research, and thus would suggest ApplE at the Linked Open Vocabulary (LOV) platform, and will also circulate the ontology resource to relevant mailing lists. 
- Further Applications: Further applications for the ApplE ontology include extrapolation to domain-specific use cases, KG and dataset development, reusing entities from the ontology, neurosymbolic applications such as prediction and classification tasks in this area, case-based reasoning, question-answering systems, ethical dilemma resolution via recommender systems, and enhancing LLM performance via KG-RAG. As and when we build such applications or are made aware of other systems that are using the ApplE ontology as a resource, we will link them here on this permanent repository.
