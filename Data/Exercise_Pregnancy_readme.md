Information about the Exercise During Pregnancy data set
================
## *Introductory Statistics for the Health Sciences*, by Lise DeShea and Larry E. Toothaker

The purpose of this document is to provide background on the data set on exercise during pregnancy.  The data came from the following study:
 * Price, B. B., Amini, S. B., & Kappeler, K. (2012).  [Exercise in pregnancy:  Effect on fitness and obstetric outcomes – a randomized trial.](http://www.ncbi.nlm.nih.gov/pubmed/22843114)  *Medicine & Science in Sports & Exercise, 44, 2263-2269*.  doi:10.1249/MSS.0b013e318267ad67

These researchers randomly assigned sedentary women in the 12th to 14th week of pregnancy to one of two groups.  One group remained sedentary, and the other group participated in an exercise program.  Those in the exercise group engaged in moderate aerobic exercise for 45 minutes to an hour four times per week through the 36th week of pregnancy.  The groups were compared on muscular strength, aerobic fitness, delivery method, recovery time, and baby birth weight.  Strength and aerobic fitness were measured on five occasions:  12-14 weeks gestation (which served as the baseline, before the intervention began), 18-20 weeks gestation, 24-26 weeks gestation, 30-32 weeks gestation, 6-8 weeks after delivery.

Variables in the data set:
 1. **ID**: A unique number assigned to each participant.
 2. **Group**:  An indicator for the participant’s assignment to a group, where a = active and c = control.
 3. **T1_lifts**:  At Time 1 (baseline:  12-14 weeks gestation), the number of times that the participant could lift a 7-kg medicine ball from the floor to waist height in 1 min.
 4. **T2_lifts**:  Like T1_lifts, but measured at Time 2 (18-20 weeks gestation).
 5. **T3_lifts**:  Like T1_lifts, but measured at Time 3 (24-26 weeks gestation).
 6. **T4_lifts**:  Like T1_lifts, but measured at Time 4 (30-32 weeks gestation).
 7. **T5_lifts**:  Like T1_lifts, but measured at Time 5 (6-8 weeks after delivery).
 8. **T1_watts**:  At Time 1, a measure of power in watts produced during a 3.2-km walk or run.  Power was calculated by multiplying the participant’s weight and the distance covered, divided by time.  
 9. **T2_watts**, **T3_watts**, **T4_watts**, **T5_watts**:  Like T1_watts, but measured at Times 2, 3, 4 and 5.
 10. **DelivMethod**:  An indicator of delivery method (1 = vaginal, 0 = cesarean).
 11. **PrimaryC**:  An indicator of whether the delivery was the first time that the participant had a cesarean (1 = yes; 0 = no, the mother previously had a cesarean delivery; missing values = the delivery was vaginal).
 12. **Babyweigh**t:  Baby’s birth weight in grams.
 13. **RecovDays**:  Number of days postpartum that the mother returned to being able to perform 3 of 5 listed household tasks (“changing sheets and making beds; sweeping, mopping, vacuuming, or other cleaning; washing and folding clothes; shopping for groceries and putting groceries away; preparing, cooking, and serving meals”).