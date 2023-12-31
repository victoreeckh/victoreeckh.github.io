- ![Thesis Proposal Master Energ1.pdf](../assets/Thesis_Proposal_Master_Energ1_1697311749137_0.pdf)
  collapsed:: true
	- HC
		- ((652aed17-dc7c-4e46-8588-989057354eb0))
		-
	- Research question
		- ((652aec1d-60a4-4a24-8642-780c7c6971bc))
- Some intial documents
	- ![Spatial-Temporal_Deep_Learning_for_Hosting_Capacity_Analysis_in_Distribution_Grids.pdf](../assets/Spatial-Temporal_Deep_Learning_for_Hosting_Capacity_Analysis_in_Distribution_Grids_1697311871893_0.pdf)
		- Spatial-Temporal_Deep_Learning_for_Hosting_Capacity_Analysis_in_Distribution_Grids.pdf
			- Summary
			  collapsed:: true
				- ((652aecbf-6ede-4658-af6d-0ff2a7ad49de))
				- HC
					- ((652aed3d-d633-43d4-aefa-9a75f7927c9d))
				- Different HCA techniques
					- ((654772cd-b79b-42f2-ac92-6b2fb27441ed))
					- ((652aed92-4f05-4784-9497-442c8199d9d1))
					- time-series, ICA
						- ((652aedef-c0bd-4977-80ec-08e476f7bf29))
						- ((652aee7e-79a8-4337-91ef-f36b53a0d7ce))
					- Machine Learning
						- ((652af1d0-f03e-41d9-9d51-6149734905ac))
						- ((652af369-9b4d-4816-9bdb-17551c159ec8))
				- LSTM illustration
					- time-series -> RNN
						- ((652c3e7d-5187-4a56-9bb1-b1d668145f42))
				- Test cases
					- IEEE 123-bus feeder
					- Arizona utility high penetration feeder
			- Questions
			  collapsed:: true
				- Input training data are vectors of voltage magnitudes and angles (load and PV profiles) etc. that are obtained through powerflow analysis, so the structure of the network still has to be known to generate the training set?
					- -> Not modelfree?
					- No topology identification?
				- Why does longest path method work best?
	- ![Electrical_Model-Free_Voltage_Calculations_Using_Neural_Networks_and_Smart_Meter_Data.pdf](../assets/Electrical_Model-Free_Voltage_Calculations_Using_Neural_Networks_and_Smart_Meter_Data_1697314312902_0.pdf)
		- Electrical_Model-Free_Voltage_Calculations_Using_Neural_Networks_and_Smart_Meter_Data.pdf
			- Summary
			  collapsed:: true
				- ((653a6c83-5a32-41e7-8ea6-6e90002cf79b))
				- ((653a6c6b-f406-4d21-a5fb-f506c4e177e6))
				- ((653a7232-7fa7-4c86-b643-33f13a3fa5f6))
				- NN selection
					- ((653a7e5d-4ca5-40ef-8785-63230845e21c))
	- ![Data-Driven_Study_of_Low_Voltage_Distribution_Grid_Behaviour_With_Increasing_Electric_Vehicle_Penetration.pdf](../assets/Data-Driven_Study_of_Low_Voltage_Distribution_Grid_Behaviour_With_Increasing_Electric_Vehicle_Penetration_1699179106790_0.pdf)
		- Data-Driven_Study_of_Low_Voltage_Distribution_Grid_Behaviour_With_Increasing_Electric_Vehicle_Penetration.pdf
			- Summary
			  collapsed:: true
				- Abstract
					- ((65476c5a-b106-411c-b1d0-9e599df40547))
					- ((65476c83-050e-416e-95db-465170c979d0))
					- ((65476ca3-8052-4d30-9c51-81f3312031ea))
				- Literature review
					- ((65476f36-f22d-4420-a11f-6172351756fd))
					- How does Monte Carlo simulation of EV impact work?
						- ((654771e1-c07d-44ea-95f2-023329eaf043))
				- Focus
					- ((654773d9-55ed-4002-ab07-cba2b0d0fa43))
				- Methodology
					- Grid data
						- ((6548fb1d-0894-4652-bcc0-6e014261507b))
					- Load
						- Interesting Python package
							- ((6548fc64-05eb-4b25-b2a9-7b40db3b8102))
					- EV penetration
					- ((65490de6-1bcf-4e21-9ff5-fcaaa7080c7c))
						- Interesting PF simulation package in python
				- Conclusion
					- ((6549117a-9e20-4b09-894c-422e777209bd))
					- Read!
				-
			- Questions
			  collapsed:: true
				- How to measure EV impact on network?
	- Ongoing project: Model-Free DER Hosting Capacity and Operating Envelopes
		- slides
			- ![UoM-C4NET-Model-FreeDERHCandOEsProjectUpdate-Final.pdf](../assets/UoM-C4NET-Model-FreeDERHCandOEsProjectUpdate-Final_1699287628166_0.pdf)
		- Paper
			- ![2023CIGRECairns-Michael-Vincenzo-Nando-Tansu-Chris-Peter-Kenneth-John-FromModel-DriventoModel-Free-RG.pdf](../assets/2023CIGRECairns-Michael-Vincenzo-Nando-Tansu-Chris-Peter-Kenneth-John-FromModel-DriventoModel-Free-RG_1699287855974_0.pdf)
		- https://electrical.eng.unimelb.edu.au/power-energy/projects/model-free-operating-envelopes
			-
- Questions
	- Intro chapters
		- Penetration of EV-PV (DER) -> effect on LV network constraints?
		  collapsed:: true
			- Distinction between different LV grids
				- Geography, function
			- Different penetration levels
		- -> It is vital to know HC -> different ways to calculate HCA
		  collapsed:: true
			- Traditional
				- Deterministic
				  collapsed:: true
					- Traditional HCA methods
					  collapsed:: true
						- ((654772cd-b79b-42f2-ac92-6b2fb27441ed))
					- The deterministic method obtains an optimal solution on a single scenario, usually the worst-case scenario(s)
				- Stochastic
				  collapsed:: true
					- probabilistic techniques, e.g., Monte Carlo simulation, model the uncertainties in the power system
				- ICA
				  collapsed:: true
					- Differently, using historical time-series data, the streamlined method [22] and the iterative ICA [23], [24] method provide insight into how hosting capacity changes over time and the ability to derive a corresponding hosting capacity pattern subjected to time
			- Machine learning based solution
	- Only evaluation?
		- Evaluate traditional vs ML
		- Evaluate different ML algos
		- Evaluate in which dimensions?
		  collapsed:: true
			- Accuracy (computed vs actual HC)
			- Amount of network/bus violations (overvoltages etc.)
			- Computational burden
		- Evaluate different approaches
		  collapsed:: true
			- e.g. different Deep learning algorithms
				- Which hyperparameters are most important?
				- Algorithm selection
		- Evaluate feasibility
		  collapsed:: true
			- smart meter data collection
			- Real time application to NN
			- Computing time, expenses etc>
	- Implementation of an algorithm evaluator (doing it myself)?
	  collapsed:: true
		- For what part will I have to dig into code? (github etc.)
		- How is it/can it be integrated in Smart meters?
- Next readings
	- S. Balduin, T. Westermann, and E. Puiutta, “Evaluating different machine learning techniques as surrogate for low voltage grids,” Energy Inform., vol. 3, p. 24, Oct. 2020.
	-