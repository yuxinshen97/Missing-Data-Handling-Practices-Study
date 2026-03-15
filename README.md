# Missing Data Handling Practices Study  
## Literature Screening and Extraction Validation

This repository documents my approach to the “LLM-Assisted Literature Screening Validation” task for the Missing Data Handling Practices Study.

I approached this task not as a one-off extraction exercise, but as a protocol design problem. The goal was not only to classify papers and record variables, but to develop a screening and extraction framework that can remain consistent, transparent, and scalable as the sample grows.

---

## Project Objective

This task has three linked objectives.

First, it requires a clear screening framework for determining which papers should enter detailed extraction, especially among empirical quantitative studies.

Second, it requires a structured extraction protocol for recording research design, focal variables, model type, and missing-data handling practices in a way that is consistent across papers.

Third, it requires an evaluation of the coding protocol itself. In practice, some papers fit the framework cleanly, while others create ambiguity around classification, construct definition, or extractability. A useful workflow therefore has to do more than produce outputs. It also needs to make uncertainty visible and document where the protocol may need refinement before full-scale implementation.

---

## General Approach

I organized the task into three parts.

### Part A. Screening Framework
I began by defining a classification framework that serves a practical purpose: deciding whether a paper should enter the extraction universe.

Rather than treating classification as a purely descriptive labeling exercise, I treated it as a decision rule for downstream coding. The central question was not simply what kind of paper this is, but whether the paper contains a sufficiently clear empirical structure to support consistent extraction.

In making this decision, I focused primarily on:
- whether the paper is empirical
- whether the empirical analysis is quantitative
- whether the paper contains a clearly identifiable focal relationship
- whether the design supports structured coding of key variables and model information

When front-end framing and methods sections pointed in different directions, I prioritized the methods, data, and empirical strategy sections. In this setting, extractability depends more on how the study is actually executed than on how it is introduced.

### Part B. Variable Extraction
For papers that met the screening criteria, I extracted structured information on:
- paper identification and study design
- research question
- dependent and independent variables
- mediators, moderators, and controls where relevant
- sample characteristics
- model type
- missing-data handling practices
- data and code availability
- replication feasibility

A key principle in this stage was to separate theoretical constructs from reported variable labels. In many papers, the construct of interest and the exact operational measure are not identical. Treating them as interchangeable can create coding error and reduce comparability across studies.

I also treated missing-data handling as an evidence problem rather than a binary field. In many papers, the handling of missingness is not stated directly. For that reason, I distinguished between:
- explicitly reported handling
- implicitly indicated handling
- not reported

This distinction is important because many papers appear to rely on complete-case or sample-restricted analysis without naming the procedure directly.

### Part C. Protocol Evaluation
I treated the extraction exercise as a way to test the coding framework itself.

In addition to recording paper-level information, I tracked where ambiguity arose, which variables were hardest to code consistently, and which parts of the protocol may need refinement before scaling to a larger sample.

This matters because a workflow can appear functional on straightforward papers while still failing on mixed-design, multi-study, or weakly reported cases. A useful protocol should therefore identify not only outputs, but also the boundaries of reliable coding.

---

## Classification Logic

I designed the screening framework around extractability.

The purpose of classification was to determine whether a paper should enter detailed coding and, if so, under what conditions. In practice, I found it useful to distinguish among the following broad categories:

1. **Empirical quantitative papers with a clearly codable design**  
   These papers are the strongest candidates for full extraction. They typically contain a clear empirical strategy, identifiable focal variables, and regression-based or closely related statistical analysis.

2. **Empirical quantitative papers that are harder to map onto the extraction template**  
   These papers are still empirical, but the relationship structure may be diffuse, highly descriptive, simulation-heavy, or otherwise difficult to translate into a standard IV/DV coding framework.

3. **Mixed-design or multi-study papers**  
   These papers may combine conceptual development, experiments, surveys, or archival analyses. In these cases, paper-level classification is often too coarse, and study-level coding becomes more appropriate.

4. **Conceptual, theoretical, review, or qualitative papers**  
   These do not enter detailed extraction under the current protocol.

5. **Borderline or low-information cases**  
   These are papers for which eligibility is plausible, but extractability is limited because key design features are unclear, incomplete, or too weakly reported.

---

## Decision Rules for Ambiguous Cases

Ambiguous cases were handled using a small set of decision rules.

**Methods over framing.**  
If the abstract or introduction emphasized broad theoretical contribution, but the methods and results sections contained a clear empirical design, I classified the paper based on the empirical sections.

**Evidence over labels.**  
I did not rely solely on the authors’ own labels, such as “theory paper” or “multi-method study.” The relevant question was whether the paper’s main claims depended on quantitative empirical evidence.

**Study-level coding when needed.**  
For papers with multiple studies, I treated the study, rather than the paper, as the relevant coding unit when the empirical components differed in design or extractability.

**Extractability as a separate concern.**  
A paper could be empirically relevant but still difficult to code reliably. In those cases, I treated eligibility and extractability as related but distinct judgments.

---

## Confidence and Uncertainty

I treated confidence as a necessary part of the coding process.

In this task, uncertainty does not only arise from weak reading. It also arises from incomplete reporting, diffuse construct definitions, and mismatches between paper design and extraction template. For that reason, I kept confidence separate from final coding decisions.

At a minimum, confidence reflects two different issues:
- how certain I am that the paper belongs in a given category
- how certain I am that the extracted fields accurately reflect the paper

This distinction is useful because some papers are easy to classify but difficult to code in detail, while others are harder to classify at first glance but become straightforward once the empirical design is located.

---

## Missing Data Handling

A central focus of this task is how papers handle missing data, and this is also one of the most weakly reported parts of many empirical papers.

In practice, missing-data handling often appears in indirect form:
- sample reductions between stages
- references to complete observations only
- unexplained differences in N across models
- variable-level omissions implied by construction rules

As a result, I treated missing-data coding as a structured reading task rather than a simple yes/no field. Whenever possible, I distinguished between directly reported handling and handling inferred from the paper’s empirical setup.

---

## Deliverables

The repository is organized to support three outputs:

1. a screening framework for classifying papers and handling borderline cases  
2. a structured extraction workflow for empirical papers  
3. a summary assessment of recurring patterns, reporting gaps, and protocol refinement needs

The final deliverables are intended to show both coding results and coding logic.

---

## Main Takeaway

The main purpose of this task was not just to process papers. It was to build a workflow that makes decisions explicit, keeps coding traceable, and surfaces uncertainty early.

For that reason, I treated literature screening and variable extraction as parts of a larger protocol-validation exercise. The end product is not simply a completed spreadsheet, but a framework that can support more reliable large-scale coding in future stages of the project.
