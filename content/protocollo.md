---
title: "Protocollo di comunicazione"
date: 2021-12-27T18:30:31+01:00
---
Obiettivo del progetto Simone è stata la definizione di un protocollo standard che consenta la
comunicazione tra i centri di controllo delle flotte, i Centri Servizi Veicoli (nel seguito CSV) e i
Centri di Controllo Locale della Mobilità.
Con riferimento all'immagine, che illustra l'architettura del progetto S.I.MO.NE., il protocollo di comunicazione è indicato con i numeri 1 e 3.

<img src="/img/architettura2.png" style="margin: 5px auto; width:70%;" />

La comunicazione (1) tra i centri di controllo delle flotte (front end) ed il Centro Servizi Veicoli è
bidirezionale; i centri di controllo delle flotte trasferiscono i dati FCD verso il Centro Servizi Veicoli
mentre quest’ultimo restituisce dati di traffico elaborati, eventi di traffico e informazioni sulle ZTL.
Anche la comunicazione (3) tra il Centro Servizi Veicoli e la Centrale Operativa Traffico e Mobilità
è bidirezionale; il Centro Servizi Veicoli invia dati di traffico elaborati a partire dagli FCD (tempi di
viaggio sugli archi della cartografia/grafo di riferimento) mentre la Centrale Operativa Traffico e
Mobilità restituisce gli eventi e gli stati del traffico nonché le informazioni sulle ZTL.

E' disponibile il [documento di specifica](/simone-definizione_protocollo_comunicazione_400.pdf)  del protocollo.

Di seguito i files XSD che definiscono la sintassi del protocollo in XML Schema:
- [traffic_data.xsd](/ns/traffic_data.xsd)
- [traffic_info.xsd](/ns/traffic_info.xsd)
- [access_control.xsd](/ns/access_control.xsd)
