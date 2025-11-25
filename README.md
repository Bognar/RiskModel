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

The Exposure Factor (EF) serves as a crucial third dimension, refining the Base Risk Score. The EF is the measure of the percentage of an asset's value lost if a threat is realized. 
In this model, it is used as a multiplier to determine the Final Risk Score.
This factor prevents you from treating two risks with the same Base Risk Score (e.g., a Medium/Medium score of 4 and a Low/High score of 3) identically, 
if one of them involves a Critical asset.

| Exposure Factor | Multiplier Value | Description |
| :--- | :---: | ---: | ---: |
| Trivial	| ×1.0	| The asset is easily replaced or has minimal monetary/operational value. |			
| Moderate	| ×1.5	| The asset is valuable but loss/damage is not business-ending. |
| Critical	| ×2.0	| The asset is irreplaceable (e.g., brand reputation) or its loss/damage is existential to the business. |			
						
						
Final Risk Score = Base Risk Score x EF Multiplier						
						
						
Risk Scenario	P × I	Base Risk Score	EF	EF Multiplier	Final Risk Score	Final Risk Level
A (High P, Low I, Trivial EF)	  3×1	  3	Trivial	  1	  3	Medium
B (Low P, High I, Critical EF)	1×3	  3	Critical	2	  6	High
