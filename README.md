   Aplicatia se imparte in doua: un site web, unde vor avea acces toti utilizatorii indiferent de roluri si o aplicatie Desktop, care va fi accesibila doar directorului. 
Aplicatia web ofera posibilitatea utilizatorului sa se inregistreze, adaugand detalii despre urmatoarele date: nume, prenume, email si parola (care va fi criptata) cu care acesta se va loga la urmatoarele accesari ale site-ului. 
La prima inregistrare, utilizatorul va primi implicit rolul de EMPLOYEE, care ulterior va putea fi modificat doar de catre director (avand rol de ADMIN). 
Dupa cum am amintit mai sus, aplicatia ofera acces diferit utilizatorilor in functie de rolul pe care acesta il are.
Aplicatia Desktop, destinata directorului, va permite vizualizarea tuturor angajatilor, assignarea rolurilor sau unassignarea acestora, vizualizarea departamentelor si implicit a angajatilor din acele departamente. Din aplicatia Desktop acesta nu va putea crea departamente sau adauga angajati acestora. Acest lucru va fi posibil prin aplicatia web care ii va permite acestuia accesul la functionalitatile amintite mai sus.


   Aplicatia are la baza un server dezvoltat folosind framework-ul JAVA Spring Boot, care inglobeaza endpoint-urile necesare, metodele si serviciile pentru ca aplicatia sa satisfaca nevoile companiei.  
Clasele folosite pentru implementarea serverului se impart in 5: Controller-e, Repository-uri, Service-uri, Clasele de baza care vor avea tabele corespunzatoare in baza de date si clasele ce ofera securitatea aplicatie bazata pe roluri. Mai jos este atasata diagrama aplicatiei, bineinteles completata de relatiile dintre clase:
![java](https://github.com/constantinescu-ciprian-30127/EmployeeManagement/assets/92230508/29118888-8703-491b-b625-cffa59b7e683)

   Aplicatia Desktop ofera directorului o interfata grafica realizata folosind Windows Forms Application, o aplicatie de tip client ce comunica cu serverul prin HTTP Request. Diagrama claselor este prezentata mai jos:
![ClassDiagram1](https://github.com/constantinescu-ciprian-30127/EmployeeManagement/assets/92230508/da73605c-9c1f-4694-8ca5-14b4a62dfaed)

   La final, dar poate ca cea mai importanta componenta din aplicatia noastra este baza de date, unde sunt stocate datele importante, fara de care aplicatia nu ar putea functiona optim. Diagrama tabelelor si relatiile dintre acestea sunt prezentate mai jos:
![db](https://github.com/constantinescu-ciprian-30127/EmployeeManagement/assets/92230508/45c3bbed-8de1-43f1-a497-d2d4fab2d774)
 	
