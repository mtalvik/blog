---
title: "Raalmõtlemine ja õppevara: loeng 01.11.2025"
date: 2025-11-16 16:25:29 +0200
course: "Informaatika didaktika"
tags: []
---

<p>Didaktika loeng informaatika õppevara loomisest ja kasutamisest. Teema oli lai: kuidas õppevara leida, kohandada, ise luua, kuidas hindamist korraldada ja diferentseeritud õpet rakendada. Aga kõige rohkem jäi meelde see, kuidas raalmõtlemist õpetada ilma et õpilased kohe arvuti taha istuksid.</p>

<h2>Unplugged kaartidega</h2>

<p>Näidati kuidas sorteerimist õpetada kaartidega. Väga lihtne idee. Mõni õpilane saab kaks-kolm kaarti ja peab need järjestama. See on QuickSort põhimõte. Teine õpilane saab neli või rohkem kaarti ja peab läbi mõtlema keerulisema kombinatsiooni. See on juba MergeSort suunas.</p>

<p>Oluline on see, et mõlemad õpivad sama asja - sorteerimist ja algoritmilist mõtlemist. Aga igaüks oma tasemel. See on diferentseerimine praktikas, mitte lihtsalt teooria.</p>

<h2>Google tööriistad õpetamiseks</h2>

<figure class="wp-block-image size-large is-resized"><img src="{{ '/assets/uploads/2025/11/screenshot-2025-11-16-at-16.08.01.png' | relative_url }}" alt="" class="wp-image-325" style="aspect-ratio:1.7487744113155992;width:435px;height:auto" /></figure>

