################################ INFO ################################
This spreadsheet is used to calculate the parameters and values as
they appeared on the paper:
A 2SIR-VD Model for Optimizing Geographical COVID-19 Vaccine
Distribution in the Philippines / Almajose, White, Diego, Lazaro,
Austriaco*
* Corresponding author; contact at naustriaco@ust.edu.ph

############################# HOW TO USE #############################
PH-only modelling [RESULTS (1S)]
1. 	Enter desired vaccination rate in cell A3. 
A/N: Spreadsheet should automatically compute the model. A CALCULATE
button has been added for additional assurance in convergence.

Comparative modelling [RESULTS (2S)]
1. 	Input needed data type in cell B3, which takes values from 1 to 4.
2. 	Check table beside entry cell to determine what each value
	represents, which should integrate the model. A CALCULATE button
	has been added for additional assurance in convergence.
3. 	Enter value for m1 in cell I3. This represents the percent of
	vaccines that will be assigned to S1 in the compartmental model.
	Takes only values from 0 to 1.
4. 	Enter desired vaccination rate in cell N3. 

########################## ADDITIONAL NOTES ##########################
1. 	Excel Macro buttons have been added for ease of copying the model
	results.
2.	PH COVID-19 historical data have been stored in the spreadsheet,
	however only the first five weeks of the second surge has been used
	in modelling the data. Data taken from DOH COVID-19 tracker:
	https://doh.gov.ph/covid-19/case-tracker
3. 	Excel Solver / GRG Nonlinear has been used to optimize the models. 

############################## CONTACT ###############################
For troubleshooting, contact allan_paolo.almajose@upd.edu.ph

############################# CHANGELOG ##############################
(JUL 14 2021)
- 	Changed integration scheme to the fourth-fifth order
	Dormand-Prince-Runge-Kutta-Fehlberg technique. As resulting
	table will not be able to replicate temporal values directly,
	Lagrange interpolation is used.
-	Updated the data series. It now contains updated data series from
	Department of Health Philippines last JUN 07 2021.