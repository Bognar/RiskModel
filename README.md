Colateral Risk Model

This model combines the two standard components of risk, Impact and Probability, into a 2D Risk Heatmap, and then integrates the third component, Exposure Factor (EF), 
as a Risk Multiplier to determine the final, comprehensive risk level.The standard unit for the heatmap is the Base Risk Score, calculated as: 

Base Risk Score = Probability Score x Impact Score

| Category | Score Range | Description |
| ---: | ---: | ---: |
| Low Risk | From 1 to 2 | Acceptable risk; addressed through standard procedures.	|
| Medium Risk | From 3 to 5	| Requires specific mitigation plan; leadership review needed.	|
| High Risk	| From 6 to 9	| Requires immediate action and executive approval for acceptance.	|
			

| Probability ↓ / Impact → | Low (1) | Medium (2) | High (3) |
| :--- | :---: | ---: | ---: |
| High (3) | 3 (Medium) | 6 (High) | 9 (High) |
| Medium (2) | 2 (Low) | 4 (Medium) | 6 (High) |
| Low (1) | 1 (Low) | 2 (Low) | 3 (Medium) |

The Exposure Factor (EF) serves as a crucial third dimension, refining the Base Risk Score. The EF is the measure of the percentage of a control's value lost if a threat is realized. 
In this model, it is used as a multiplier to determine the Final Risk Score.
This factor prevents you from treating two risks with the same Base Risk Score (e.g., a Medium/Medium score of 4 and a Low/High score of 3) identically, 
if one of them involves a Critical control.
Practical example: Two users that do not have MFA enambed, one is employee and another one is CFO. We can't allow them to have same risk level considering the colateral impact.

| Exposure Factor | Multiplier Value | Description |
| :--- | :---: | ---: |
| Trivial	| ×1.0	| The control is easily replaced or has minimal monetary/operational value. |			
| Moderate	| ×1.5	| The control is valuable but loss/damage is not business-ending. |
| Critical	| ×2.0	| The control is irreplaceable (e.g., brand reputation) or its loss/damage is existential to the business. |			
						
						
Final Risk Score = Base Risk Score x EF Multiplier						
						
						
| Risk Scenario	| P × I	| Base Risk Score	EF	| EF Multiplier | Final Risk Score EF | Final Risk Level |
| ---: | ---: | ---: | ---: | ---: | ---: |
| A (High P, Low I, Trivial EF) | 3×1 | 3 | Trivial | 1 | 3	| Medium |
| B (Low P, High I, Critical EF) | 1×3 | 3 | Critical | 2 | 6 | High |


| Category | Score Range | Description |
| ---: | ---: | ---: |
| Low Risk | From 1 to 4 | Acceptable risk; addressed through standard procedures.	|
| Medium Risk | From 5 to 9	| Requires specific mitigation plan |
| High Risk	| From 10 to 14	| Requires immediate action, leadership review needed.	|
| Critical Risk	| From 15 to 18	| Requires immediate action and executive approval for acceptance.	|
