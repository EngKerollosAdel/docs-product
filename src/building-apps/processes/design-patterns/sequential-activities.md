---
locale: en-us
guid: 8545c13f-4722-4075-954a-8790ebc8e683
app_type: traditional web apps, mobile apps, reactive web apps
platform-version: o11
figma: https://www.figma.com/file/iBD5yo23NiW53L1zdPqGGM/Developing%20an%20Application?node-id=269:1
summary: Learn how to design sequential activities in OutSystems 11 (O11) by connecting them in the flow path according to their execution order.
tags: workflow design, process modeling, flowchart, user guide
audience:
  - mobile developers
  - frontend developers
  - full stack developers
outsystems-tools:
  - service studio
coverage-type:
  - understand
topic:
  - process-decision-patterns
---

# Designing Sequential Activities

To design activities which are to be executed in sequence, simply place those activities in the flow path connected by their execution order.

When the process is executed, activities are executed, one by one, following the sequence in the flow; the process execution only advances to the next activity when the current one is finished.


## Example

As an example, think of a recruitment process for candidates who apply for a job: screen the candidate, validate the Curriculum Vitae, interview the candidate, and approve (or not) based on the gathered feedback.

![Flowchart illustrating the sequence of activities in a recruitment process including screening, CV validation, interviewing, and approval.](images/sequential-activities.png "Sequential Activities Flowchart")
