# Investigating-the-No-Show-Trend-in-Medical-Appointments-in-Brazil-in-2016--Data-Analysis-Project

## Following files are included in this repository:

### Files given/used:
* Dataset can be found [here](https://github.com/ShaheerKhan200/Investigating-the-No-Show-Trend-in-Medical-Appointments-in-Brazil-in-2016----Data-Analysis-Project/blob/main/noshowappointments-kagglev2-may-2016.csv).

### Code
* Code: code for gathering, assessing, cleaning, analyzing, and visualizing data, can be found [here](https://github.com/ShaheerKhan200/Investigating-the-No-Show-Trend-in-Medical-Appointments-in-Brazil-in-2016----Data-Analysis-Project/blob/main/Project%202%20Code.ipynb).

### Result:
* Report: documentation of analysis and insights into final data can be found [here](https://github.com/ShaheerKhan200/Investigating-the-No-Show-Trend-in-Medical-Appointments-in-Brazil-in-2016----Data-Analysis-Project/blob/main/Project%202%20Report-.html).


## Dataset

The dataset that I have wrangled, analyzed and visualized is a gathered information from 100k medical appointments in Brazil and is focused on the question of whether or not patients show up for their appointment. A number of characteristics about the patient are included. The analysis will be tackling 2 questions which help with the understanding of the characteristics that cause patients to miss their appointments in Brazil based on the data from 2016.

This analysis will be addressing 2 questions as shown below:
* Research Question 1: Based on the characteristics/factors given about the patient. Which factor/factors have a drastic affect on the patients missing their appointment or What factors if any, have more patients miss their appointment than attended?

* Research Question 2: Given the patient has missed the appointment, what factor(s) is/are an indicator for a scheduled appointment to be missed?


Following Variables were used in the analysis:
* Gender: Depicts whether the patient is Male(M) or Female(F) - (Categorical)
* Scheduled_Date: Signifies the date the patient registered their appointment - (Quantitative) *Feature Engineered Variable*
* Scheduled_Time: Signifies the time the patient registered their appointment - (Quantitative) *Feature Engineered Variable*
* Scheduled_Hour:	Signifies the hour the patient registered their appointment - (Quantitative) *Feature Engineered Variable*
* Scheduled_Weekday: Signifies the weekday (ie Monday, Tuesday etc) the patient registered their appointment - (Categorical) *Feature Engineered Variable*
* Appointment_Date: The date of the actual appointment, when the visit to the doctor happens
* Appointment_Month	The month of the actual appointment, when the visit to the doctor happens - (Quantitative) *Feature Engineered Variable*
* Appointment_Day: The day of the actual appointment, when the visit to the doctor happens - (Quantitative) *Feature Engineered Variable*	
* Appointment_Weekday: The weekday (ie Monday, Tuesday etc) of the actual appointment, when the visit to the doctor happens - (Categorical) *Feature Engineered Variable*
* Age: The age of the patient - (Quantitative)
* Neighbourhood: The neighbourhood where the appointment takes place/indicates the location of the hospital. - (Categorical)
* Scholarship: Indicates whether or not the patient is enrolled in Brasilian welfare program called Bolsa Família - (Categorical)
* Hypertension: Indicates whether the patient has Hypertension or not - (Categorical)
* Diabetes: Indicates whether the patient has Diabetes or not - (Categorical)
* Alcoholism: Indicates whether the patient has Alcoholism or not - (Categorical)
* Handicap: Indicates whether the patient is Handicaped or not - (Categorical)
* SMS_received: Indicates whether sms was received by the patient or not prior to the appointment - (Categorical)
* Appointment_Missed: Indicates whether the patient has shown up or not. "Yes" signifies that the patient did not show up to the medical appointment and "No" means the opposite - (Categorical)
* Age_Group: age broken down into 3 categories 'Children_Adolescents' (<= 14), 'Adult' (>= 15 and <= 64), 'Senior' - (Categorical) *Feature Engineered Variable*


## Summary of Findings

Research Question 1:

* Females attended and missed more number of appointments than Males. In conclusion, number of missed appointments by both genders were less than the number of attended appointments.

* The gender factor is not a good idicator as neither of the gender have more patients miss their appointment than attended.

* The senior age group have the most patients attending their appointments at 84.6% compared to about 80% of the remaining age groups. The age factor had more patients attending their appointments than missing it in all of the age groups. Hence the age factor is not a good indicator to show if a patient will show up for their scheduled appointment or not.

* The 7 am time seems to have the least number of missed appointments and the most appointments attended. Other than that the scheduled hour factor had more or less similar proportion figures of patients attending their appointments or missing it in the scheduled hours and none of the hours had more patients missing their appointments than attending them.

* Tuesday amongst the other weekdays have the most number of appointments missed and attended followed by Wednesday and Monday. Whereas Saturday witnessed the least number of appointments attended and missed.

* The month of May received the most number of attended and missed appointments, followed by June and April.

* Tuesday and Wednesday are the busiest day, both the days received similar number of attended and missed appointments, followed by Monday, Friday and then Thursday.

* Neighbourhood JARDIM CAMBURI has the most number of missed and attended appointments followed by MARIA ORTIZ. On the contrary the least number of appointments were recorded in AEROPORTO neighbourhood.

* Patients granted scholarship have more missed appointments than those patients with no scholarship, though more data would be required to substantiate the observation made. Scholarship factor didn't cause more number of appointments being missed than attended.

* Patients with hypertension seem to have more appoinments being attended than patients with no hypertension.

* Patients with diabetes have more appoinments being attended than patients with no diabetes.

* Patients who are handicapped attended more appoinments than non-handicapped patients.

* Patients receiving the SMS seems to show more number of appointments being missed than those who don't receive any SMS.

Research Question 2: 

* Only 20% of the patients have missed their appointment.

* Females tend to miss their appointments more based on the data given. Almost twice as more number of females have missed their appointments than males. Hence Gender is a strong indicator for a scheduled appointment to be missed.

* Adults tend to miss their appointments more. Almost thrice as more adults miss their appointments than children and almost 10 times as more adults missed their appointments than seniors. Hence Age Group is a strong indicator for a scheduled appointment to be missed.

* Majority of appointments that were missed occured when the appointments were booked from 7 to 10 am and at 2 pm. Least number of appointments missed occured when the appointment was booked at 6 am and 5-9 pm. To conclude, the scheduled hour factor is a good indicator to show if a patient will show up for their scheduled appointment or not.

* Tuesday amongst the other weekdays have the most number of appointments missed followed by Wednesday and Monday. Whereas Saturday witnessed the least number of appointments attended and missed. Scheduled Weekday factor is not a strong indicator for appointments to be missed.

* The month of May received the most number of missed appointments almost 26 times more than April and 3 times more than June. Based on this, the appointment month factor could be a good predictor to show if a patient will show up for their scheduled appointment or not, but more data is needed from other months to make an accurate analysis.

* Tuesday among the other weekdays have the most number of appointments missed followed by Wednesday and Monday. Whereas Saturday witnessed the least number of appointments missed. Appointment Weekday factor is not a strong indicator for appointments to be missed.

* JARDIM CAMBURI has the most number of missed appointments followed by MARIA ORTIZ. On the contrary there were no missed appointments in ILHA DO BOI, ILHA DO FRADE and AEROPORTO neighbourhood.

* The Scholarship factor indicates whether or not the patient is enrolled in Brasilian welfare program called Bolsa Família and how this contributed to appointments being missed. Patients with scholarship had 8 times less appointment being missed than those patients who have no scholarship. the scholarship factor is a very strong indicator for appointments to be missed.

* Patients with no hypertension had about 5 times more appointments being missed than those patients who have hypertension.

* Patients with no diabetes had about 15 times more appointments being missed than those patients who have diabetes. Diabetes factor is a very strong indicator for appointments to be missed.

* Patients with no alcoholism had about 32 times more appointments being missed than those patients who have alcoholism. The alcoholism factor is a very strong indicator for appointments to be missed.

* Patients who are not handicap had about 61 times more appointments being missed than those patients who are handicap. The handicap factor is a very strong indicator for appointments to be missed.


## References

[1] https://www.thetopsites.net/article/52692083.shtml

[2] https://medium.com/@deallen7/managing-date-datetime-and-timestamp-in-python-pandas-cc9d285302ab#1b5b

[3] https://www.datacamp.com/community/tutorials/converting-strings-datetime-objects

[4] https://datatofish.com/strings-to-datetime-pandas/

[5] https://www.dezyre.com/recipes/split-datetime-data-create-multiple-feature-in-python

[6] https://en.wikipedia.org/wiki/List_of_countries_by_age_structure

[7] https://www.mmbyte.com/article/2228.html

[8] https://medium.com/@morganjonesartist/color-guide-to-seaborn-palettes-da849406d44f

[9] https://stackoverflow.com/questions/35692781/python-plotting-percentage-in-seaborn-bar-plot
