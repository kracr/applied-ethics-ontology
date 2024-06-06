# applied-ethics-ontology
## Overview

This repository holds the [Applied Ethics (ApplE)](https://purl.org/appliedethicsontology/documentation) ontology, which captures ethical information using two modules: an [applied ethics module](#appliedethics) and an [event context module](#eventcontext). To enhance the reusability of this resource, this README file contains information about the [methodology](#method) used to develop the ontology, along with a [tutorial](#tut) to demonstrate its various applications. The associated [queries](https://github.com/kracr/applied-ethics-ontology/blob/main/tests/CQs%20and%20Queries.xlsx), [SWRL rules](https://github.com/kracr/applied-ethics-ontology/blob/main/tests/SWRL%20rules%20sheet.xlsx), [visual representations](https://github.com/kracr/applied-ethics-ontology/tree/main/images), and [documentation](https://github.com/kracr/applied-ethics-ontology/blob/main/Paper%20Submission.pdf) are also enclosed within this repository.  

Further information regarding the ApplE ontology may be accessed at the following:
- [ApplE Ontology](https://purl.org/appliedethicsontology)
- [Documentation](https://purl.org/appliedethicsontology/documentation)
- [Apache License 2.0](https://www.apache.org/licenses/LICENSE-2.0)

Table of Contents:
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

   6.3. [How to - Dataset Development](#c)

   6.3. [How to - Metaethics Research](#d)

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

   - Applied Ethics: A discipline concerned with the application of ethics in realworld events.

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

This repository consists of the ApplE ontology and related artefacts.

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

The ontology is available for anyone to access via this repository and the PURL locator. We have suggested the ApplE ontology to the [Linked Open Vocabulary](https://lov.linkeddata.es/dataset/lov/) as a resource since the platform does not contain any ontology or ODP that is dedicated to Applied Ethics, Ethics, or Ethics Theory. 

Once accessed/downloaded, a user may import the ontology to their own and use the entities (classes, data properties, instances, etc.) they would like for their own ontology. This is usually recommended when a user may like to expand on our ontology for a specific use case, or use many entities.

Alternatively, a use may use the IRI of the entity they choose and directly import it via that identifier. This is recommended when the number of desired entities from the ApplE ontology are few.

Reusing entities from established ontologies is considered a good practice in the ontology development and modeling community as it aids the interconnectedness of information.

<a name="b"></a>
###  6.2. How to - Domain-Specific Use Case

One may apply the ontology to a specific use case, and use the given entities and properties to infer semantically appropriate information from the scenario. A user may plug in the user-required values in the form of instances for as many classes as they can (provided that the information regarding the scenario is known to them), and let the ontology do the rest.

The instances will then add to a knowledge graph that would represent the domain-specific use case via the ApplE ontology.

For example, given the following real-world motivation scenario:

_This case refers to the mass addiction to opioid-based painkillers in the US in the early 2000s. Bioethics features an applied ethics philosophy called Principlism, which favors the principles of justice, nonmaleficence, beneficence, and autonomy. Consider this. A doctor, with good intentions, prescribed to a teenage patient thirty tablets of Oxycontin, a powerful painkiller containing oxycodone, a powerful opioid, for post-dental surgery pain. They were not fully aware of its addictive nature when taken over prolonged periods of time, and yet prescribed a large dose of the drug against policy so the patient would not have to come to the clinic multiple times. However, the continuous intake of the drug led to Opioid Use Disorder (OUD) [45] in the patient. Given that the good, short-term consequence was mild (relieving pain), but the bad, long-term consequence was significant (addiction to drugs), the doctor was at fault regardless of his good intentions. The doctor violated the principles of responsibility and nonmaleficence while upholding the principle of beneficence. They were responsible for fully knowing the drug before prescribing it and following their duties without breaching any policy._

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
###  6.3 How to - Dataset Development

The ApplE ontology may be used to drive the development of Knowledge Graphs and Datasets. The taxonomy this ontology is built upon was created in collaboration with a domain expert, in our case, an Applied Ethicist, 

<a name="d"></a>
###  6.4. How to - Metaethics Research
