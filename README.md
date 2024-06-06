# applied-ethics-ontology
## Overview

This repository holds the Applied Ethics (ApplE) ontology, which captures ethical information using two modules: an ethics theory module and an event context module. To enhance the reusability of this resource, this README file contains information about the methodology used to develop the ontology, along with a tutorial to demonstrate its various applications. The associated queries, SWRL rules, visual representations, and documentation are also enclosed within this repository.  

Further information regarding the ApplE ontology may be accessed at the following PURLs:
- [ApplE Ontology](https://purl.org/appliedethicsontology)
- [Documentation](https://purl.org/appliedethicsontology/documentation)
- [Apache License 2.0](https://www.apache.org/licenses/LICENSE-2.0)

Table of Contents:
1. [Introduction](#intro)
2. [Methodology](#method)
3. [ApplE Ontology](#onto)

   3.1. [Applied Ethics Module](#appliedethics)

   3.2. [Ethics Theory Module](#ethicstheory)
4. [Resource Specifications](#resourcespec)
5. [Repository Details](#repo)
6. [Tutorial](#tut)
   
   6.1. [How to - Reuse Desirable Entities](#a)

   6.2. [How to - Extrapolate to Domain-Specific Use Case](#b)

   6.3. [How to - Dataset Development](#c)

   6.3. [How to - Metaethics Research](#d)

<a name="intro"></a>
## 1. Introduction

Applied ethics is ubiquitous in most domains and requires much deliberation due to its philosophical nature. This leads to conflicting courses of action where ethical dilemmas become challenging to resolve. The major driving forces in such a decision can be discretized and simplified to provide an indicative answer regarding the morality of an action. 

Knowledge representation and reasoning (KRR) offer an efficient way to explicitly translate abstract ethical concepts into applicable principles within the context of an event. To achieve this, we propose ApplE, an Applied Ethics ontology that captures ethical theory and event context to holistically describe the morality of an action. The development process adheres to a modified version of the Simplified Agile Methodology for Ontology Development (SAMOD) and utilizes standard design and publication practices. 

Using ApplE, we model a use case from the bioethics domain that demonstrates our ontology’s social and scientific value. Apart from the ontological reasoning and quality checks, ApplE is also evaluated using the three-fold testing process of SAMOD. ApplE follows FAIR principles and aims to be a viable resource for applied ethicists and ontology engineers.

![alt text](https://github.com/kracr/applied-ethics-ontology/blob/main/images/upper%20level%20ontology.png?raw=true)

<a name="method"></a>
## 2. Methodology

The ApplE ontology was developed in accordance with the Simplified Agile Methodology for Ontology Development (SAMOD) and the Spiral Software Development Methodology. This customized methodology borrows from agile development and supports quick, iterative cycles of development catered towards ontologies with fewer axioms. SAMOD describes the involvement of a domain expert (DE), in our case, an applied ethicist, who outlined the classes to be considered for the ontology in a taxonomy. The ontology engineers (OEs) implemented these entities. Although SAMOD recommends the involvement of the DE to be limited to the initial development phase, we deviated from this by involving the DE twice: once at the beginning to develop the initial modelet and then to model a domain-specific use case.

![alt text](https://github.com/kracr/applied-ethics-ontology/blob/main/images/methodology.jpg?raw=true)

Steps to building ApplE:
1. Developing the domain taxonomy with the involvement of the DE. In the second pass, we developed the use cases.
2. Formalizing the domain in a modelet.
3. Merge the modelet to any previous milestone.
4. Refactor the new ontology to ensure semantic integrity.

During the initial phase, informal competency questions were created to gauge the quality of the ontology. A glossary of terms was also built in order to discretize the abstract philosophical terms that ApplE call for. The testing phase involves three-fold testing as the model, data, and query level. More on this has been discussed in our paper. Please see the 'tests' folder for some related artefacts such as competency questions and SWRL rules.

Brief Glossary of Terms:

- Applied Ethics Module
   Ethics: A discipline concerned with studying what is morally right, wrong, good, or bad.

   Applied Ethics: A discipline concerned with the application of ethics in realworld events.

   Applied Ethics Philosophy: A theory or ideology that stems from normative ethics and is applied to real-world events.

   Ethical Principle: A concept that defends the morality of an action at an intrinsic level.

   Ethical Issue: A situation where an ethical conflict may arise.
- Event Context Module

   Context: The circumstances in which an event occurs.

   Event: Something that happens.

   Agent: An entity capable of doing and receiving actions (eg: Person, Company, Animal, Government, etc.).

   Action: Something that is done.

   Consequence: The outcome of an action.

   Moral Intention: The intention of an agent with regard to a moral action.

<a name="onto"></a>
## 3. ApplE Ontology

<a name="appliedethics"></a>
### 3.1 Applied Ethics Module

<a name="ethicstheory"></a>
### 3.2 Ethics Theory Module

<a name="resourcespec"></a>
## 4. Resource Specifications

- FAIR Compliance and Persistent Availability: The ApplE ontology is FAIR compliant and available on GitHub and is easily findable via a permanent locator. It falls under the Apache 2.0 license. 
- Ontology Validation: The ontology has been validated using SAMOD's three-fold evaluation process and has been checked for inconsistencies and pitfalls using the OOPs Pitfall Scanner and the HermiT reasoner.
- Documentation: The documentation for the ontology is available for public access via a PURL locator and uses the standard Live OWL Documentation Environment (LODE) documentation format for ease of readability.
- Resource Maintenance: The ontology is to be maintained on this GitHub repository and will be available for public use.

<a name="repo"></a>
## 5. Repository Details

<a name="tut"></a>
## 6. Tutorial
This tutorial describes methods of application where the ApplE ontology may be used as a resource for applied ethics information. 
<a name="a"></a>
###  6.1. How to - Reuse Desirable Entities

<a name="b"></a>
###  6.2. How to - Domain-Specific Use Case

<a name="c"></a>
###  6.3 How to - Dataset Development

<a name="d"></a>
###  6.4. How to - Metaethics Research
