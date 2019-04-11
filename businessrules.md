# Sistem informatic pentru gestionarea documentelor electronice

## Utilizator
Un utilizator este oparatorul uman care interactioneaza cu sistemul. 
- Isi poate crea cont in sistem
- Se poate loga in sistem
- Isi poate modifica datele in sistem
- Isi poate reseta parola
- Poate adauga, vizualiza, edita, sterge, descarca, impartii foldere si fisiere.
- Are rol de **proprietar** asupra fisierelor si folderelor create de el
- Are rol de **imputernicit** asupra fisierelor impartite cu el.
- Un utilizator **imputernicit** poate avea drepturi **totale** sau de **vizualizare** asupra folderelor si fisierelor impartite cu el.

## Folder
Un folder reprezinta o grupare de fisiere.

- Poate fi modificat, sters, vizualizat, descarcat in forma `.zip` de catre utilizatorul **proprietar** sau utilizatori **imputerniciti** cu drepturi **totale**.
- Poate fi vizualizat si descarcat in forma `.zip` de catre utilizatorii **imputerniciti** cu drepturi de **vizualizare**.

## Fisier
Un fisier reprezinta un document de o varietate de tipuri. (`.docx .png .pdf .xlsx .html .md`, etc)

- Poate fi modificat, sters, vizualizat, descarcat de catre utilizatorul **proprietar** sau utilizatori **imputerniciti** cu drepturi **totale**.
- Poate fi vizualizat si descarcat de catre utilizatorii **imputerniciti** cu drepturi de **vizualizare**