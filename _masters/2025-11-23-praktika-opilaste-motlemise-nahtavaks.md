---
title: "Praktika: õpilaste mõtlemise nähtavaks"
date: 2025-11-23 23:09:07 +0200
course: "Informaatika alused"
tags: []
---

<p>Teema oli tehniliselt keeruline - IPv4 aadresside jaotamine, maskid, valemid. Lisaks teadsin ma oma klassi: nad ei räägi meeleldi kogu klassi ees. Seega Think-Pair-Share? Ei tööta. Klassikaline arutelu? Unusta ära. Ma vajasin meetodeid, kus&nbsp;<strong>igaüks saab osaleda ilma hirmuta</strong>.</p>

<p>Kasutasin nelja erinevat meetodit läbi 92-minutilise tunni:</p>

<figure class="wp-block-image size-large"><img src="{{ '/assets/uploads/2025/11/screenshot-2025-11-23-at-22.47.41.png' | relative_url }}" alt="" class="wp-image-334" /></figure>

<p>Tahvlitöö oli huvitav, nägin kuidas nad mõtlevad. Üks õpilane kirjutas kohe .255 broadcast'iks. Teine mõtles, vaatas, siis parandas . Ma ei vastanud, küsisin tagasi: "Mida sa arvad?".</p>

<p>Gruppipiga plaaneerisime diferentseeritud hindamise : TASE 1 (lihtsam): Ainult /24 mask, põhikontseptsioonid, 17 punkti<br>Hiljem ma lisasin igaks juhuks ka TASE 2 (keerulisem): Erinevad maskid (/25, /26, /27), binary, 22 punkti. Kes lõpetab kiiresti ja saab hästi, võtab TASE 2. Kes vajab rohkem aega, jääb TASE 1 juurde.</p>

<p><strong>TASE 1 küsimused - Yip'i tüpoloogia</strong></p>

<p>Kasutasime Yip'i (2004) küsimuste tüpoloogiat. Yip keskendub kontseptuaalse muutuse toetamisele.  Siin on meie 6 küsimust:</p>

<figure class="wp-block-image size-large"><img src="{{ '/assets/uploads/2025/11/screenshot-2025-11-23-at-22.53.33-1.png' | relative_url }}" alt="" class="wp-image-339" /></figure>

<p>Valise, et küsimused läheksid lihtsamast (K1) → keerulisemani (K6). See on oluline,  sest kui õpilane saab K1 ja K2 õigesti, aga K5 ja K6 vales, siis ma tean: ta mäletab fakte, aga ei oska veel <strong>kriitiliselt mõelda</strong> või <strong>strateegiliselt planeerida</strong>. <br><br>Saime keskmiselt  81%, mis on väga hea resultaat esimese testi jaoks uue teemaga<br><strong>Keskmine:</strong> 13.75/17 (81%)<br><strong>Mediaan:</strong> 15.25/17 (90%)<br><strong>Täispunkte:</strong> 3 õpilast</p>

<p><strong>K5 (vale arusaama leidmine) oli paljastav.</strong> Parimad õpilased leidsid vea (256→254) ja selgitasid miks.  Nõrgemad kirjutasid ainult "Vale" ilma selgituseta. See näitas, kes mõistab sügavalt ja kes ainult mäletab.</p>

<p><strong>Üks õpilane sai 4.5/17.</strong>&nbsp;See tähendab, ta ei mõista network/host/broadcast erinevust. Valem ei ole meeles või ei oska rakendada. Ma pean temaga eraldi rääkima. Võimalik, et oli segaduses või ei kuulanud loengut? Või on teemaga täiesti kadunud? Pean järgmises tunnis aitama.</p>

<p><strong>Keskmine grupp (8.5-12.5 punkti) võitles kõrgemate kognitiivsete tasanditega.</strong> Nad said K1, K2, K3 peaaegu õigesti (meenutamine, analüüs, rakendamine). Aga K5 ja K6 (hindamine, laiendamine) olid keerulised. See on loomulik! Need küsimused nõuavad <strong>kõrgemat mõtlemist</strong>. Mitte ainult "arvuta", vaid "miks" ja "kuidas". See on täpselt see oskus, mida me peame arendama.</p>

<h3>Yip'i tüpoloogia töötas</h3>

<p>Küsimuste progressioon (meenutamine → analüüs → rakendamine → hindamine → laiendamine) näitas täpselt, "kes" on kus. Tugevad õpilased said kõik küsimused õigesti. Keskmised said põhiküsimused õigesti, aga kõrgemad mõtlemistasandid jäid poolikuks. Nõrk õpilane ei saanud isegi põhiküsimusi. Nüüd ma tean, kellele mida õpetada.</p>

<p>92 minutit tundus palju, aga läks kiiresti. Järgmine kord peab tahvlitöö olema 25 minutit, mitte 30. Või loeng lühem. Või TASE 2 on eraldi tunni ülesanne algselt. Ei näinud ühtegi kopeerimist, sest valmistasid 3 varianti. Õpilased istusid läbisegi (A-B-C-A-B-C), seega naaber oli alati teine variant. Nad pidid ise mõtlema. </p>

<h3>Nüüd ma tean, kes on kus, ja saan planeerida järgmise tunni.</h3>

<p><strong>15 min: Tagasiside</strong><br>Jagan testid tagasi<br>Läbi võtame TOP 3 viga: unustasid -2 valemis, broadcast vale, põhjendused puudusid<br>"Mis oli raske?" - arutelu</p>

<p><strong>60 min: Diferentseeritud töö (3 gruppi!)</strong><br>Grupp A (4 õpilast, 15-17 punkti): Need on valmis! Nad teevad TASE 2 testi.<br>Grupp B (3 õpilast, 8.5-12.5 punkti): Nad vajavad veel harjutusi "põhjendamise" osas. 20 min harjutused klassis (ma aitan), siis TASE 2 test.<br>Grupp C (1 õpilane, 4.5 punkti): Individuaalne abi minult 20 minutit. Selgitame põhikontseptsioone uuesti.</p>

<p><strong>15 min: Kokkuvõte</strong><br>Exit ticket Mentimeter<br>"Mis on selgem nüüd?"</p>

<p>See oli minu esimene kord luua diferentseeritud teste Yip'i tüpoloogia järgi. Ja ma olen rahul. Keskmine 81% on hea, 3 täispunkti on suurepärane, ja ma nägin täpselt, kes vajab abi. Diferentseerimine ei lõpe testiga. See jätkub järgmises tunnis, kus igaüks töötab oma tasemele sobival tasemel. Ja see on täpselt nii, nagu peaks olema.</p>

<p><strong>Kasutatud materjalid:</strong><br>Yip, D. Y. (2004). Questioning skills for conceptual change in science instruction.&nbsp;<em>Journal of Biological Education</em>, 38(2), 76-83.</p>
