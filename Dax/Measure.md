# DAX Measures

## 1. Total Incidents
Total Incidents = DISTINCTCOUNT('cyber_incident_analytics global_incident'[incident_id])

Counts the total number of unique cyber incidents.

## 2. Incidents with Parsed Start Date
Incidents with Parsed Start Date = CALCULATE([Total Incidents], NOT ISBLANK('cyber_incident_analytics global_incident'[parsed_start_date]))

Counts incidents where a valid parsed start date is available.

## 3. Incidents Having Receiver Data
Incidents Having Receiver Data = CALCULATE([Total Incidents], NOT ISBLANK('cyber_incident_analytics receiver'[incident_id]))

Counts incidents that have receiver information.

## 4. Distinct Receiver Entities
Distinct Receiver Entities = DISTINCTCOUNT('cyber_incident_analytics receiver'[receiver_entity])

Counts unique receiver entities affected by cyber incidents.

## 5. Average Impact Score
Average Impact Score = AVERAGE('cyber_incident_analytics impact'[impact_score])

Calculates the average impact score across incidents.

## 6. High Impact Incidents
High Impact Incidents = CALCULATE([Total Incidents], 'cyber_incident_analytics impact'[impact_score] >= 7)

Counts incidents with an impact score of 7 or higher.

## 7. Attributed Incidents
Attributed Incidents = DISTINCTCOUNT('cyber_incident_analytics attribution'[incident id])

Counts incidents with available attribution information.

## 8. Attribution %
Attribution % = DIVIDE([Attributed Incidents], [Total Incidents], 0)

Calculates the percentage of total incidents that have attribution data.

## 9. Average Weighted Intensity
Average Weighted Intensity = AVERAGE('cyber_incident_analytics global_incident'[weighted_intensity])

Calculates the average weighted intensity of cyber incidents.