<p>Loengul tutvustati mitmeid tööriistu mis on tasuta ja kohe kasutatavad. Teachable Machine (<a href="https://teachablemachine.withgoogle.com/">https://teachablemachine.withgoogle.com/</a>) kus saab treneerida masinõppe mudelit piltide, helide või poosidega. Ilma programmeerimiseta, lihtsalt näitad näiteid ja mudel õpib. Soomes kasutatakse seda edukalt.</p>

<p>Google Experiments'i Sound Teddy (<a href="https://experiments.withgoogle.com/sound-teddy">https://experiments.withgoogle.com/sound-teddy</a>) mis reageerib helile. Moebio (<a href="https://moebio.com">https://moebio.com</a>/) andmete visualiseerimiseks. Kõik need on tasuta, ei vaja keerulist registreerimist ega makseid.</p>

<figure class="wp-block-image size-large is-resized"><img src="{{ '/assets/uploads/2025/11/screenshot-2025-11-16-at-16.18.11.png' | relative_url }}" alt="" class="wp-image-327" style="aspect-ratio:1.9807027125432368;width:588px;height:auto" /></figure>

<p>See on oluline, sest sageli jääb mõni hea idee kasutamata kui see maksab või on keeruline kasutusele võtta.</p>

<h2>Kodutöö: digiõppevara ja hindamisvahend</h2>

<p>Selle nädala ülesanne oli lisada ühele tunnikavale digitaalne interaktiivne õppematerjal ja teisele hindamisvahend. Valisin nii, et Docker tunnikavale teen digiõppevara ja CI/CD tunnikavale hindamisvahendi.</p>

<h3>Docker digiõppevara</h3>

<p>Koostasin kolm interaktiivset materjali.</p>

<p>Esimene on Google Forms quiz kümne küsimusega Docker põhimõtete kohta. Link on <a href="https://docs.google.com/forms/d/e/1FAIpQLSdzu28vxMQHzW_qcUxXDe5nNmrRfs0OWg2_n3LNZMR4puxkNA/viewform">https://docs.google.com/forms/d/e/1FAIpQLSdzu28vxMQHzW_qcUxXDe5nNmrRfs0OWg2_n3LNZMR4puxkNA/viewform</a> ja seal on küsimused nagu mis on container, kuidas image erineb containerist, milleks on Dockerfile. Forms annab automaatselt hindeid ja õpilane näeb kohe tulemust.</p>

<p>Teine on ekraanivideo umbes 10 minutit kus ma näitan samm-sammult kuidas Dockerfile'i luua, kuidas image'i buildida ja kuidas konteinerit käivitada. See on integreeritud labor.md faili (<a href="https://mtalvik.github.io/automatiseerimine_ext/docker_basics/labor/">https://mtalvik.github.io/automatiseerimine_ext/docker_basics/labor/</a>) nii et õpilased saavad vaadata oma tempos, pausida, tagasi kerida.</p>

<p>Kolmas on GitHub harjutused kus on kuus praktilist ülesannet. Igaühe juures on TODO list. Õpilased forgivad repo, teevad oma lahendused, avanevad pull requesti ja saavad peer review. See on interaktiivne - nad ei loe lihtsalt teksti vaid teevad ja saavad tagasisidet.</p>

<h3>CI/CD hindamisvahend</h3>

<p>CI/CD tunnikavale koostasin hindamisrubriigi. See on 32-punktiline süsteem kaheksa kriteeriumiga. Iga kriteerium annab 1-4 punkti.</p>

<p>Kriteeriumid on pipeline struktuur (kas on kõik neli stage'i), YAML süntaks (kas töötab), vigade parandamine (labor'is on tahtlikult vead sees), Docker integratsioon, testimine, dokumentatsioon, manual approval ja väljakutsete lahendamine.</p>

<figure class="wp-block-image size-large"><img src="{{ '/assets/uploads/2025/11/screenshot-2025-11-16-at-16.21.53.png' | relative_url }}" alt="" class="wp-image-329" /></figure>

<p>Oluline on see, et labor'is on tahtlikult vead. Syntax error kus puudub koolon, negatiivne hind, vale port Dockerfile'is. Õpilased peavad need leidma ja parandama. See õpetab logide lugemist ja debugimist palju paremini kui töötav kood algusest.</p>

<p>Plus on kontrollnimekiri: kas&nbsp;<code>.github/workflows/ci.yml</code>&nbsp;fail on olemas, kas pipeline käivitub automaatselt, kas kõik stage'id töötavad, kas tahtlikud vead on parandatud.</p>

<h3>Mentimeter quiz</h3>

<p>Lisaks tegin CI/CD tunni alguseks Mentimeter quiz'i (<a href="https://www.menti.com/al8bv5nycvr4">https://www.menti.com/al8bv5nycvr4</a>). Seal on kaks osa.</p>

<p>Esimene osa on soojendus kolme küsimusega: kuidas sa end tunned, mida mäletad eelmisest tunnist, mis sind täna huvitab. See on warm-up et saada õpilased rääkima.</p>

<p>Teine osa on viktoriiniline võistlus viie küsimusega. Igal küsimusel on ajavahemik (20 või 30 sekundit) ja punktid (1-3 sõltuvalt raskusest). Kokku saab võita 9 punkti ja Mentimeter näitab edetabelit. See on põnevam kui küsida "kas te lugesite materjali?"</p>

<h2>Kuidas see kokku sobib</h2>

<p>Loengul räägiti diferentseerimisest läbi erineva tasemega ülesannete. Mu tunnikavades on starter template'id tugõppijatele ja lisaväljakutsed andekamatele.</p>

<p>Loengul näidati Google tööriistu. Mina kasutan GitHub Actions'it ja Docker'it mis annavad kohest tagasisidet. Pipeline kas töötab või ei tööta. Container kas käivitub või ei käivitu. Õpilane näeb ise kohe.</p>

<p>Loengul räägiti unplugged meetoditest. Mu Docker tunnis on Docker Hub'i uurimine enne kodeerimist. See on unplugged element - vaata mis teised on teinud, mõista struktuuri, alles siis hakka ise kirjutama.</p>

<p>Ja see tahtlike vigade asi. See tundub esialgu veider aga on õpetuslik. Kui õpilane saab kohe töötava koodi, ta kopeerib selle ja ei mõtle. Kui on viga sees, ta peab logisid lugema, debugima, mõtlema. See on päris oskus mida tal vaja läheb.</p>

<p>Rubriik annab struktuuri hindamisele. Ei ole enam "kolm sest tundub kolme väärt". On täpsed kriteeriumid ja punktid. Õpilane teab mida oodatakse ja õpetaja teab kuidas hinnata.</p>

<hr class="wp-block-separator has-alpha-channel-opacity" />

<p><strong>Viited:</strong></p>

<p>Minu materjalid:</p>

<ul class="wp-block-list">
<li>CI/CD loeng: <a href="https://mtalvik.github.io/automatiseerimine_ext/ci_cd/loeng/">https://mtalvik.github.io/automatiseerimine_ext/ci_cd/loeng/</a></li>

<li>CI/CD labor: <a href="https://mtalvik.github.io/automatiseerimine_ext/ci_cd/labor/">https://mtalvik.github.io/automatiseerimine_ext/ci_cd/labor/</a></li>

<li>Docker labor: https://mtalvik.github.io/automatiseerimine_ext/docker_basics/labor/</li>

<li>Mentimeter quiz: https://www.menti.com/al8bv5nycvr4</li>

<li>Docker quiz: https://docs.google.com/forms/d/e/1FAIpQLSdzu28vxMQHzW_qcUxXDe5nNmrRfs0OWg2_n3LNZMR4puxkNA/viewform</li>

<li></li>
</ul>

<p></p>
