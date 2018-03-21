# Aplicatie educationala Supplementary Specification

# Introduction
Acest document cuprinde cerintele de sistem care nu sunt incluse in modelul cazurilor de utilizare. Aceste cerinte cuprind:
- Cerințe  de reglementare, inclusiv standardul de aplicare
- Atributele de calitate ale sistemului care urmează să fie construite, inclusiv cerințele de utilizare, fiabilitate, performanță și sustenabilitate.
- Alte cerințe, cum ar fi sistemul de operare și mediile, cerințele de compatibilitate și constrângerile de proiectare.

# Non-functional Requirements

Sistemul ar trebui să fie tot timpul cu toate informațiile la zi, conectat la server și să se salveze informațiile în timp real, fără să se piardă. Acest lucru va fi posibil folosind CRUD de catre administrator pentru a modifica baza de date.

## Availability

Va fi valabil pe fiecare calculator conectat la internet.

## Performance

Una dintre cele mai importante cerințe nefuncționale ale clienților este un sistem cu o rată de performanță bună și rapidă. Prin urmare, obiectivul de performanță este împărțit în trei sub-obiective: timpul, spațiul și răspunsul. Fiecare cerere către server este procesată cât mai repede posibil și răspunsul sau eroarea sunt trimise înapoi utilizatorului

## Security

Un utilizator are acces numai la datele sale personale, după o autentificare reușită. O parolă validă este un șir care are minimum 8 caractere, care conține atât litere mari, cât și litere mici și un caracter numeric. Va fi sigur, datele vor fi protejate intr-o baza de date, iar fiecare utilizator are anumite drepturi care nu vor putea fi incarcate.

## Testability

Acesta poate fi testat la inceput local, pentru a vedea toate problemele cu acest sistem. Voi folosi JUnit teste si testare manuala sau/si automata.

## Usability

Va putea fi utilizat de orice persoana fizica, care are cunostinte minime despre utilizarea unui calculator.

# Design Constraints

Proiectul va fi implementat in limbajul Java, fiind un limbaj de programare de nivel inalt, impreuna cu Windowbuilder  care va fi utilizat pentru  interfata grafica, si MySql pentru data de baze unde voi retine informatiile. 
Utilizatorul va accesa aplicatia, se conecteaza cu datele de logare si in functie de drepturile atribuite poate face diverse operatii.


# Resources

* http://www.upedu.org/process/gdlines/md_srs.htm
* Example of Supplementary Specification: http://csis.pace.edu/~marchese/SE616_New/Samples/Example%20%20Supplementary%20Specification.htm
