## My Analytical Framework

I built this task around a simple principle: the classification framework should not merely label papers, but determine how each paper enters the downstream extraction workflow.

To do that, I use a three-layer structure:

### Layer 1: Study Type Classification
Each paper is first classified by research design:
- empirical quantitative, regression-based
- empirical quantitative, non-regression-based
- experimental/simulation-based quantitative
- qualitative or mixed-methods
- conceptual/review/theory

### Layer 2: Extraction Eligibility
The classification then feeds directly into the extraction decision:
- full extraction
- partial note only
- exclude from B1 extraction

This step is important because the task’s variable list is designed specifically for regression-based empirical studies, so not all quantitative papers should be treated as equally extractable.

### Layer 3: Confidence and Flagging
For every paper, I record:
- a confidence rating (high / medium / low)
- and, where needed, a flag indicating the main source of ambiguity

This makes the workflow both scalable and auditable, especially for borderline cases such as multi-study papers, unclear variable roles, and indirect reporting of missing data practices.
