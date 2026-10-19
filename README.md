# Subsea Asset Integrity Case Studies Using Python

## Project Overview

This project contains three practical case study exercises focused on subsea asset integrity, condition monitoring, and risk-based maintenance in the oil and gas industry.

The exercises apply Python-based data analysis, engineering calculations, and visualisation techniques to assess operating conditions, estimate equipment degradation, and identify potential failure risks in subsea production systems.

The work was carried out using Jupyter Notebook and synthetic asset-integrity/SCADA data for learning and demonstration purposes.

## Case Studies

### Case Study 1: Pressure–Temperature (P–T) Envelope Analysis

**Objective:** Assess subsea operating conditions against defined pressure and temperature operating limits to identify potential envelope exceedances.

**Key activities:**
- Analyse synthetic SCADA operating data.
- Compare recorded pressure and temperature values against their specified operating limits.
- Identify and count operating-envelope exceedances.
- Visualise operating conditions and highlight potential abnormal operating states.
- Interpret the results in the context of subsea asset integrity and operational monitoring.

**Engineering relevance:** Operating-envelope monitoring helps identify conditions that may contribute to equipment damage, flow-assurance problems, or reduced operational reliability.

### Case Study 2: Corrosion Prediction and Remaining Useful Life (RUL)

**Objective:** Estimate the remaining useful life of subsea jumpers using wall-thickness measurements, minimum allowable wall thickness, and corrosion-rate data.

**Key activities:**
- Work with synthetic asset-integrity and SCADA data alongside jumper inspection records.
- Calculate corrosion rates and assess wall-thickness degradation.
- Estimate the remaining useful life of six jumpers.
- Visualise RUL against corrosion rate.
- Apply colour-coded risk classifications to support maintenance prioritisation.

**Methodology:**

The remaining useful life is estimated using:

\[
RUL=\frac{t_{\text{current}}-t_{\text{minimum}}}
{CR}
\]

Where:

- \(t_{\text{current}}\) = current measured wall thickness (mm)
- \(t_{\text{minimum}}\) = minimum allowable wall thickness (mm)
- \(CR\) = corrosion rate (mm/year)

The calculation assumes a constant corrosion rate and is intended as a simplified screening estimate.

**Engineering relevance:** RUL estimation supports inspection planning, corrosion management, and maintenance prioritisation. Actual remaining life assessments require consideration of uncertainty, inspection quality, corrosion mechanisms, applicable codes, and operating conditions.

### Case Study 3: Failure Mode, Effects, and Criticality Analysis (FMECA)

**Objective:** Identify potential failure modes of a subsea Christmas tree, evaluate their consequences, and prioritise risks using a structured engineering assessment.

**Key activities:**
- Develop an FMECA worksheet covering at least 10 potential failure modes.
- Identify the potential effects and causes of each failure mode.
- Assign severity, occurrence, and detection ratings where applicable.
- Calculate Risk Priority Numbers (RPNs).
- Create a risk matrix plotting failure modes by severity and occurrence, with RPN values annotated.
- Identify higher-priority failure modes for further investigation and mitigation.

**Risk Priority Number:**

\[
RPN=S\times O\times D
\]

Where:

- \(S\) = Severity rating
- \(O\) = Occurrence rating
- \(D\) = Detection rating

The RPN provides a comparative prioritisation measure. It should not be treated as a standalone measure of absolute risk, and high-severity failure modes should receive appropriate attention even when their RPN is relatively low.

**Engineering relevance:** FMECA supports systematic failure identification, risk-based maintenance planning, and the development of mitigation strategies for critical subsea equipment.

## Tools and Technologies

- **Python** — engineering calculations and data analysis
- **Jupyter Notebook** — interactive analysis and documentation
- **Pandas** — tabular data manipulation
- **NumPy** — numerical calculations
- **Matplotlib** — data visualisation and risk plotting
- **Synthetic SCADA and inspection data** — demonstration datasets

## Project Scope and Limitations

- The exercises are educational case studies and use synthetic or exercise-provided data where applicable.
- The results are intended to demonstrate analytical methods rather than certify the integrity of an operating asset.
- Operating limits, corrosion rates, rating scales, and risk classifications should be verified against applicable engineering standards and project-specific requirements before real-world use.
- The RUL calculations assume a constant corrosion rate unless otherwise stated.
- FMECA ratings are dependent on the defined scoring criteria and available failure information.
- The analyses do not replace detailed engineering assessments, inspection programmes, or integrity-management procedures.

## How to Run the Notebooks

1. Install Python and Jupyter Notebook, or use Google Colab.
2. Install the required libraries if they are not already available:

   ```python
   %pip install pandas numpy matplotlib
   ```

3. Open the relevant `.ipynb` notebook.
4. Ensure that any required CSV files are available at the file paths referenced in the notebook.
5. Run the notebook cells sequentially.
6. Review the calculations, tables, plots, and engineering interpretations.

## Key Learning Outcomes

Through these exercises, the project demonstrates practical application of Python to:

- Monitor subsea operating conditions against pressure and temperature limits.
- Estimate corrosion-related remaining useful life.
- Identify and prioritise potential equipment failure modes.
- Communicate engineering findings through tables, calculations, and visualisations.
- Apply data analysis to asset-integrity and maintenance decision-making.

## Conclusion

These three case studies demonstrate how Python-based analysis can support subsea asset-integrity assessment, degradation monitoring, and risk prioritisation. They also provide a foundation for further work in predictive maintenance, machine learning, and digital asset management within the oil and gas industry.
