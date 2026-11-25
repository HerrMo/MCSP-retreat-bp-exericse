# Data dictionary

## Study

Fully synthetic teaching data from a simulated randomized study comparing
a structured blood-pressure management programme with usual care.

Systolic blood pressure is measured at baseline and after 12 weeks.
No real patient records are included.

## Variables

| Variable | Description | Format or coding |
|---|---|---|
| patient_id | Synthetic participant identifier | Text, e.g. `P0001`; identifies a unique patient |
| group | Randomized study group | `usual_care` = usual care; `programme` = structured blood-pressure management programme |
| age_years | Age at baseline | Integer, in years |
| sex | Simplified synthetic sex variable | `female` or `male` |
| bmi_kg_m2 | Body mass index at baseline | Numeric, in kg/m² |
| diabetes | Diabetes status at baseline | `0` = absent; `1` = present |
| sbp_baseline_mmhg | Systolic blood pressure at baseline | Numeric, in mmHg |
| sbp_12wk_mmhg | Systolic blood pressure after 12 weeks | Numeric, in mmHg |

## File format and missing values

- Filename: `bp_study.csv`
- Format: comma-separated values with a header row.
- Decimal separator: point.
- Blank fields indicate missing values.
- Each patient should contribute one record to the analysis.

## Interpretation

The variable distributions and study outcomes were constructed for
teaching and are not calibrated to a specific clinical population.
The limited categories used for sex are a teaching simplification.

Results do not provide evidence about the effectiveness of any
clinical intervention.
