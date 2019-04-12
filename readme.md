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

## Diagrame de clase

![Relatie entitati](https://www.plantuml.com/plantuml/png/0/hPHDIyD048RlWVo79QUqceFNKgHYAnPgALezA1wspLW7DzcmknLK_E_E9fklDb8LSmZPUJFlpZoJpKWRhims4RxdUmQD07ODWXi41YcjwSagQy6rPhS61Rvp8nNxy3r6rn6RZjc0OMhAzNoR04MqKPXkok12GTeLdoGSnKuqOfTSFo-uaeBl9KnJ1Hka63SpFc1ZRc292PIPCqnV1kocaRAIKh0xKFY4QwwWi0t1xdlCidpLwtpJMeM2RYH_rWWkK2CqsX_Rnb3jjxR4R2zshi3MpNOBju1afX1e5YJMcAjTfCwL-LO8lX8mp0Ed5PM4Eg5XqHipWZCy4zAsKEcJc0Qfi9IBPIb7n0kK9j4Ii9qMIQyIO-SCOLrIhwNRr0s4xU2LZ7E8OG6h3T3LLXEihNS_fGMe13LtvVAgmeQRqtxYHiZRv1is1T_3G_tp0FzrGZPM9gxU33myKiMQ_ApbFMRXRsQKjzuxFFISLkC749m4h1z5BEW7xb1yA-TR-5u1kIau2bsI8z0bbRkvezXfsA5LZYD8O_hXVG40 "Relatie entitati")

![class.controllers](https://www.plantuml.com/plantuml/png/0/TLB1RiCW3Br7oZ_ak1tw2rMxPbiFhLQjcdP6O3Me14lWAAgc_VkW6Lv8Caxu6R_tRBpn91nrhIcBif16U5zjfSJEqWujEJG6t5TPLE4SyABjmoC7s56Atk6YFO7xYptGAP3rw5G2Nu4-FBWQI6ZZ4_giDDFi6f3NWxRN27mdFx4ekflvgbQhDMU7jtjiOMOy2B_rjaRPjM29bS-DSA2URaV8aKzDpO2nXHTjWEzer22PYztTfEHIwiunJKmR60YMMeZrx7shL1RNO80WGenWRmqAbVN6WtOW2APV4DgTocTDZQSnSpWu-4zz_Cl1-ynKbCvOHoDBiiUmDcUmYYLZy5kyk1thKKbyiWctiEa_ "class.controllers")

## Diagrame de secventa

![Creare cont](https://www.plantuml.com/plantuml/png/0/RLAzRiCW4DujyGudJucKv04yH56h3fshgbtFvfAYOh3Wy92dxs7oPwSUCBhxVhWF3f4nSEgjgbJ5XYt1Qo0C19rtd8lOiGzGVxAnveoohm4Zf4X1LODmJMS6T0pr5xNHC9MsKPL6nXOZGVs2PmHD89NIrks2-zQZiV11OQIYJxcGxRCHRFUYsC2xu-1rwYWKBLYvrDEcW3SWYjxYMZZcoXZH6eqt-D677la9ZrPgmGjELI1VvcS1iMukZPkIgiZAJ35r7SKxV2ypDH3HZZGDc-roWk1yAYZT5b4vLI7FsDEH6h36_O8aRiRh5S1gQgqBUDh3zljoDWwcbyW5MkBAaDrkTn5-I0wpOPPyDbZES8iiGqjpcSzY79S0uUWZmmdb1Tmninm7F1c7Cvs79EE_oa-zcUAFxqbKbq6Jqt99UL7LGVxokFy0 "Creare cont")

![Login](https://www.plantuml.com/plantuml/png/0/fL91QiCm4BmBz8V5bxRGVC274agFlOQUrzAcMQhOnhionQ_loZ9D23aKUZ7op6XcTkszA4wQpyaxxvGr4RmFdzoNLmmwJD0Sb1ClQES6K20BJTwDTei3ZzWhD1_K2IjLchsBgDYX43Ilk2140aCg7Jll7k0YU6C9SEI5GwLPlafq2O7TYxcra4eVU2pGyuWYJsipdiroJSjSbB5h8M2sQGpzRMpIf43JOB3rwc2tcLuam3rzioZrMhsAmh9Q6D62SRjTQtX7oMhVCOnhdQlWMgjGCoQEnUA4SZBNQKZuvoZ98P38_xFgYWJJJEMZ20dddkwjxyZ2TBF6g_IDlfdWD9p9fZ2O-kZTtfxsL_q0 "Login")

![Fisier Nou](https://www.plantuml.com/plantuml/png/0/PL4nRiCm3DmD-0-4ftR81pmKGL5qx5PafYMc8Ah8XaXbyEjBMROGD9CatXtlH9v5CMc-XRxhEsKD19yiJ0c-vbngw7HEC7mh1rxHxWEWG1PAVRUOb1ql61M62qt2IXNcllEeEA4G3E-u8dW2grJOJu_m1uk3Aw_iAiZoMuoB1PpUhDTew1OfpXbU_EpoZQA-6eKFmXq3UqpLetXnr6HlonyKACtRVUTRut6lDM7VKR0mafqZEPX-UhHkLGiuWc2uq_QnFOzzoG0uxOcUEpdCMYnhHuBSHchIgGa3sqeEKjMtq0l-SCJ_58g-3Enifoto3m00 "Fisier Nou")

## Diagrama de stare

![Stari Fisier](https://www.plantuml.com/plantuml/png/0/NP3DQWCn38Jl1h_3d0DvWHnA3g7GGqeXnz23M2iWwfz5bdleqrVP_cox5zlCo9z6EdOZjL5o336OM6PSN14yIXVMkthTlMA_Vy1p6p7uSS2fJQDmjP71w9JVoJ0palItxuglt-wJCcPjimex5bsGk8uYoalb0Zwt93UPo5RfgSmUIrpvUMsOHQeKZ0hAXc6IvOEiAQYtILQIeox6scDOhWFEfDu84-4cKXFwF_UbaR4xKFQz3Bs3rWZuW_lDZ6sFxKYhw8kCuSWr-Re_0G00 "Stari Fisier")

## Diagrama de activitate

![activity.login](https://www.plantuml.com/plantuml/png/0/VP312i8m38RFBVGTUkn0z3uPJ0LFdXGVeDZC5hfsDAs-lgbJK0HF2Vd__5z8ZrcdN4OlkE3FNl1sSxd44l8kXfoYzv2MXtXrGS6edL_8IIFUOpBDchnd97dlWfdLEXFS3QhE6vaj1Aa6xH4QmLbxX60WgQqsif1XLQFg2iCS9y61V5BbL6QtbPsq6gtw938A9w6JJtALVp1_E2yG-oQnzWI8BeObwXkesVaEiN64xzrWt437paNmdZhwu0C0 "activity.login")
