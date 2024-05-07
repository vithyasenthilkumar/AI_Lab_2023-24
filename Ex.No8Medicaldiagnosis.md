# Ex.No: 8  Logic Programming –  Medical Diagnosis Expert System
### DATE: 23/03/2024                                                                           
### REGISTER NUMBER : 212221040182
### AIM: 
Write a Prolog program to build a medical Diagnosis Expert System.
###  Algorithm:
1. Start the program.
2. Write the rules for each diseases.
3. If patient have mumps then symptoms are fever and swollen glands.
4. If patient have cough, sneeze and running nose then disease is measles.
5. if patient have symptoms headache ,sneezing ,sore_throat, runny_nose and  chills then disease is common cold.
6. Define rules for all disease.
7. Call the predicates and Collect the symptoms of Patient and give the hypothesis of disease.

### Program:
```
hypothesis(Patient,german_measles) :- 
 symptom(Patient,fever), 
 symptom(Patient,headache), 
 symptom(Patient,runny_nose), 
 symptom(Patient,rash). 
hypothesis(Patient,flu) :- 
 symptom(Patient,fever), 
 symptom(Patient,headache), 
 symptom(Patient,body_ache), 
 symptom(Patient,conjunctivitis), 
 symptom(Patient,chills), 
 symptom(Patient,sore_throat), 
 symptom(Patient,runny_nose), 
 symptom(Patient,cough). 
hypothesis(Patient,common_cold) :- 
 symptom(Patient,headache), 
 symptom(Patient,sneezing), 
 symptom(Patient,sore_throat). 
hypothesis(Patient,chicken_pox) :- 
 symptom(Patient,fever), 
 symptom(Patient,chills), 
 symptom(Patient,body_ache), 
    symptom(Patient,rash). 
hypothesis(Patient,measles) :- 
 symptom(Patient,cough), 
 symptom(Patient,sneezing), 
 symptom(Patient,runny_nose). 
symptom(raju,headache). 
symptom(raju,sneezing). 
symptom(raju,sore_throat).
```
### Output:
![image](https://github.com/vithyasenthilkumar/AI_Lab_2023-24/assets/127177445/396f7798-79f5-4e3b-a27c-760d5a69fe03)
![image](https://github.com/vithyasenthilkumar/AI_Lab_2023-24/assets/127177445/c31a6f22-61f1-40ca-b370-b68de7f8ce44) 
![image](https://github.com/vithyasenthilkumar/AI_Lab_2023-24/assets/127177445/2621c3da-2b11-491d-acdd-66847c9fc9e0)
![image](https://github.com/vithyasenthilkumar/AI_Lab_2023-24/assets/127177445/fe71fe8a-43a7-448f-85cd-da1fd7a0b53a)
### Result:
Thus the simple medical diagnosis system was built sucessfully.
