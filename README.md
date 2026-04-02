Obiectivul proiectului:

 Obiectivul acestui proiect a fost crearea unei baze de date relationale care sa gestioneze activitatea unui hotel. Mi-am dorit sa digitalizez receptia unui hotel,  astfel in loc sa tina evidenta pe un caiet, hotelul va avea o baza de date clara unde se poate vedea cand sunt camera libere, cine sunt angajatii etc. Practic scopul  este sa nu se piarda date si sa se faca cat mai putine greseli (de exemplu sa nu cazam doi oameni in aceeasi camera in acelasi timp).

Descrierea tabelelor:

1.	TIPURI_CAMERE: Aici se stocheaza categoriile de camere: Standard, Deluxe sau Suite, cat costa pe noapte si pentru cate personae este destinate camera.
2.	CAMERE: Aici sunt stocate camerele propriu zise. Pentru fiecare camera stim la cee taj se afla, daca are vedere la mare si ce tip de camera este, asfel are legatura cu tabela de mai sus.
3.	ANGAJATI_HOTEL: Aici sunt stocati toti salariatii. Pe langa nume prenume si salariu, am implementat o ierarhie: fiecare angajat are un sef adica managerul, iar acesta se afla tot in lista de angajati.
4.	TURISTI: Aici se afla clientii. Se salveaza numele, prenumele, numarul de telefon si am adaugat si o conditie pentru email, ca sa nu avem acelasi client inregistrat de doua ori.
5.	REZERVARI: Aceasta este tabela centrala. Cand vine un client se creeaza o rezervare. Aici se stocheaza cine a venit, adica turistul, angajatul cu care a interactionat si data tranzactiei.
6.	DETALII_REZERVARE: O rezervare poate include mai multe camera asa ca nu puteam sa scriem totul in tabela rezervari. Am creat aceasta tabela legatura unde sunt mai multe detalii despre rezervare.
