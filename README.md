# OSHA-Workplace-Injuries
## overview
Analyzes 90K+ OSHA records from 2015–2024 to identify injury trends across industries and body regions. Includes data cleaning, custom calculations, and Tableau visuals that reveal the top injury type for each body region and highlight key workplace safety patterns.

## Dataset Description
 **Source:** OSHA workplace injuries https://www.osha.gov/severe-injury-reports  <br />
 **Tables:** 1 CSV file  <br />
 **Time period:** 2015-2024  <br />
 **Rows:** 99491  <br />

 **Table** <br />
 
| Column Name | Description |
| --- | --- |
| Id |Id of the injury |
| UPA | A unique identifier assigned by OSHA to the establishment (employer location) that reported the severe injury or illness. It serves as the primary key for linking the injury case back to the specific facility details (name, address, NAICS code, etc.). |
| EventDate|Date of injury occurance  |
| Employer |Name of Employer |
| Address1| Address of Employer |
| Address2| Physical street address for location, mapping, and mailing purposes.|
| City |The city where the establishment is located. |
| State| The state where the establishment is located.|
| Zip|The full zip code for the establishment. |
|Latitude | The latitude of employer|
| Longitude| The longitude of employer |
| Primary NAICS	|The North American Industry Classification System (NAICS) code for the establishment|
|Hospitalized |Number of hozpitilized people within each record |
| Amputation| Number of amputated parts people within each record|
| Loss of Eye| Number of eays lost within each record|
| Inspection| inspection reference number|
| Final Narrative| Details about the injury|
| Nature|4-digit code of nature of injury. |
|NatureTitle | The nature title of the injury|
| Part of Body| Code for the part of the body Affected|
| Part of Body Title|Specific title of the Body Affected |
|Event | Event code for category of event|b
| EventTitle|Title of event  |
| Source| 4-digit code for source of injury|
| SourceTitle|Title of source of injury |
| Secondary Source |4-digit code for secondary source of injury |
| Secondary Source Title| Title of secondary source of injury|
|FederalState |Indicates whether the establishment is covered by a State OSHA Plan (True) or by Federal OSHA (False). |
| Industry| The industry of the estableshment |
| BodyRegion| General body region affected in the injury|
|Injury Type |Type of injury categorized from the NatureTitle column |
| Sector| Sector categorized from the industry column|
| EventCategory | Event of the injury categorized from the EventTitle column|
|Source_Category |Source of the injury category categorized from SourceTitle column |      

## Data Cleaning &amp; Preparation

Refer to Jupyter notebook <br />


## Key Insights / Results

## **Key Insights / Results**

* **Upper and lower limbs are the most frequently injured body regions**, with upper-limb cases showing the highest hospitalization rates. These regions account for the majority of reported incidents between 2015–2024.

* **Manufacturing and Construction are the sectors with the highest number of injuries**, including severe outcomes such as fractures and amputations. Both industries consistently appear in the top injury categories across sources, events, and body regions.

* **Texas reports the highest volume of workplace injuries**, making it the leading state in total incidents. Other high-incident states include California and Florida, but Texas remains the clear outlier.

* **Fractures, sprains, and lacerations dominate as the top injury types**, varying in rank depending on the body region. This highlights the importance of analyzing injuries by region rather than relying on overall counts.

* **Injury severity varies significantly by body region**, with areas like the upper limbs showing higher proportions of hospitalization and amputation compared to torso or internal system injuries.

* **Industry-specific patterns are clear:**

  * Manufacturing shows high rates of cuts, fractures, and machinery-related injuries.
  * Construction is more prone to falls, striking injuries, and equipment-related incidents.

* **Trends across the 10-year dataset indicate a general increase in reported injuries**, posing a growing challenge for worker safety and compliance requirements.

## Recommendations
1. Prioritize Safety Measures for Upper and Lower Limbs
Upper and lower limbs account for the highest number of injuries, with upper limbs showing significantly higher hospitalization rates.
Recommendation:
* 	Introduce stricter PPE enforcement (gloves, arm guards, footwear).
* 	Increase training on safe manual handling and tool use.
* 	Implement ergonomic redesigns for repetitive-motion tasks.
2. Improve Safety in Manufacturing and Construction
Manufacturing and construction show the highest number of injuries and amputations.
Recommendation:
* Strengthen lockout–tagout (LOTO) compliance.
* Increase inspection frequency on mechanical and powered equipment.
* Use digital checklists for hazardous operations to reduce human error.


## Conclusion
* Upper and lower limbs account for the majority of injuries, with upper-limb cases showing significantly higher hospitalization rates, emphasizing the need for stronger protective measures and safer handling practices.
* Manufacturing and construction experience the highest injury burden, including severe cases such as amputations, highlighting the importance of stricter machine safety, improved training, and enhanced hazard controls in these sectors.
* Texas reports the highest number of injuries among all states, indicating a need for focused safety initiatives, stronger regulatory enforcement, and targeted industry interventions within the region.

## Tools & Libraries

* Python: pandas, numpy
* Jupyter Notebook
* Tableau for visulizations




