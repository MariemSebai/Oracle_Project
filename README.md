# Oracle-Project

You are given the following ADMMEDIC database diagram which represents visits to a new medical center.

Medecin(matricule, nom_med, prenom_med, specialite),</br>
Patient(noss,nom_pat, prenom_pat, nbpriseMax, quantiteMax),</br>
Medicament(code_med, libelle),</br>
Consultation(Num_consul, date_consult, #matricule, #noss),</br>
Prescription(#code_med, #Num_consul, nbprise, quantite).</br>

Required work :
Using Oracle as your database management system, you are asked to answer the following questions:

1. Creation of tables. <br/>
2. Filling the tables with fictitious data. <br/>
3. Creation of the sequences and triggers necessary for supplying the primary keys of the tables. <br/>
4. Create a trigger that allows you to check, when inserting a row in the Prescription table, whether the number or quantity does not exceed the maximum values ​​indicated in the medication table. If this is the case, an alarm message should be displayed to notify the doctor that he has exceeded normal doses. <br/>
5. We want to create a package containing the following functions and procedures: <br/>
• For each table creation of a PinsertTableName procedure which takes as input as many parameters as there are attributes in the table and allows a new row to be inserted in the latter. <br/>
• For each table creation of a PUpdateNomTable procedure which takes as input as many parameters as there are attributes in the table and allows updating the row whose primary-key corresponds to the number passed as a parameter. <br/>
• For each table, creation of a PDeleteNomTable procedure which takes as input a number p_id and allows deleting the row whose primary-key corresponds to the number p_id passed as a parameter. <br/>
• A procedure that allows you to display the list of first and last names of physicians knowing their specialty. <br/>
• A function which calculates and returns for a given doctor (whose number is passed in parameter) the percentage of consultation (PC) carried out by this one; knowing that PC is calculated as follows: <br/> PC = nb_consultation_medicin / nb_consultations_total. <br/>
• A procedure which allows to display for a given patient (whose social security number is passed as a parameter) the list of the names of the doctors with whom he has made consultations and the dates of the consultations. The list should be ordered in chronological order of consultation. <br/>
• A procedure that allows you to display for a given patient (whose social security number is passed as a parameter) the list of drugs that have been prescribed and their number of doses. <br/>
NB
- In all functions and procedures it is necessary to plan to program the exception management part.
