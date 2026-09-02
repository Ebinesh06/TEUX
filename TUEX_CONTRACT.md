\# TUEX Development Contract



\## 1. Project Definition



TUEX is an AI-powered verification layer that converts

unstructured human input into structured, verified data

that existing software can consume.



Education is our first demonstration workflow.

The core engine must not be hard-coded only for education.



\---



\## 2. Core Pipeline



Input

→ AI Understanding

→ Structured Data

→ Normalization

→ Entity Matching

→ Deterministic Validation

→ Cross-Source Comparison

→ Conflict Detection

→ Human Verification

→ Verified Record

→ Database

→ API / CSV / PDF



\---



\## 3. Core Principle



AI assists the decision.



The human owns the decision.



AI must NEVER silently commit conflicting information.



When a meaningful conflict exists:



1\. TUEX identifies the conflicting values.

2\. TUEX identifies the sources.

3\. TUEX explains the conflict.

4\. TUEX asks an authorized human to verify.

5\. The human decision becomes the verified result.

6\. The verification event is stored in the audit trail.



\---



\## 4. Supported Input Types



The MVP supports:



\- Text

\- Images

\- Audio / voice

\- Documents where practical



AI is responsible for understanding unstructured input.



Application code is responsible for deterministic

validation, comparison, state transitions and persistence.



\---



\## 5. Shared Data Contract



Every processing workflow should produce data compatible

with this structure:



```json

{

&#x20; "workflow": "attendance",

&#x20; "status": "ready",

&#x20; "records": \[],

&#x20; "conflicts": \[],

&#x20; "needs\_human\_review": false

}

