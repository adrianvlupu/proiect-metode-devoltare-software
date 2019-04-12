# Sistem informatic pentru gestionarea documentelor electronice

## Entitati si reguli de business

### Utilizator
Un utilizator este oparatorul uman care interactioneaza cu sistemul. 
- Isi poate crea cont in sistem
- Se poate loga in sistem
- Isi poate modifica datele in sistem
- Isi poate reseta parola
- Poate adauga, vizualiza, edita, sterge, descarca, impartii dosare si fisiere.
- Are rol de **proprietar** asupra fisierelor si dosarelor create de el
- Are rol de **imputernicit** asupra fisierelor impartite cu el.
- Un utilizator **imputernicit** poate avea drepturi **totale** sau de **vizualizare** asupra dosarelor si fisierelor impartite cu el.

### Dosar
Un dosar reprezinta o grupare de fisiere.

- Poate fi modificat, sters, vizualizat, descarcat in forma `.zip` de catre utilizatorul **proprietar** sau utilizatori **imputerniciti** cu drepturi **totale**.
- Poate fi vizualizat si descarcat in forma `.zip` de catre utilizatorii **imputerniciti** cu drepturi de **vizualizare**.

### Fisier
Un fisier reprezinta un document de o varietate de tipuri. (`.docx .png .pdf .xlsx .html .md`, etc)

- Poate fi modificat, sters, vizualizat, descarcat de catre utilizatorul **proprietar** sau utilizatori **imputerniciti** cu drepturi **totale**.
- Poate fi vizualizat si descarcat de catre utilizatorii **imputerniciti** cu drepturi de **vizualizare**

## Diagrama de utilizare

![usecase](https://www.plantuml.com/plantuml/png/0/ZP9D2W8n34Rt0tE7uCfPY3SGHJU2WYYw3zCu16exf1aNYdUtHSM_2dRPlFJBQpiEYgBTmPP5MMoLBPzGlS1WC8B-L0Y5eFPEg-_gmZViCljBRtZFDO919KiPOas1D9tSedYBLSeMgXLTOmbwA_6jS29W2FD3soc9uveL-keLRTK33F12dSi2ulgCcHZicXHZV40PxZamIPLd7qF_Hs_YH0tznqQ1UCESXr-itqMFVEemdIDqqtqhtuM_ubBUxjcPIypsp2X4zL_sbxAuf2SQapFnfrm1 "usecase")

## Diagrama de clase

Entitati sistem

![class](https://www.plantuml.com/plantuml/png/0/hLHTIyCm57qlz3zS-jHjzi7NCKHn4mTp39m-A3vastLUI9kIP8AA_zsaJVgnLQPYtt9ESkwvvoOzLvf9lKjv68J1cZEbu4uJftUcXOIFC03p3M0wXY5GflrwlalH84fBohOUN4ZCkl19oeZleGbSC_MoO59mTd1WcadSai6Odh4XZ9d69QLeBTeDAo4utAEaPrepYQL8ZBRA2UJ5gXS6dtL7LwG86zsChK-IXqwNb1zWbnAj3MZwyFsAN1AQ00rPfrPL4QfWvZlEsOhZg03EgYPJOrMJDZjcfjVH1HUscugVRCWeawVBfQSJkDKebI5j63wO0RmAsZXbZ6jBlHPlZsunReCtObFa6PTXjGDqtke4Q-dzcx50cP9YpYwh73RK7FSJDHDvE_c6J9dlyQ7-UO3_EY6B-OEhDusFJyQnCdfMye7o-3SpAbhl7HzwaLRZFKUd4VIJ1A9-v1x5jtHH8WpAa9k4Iw6BSWbqKRwQUugTWXrSfNYEsSRyfRu0 "class")

## Diagrame de secventa

![Login](https://www.plantuml.com/plantuml/png/0/fL91QiCm4BmBz8V5bxRGVC274agFlOQUrzAcMQhOnhionQ_loZ9D23aKUZ7op6XcTkszA4wQpyaxxvGr4RmFdzoNLmmwJD0Sb1ClQES6K20BJTwDTei3ZzWhD1_K2IjLchsBgDYX43Ilk2140aCg7Jll7k0YU6C9SEI5GwLPlafq2O7TYxcra4eVU2pGyuWYJsipdiroJSjSbB5h8M2sQGpzRMpIf43JOB3rwc2tcLuam3rzioZrMhsAmh9Q6D62SRjTQtX7oMhVCOnhdQlWMgjGCoQEnUA4SZBNQKZuvoZ98P38_xFgYWJJJEMZ20dddkwjxyZ2TBF6g_IDlfdWD9p9fZ2O-kZTtfxsL_q0 "Login")


![Fisier Nou](https://www.plantuml.com/plantuml/png/0/PL4nRiCm3DmD-0-4ftR81pmKGL5qx5PafYMc8Ah8XaXbyEjBMROGD9CatXtlH9v5CMc-XRxhEsKD19yiJ0c-vbngw7HEC7mh1rxHxWEWG1PAVRUOb1ql61M62qt2IXNcllEeEA4G3E-u8dW2grJOJu_m1uk3Aw_iAiZoMuoB1PpUhDTew1OfpXbU_EpoZQA-6eKFmXq3UqpLetXnr6HlonyKACtRVUTRut6lDM7VKR0mafqZEPX-UhHkLGiuWc2uq_QnFOzzoG0uxOcUEpdCMYnhHuBSHchIgGa3sqeEKjMtq0l-SCJ_58g-3Enifoto3m00 "Fisier Nou")
