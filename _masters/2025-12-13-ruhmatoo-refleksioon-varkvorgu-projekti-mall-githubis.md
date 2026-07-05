---
title: "Rühmatöö refleksioon: värkvõrgu projekti mall GitHubis"
date: 2025-12-13 20:09:24 +0200
course: "Informaatika didaktika"
tags: []
---

<p><strong>Repo:</strong>&nbsp;<a href="https://github.com/orgs/varkvork-projekt/">https://github.com/orgs/varkvork-projekt/</a></p>

<p>Rühmatöö ülesanne oli luua ainetevahelise digiloovtöö mall, mis seob informaatika vähemalt kahe teise õppeainega. Valisime IoT stendi teema, mis lõimib informaatikat füüsika ja inglise keelega. Lõime GitHubis keskkonna, mida õpilased saaksid kasutada oma digiloovtöö läbiviimiseks.</p>

<figure class="wp-block-image size-large"><img src="{{ '/assets/uploads/2025/12/screenshot-2025-12-13-at-19.38.11.png' | relative_url }}" alt="" class="wp-image-396" /></figure>

<h3>Repo struktuur</h3>

<p>Panime paika kaustade struktuuri: docs dokumentatsioonile, src koodile, schematics skeemidele. README hoidsime lühikese - badge'd näitavad staatust, lingid viivad Wiki'sse edasi.</p>

<p>Lõiming tuleb sisse läbi etappide - näiteks Etapp 4 (Disain) nõuab füüsika teadmisi skeemide koostamiseks, Etapp 6 (Dokumentatsioon) eeldab ingliskeelse tehnilise kirjelduse tegemist.</p>

<figure class="wp-block-image size-large is-resized"><img src="{{ '/assets/uploads/2025/12/screenshot-2025-12-13-at-19.41.30.png' | relative_url }}" alt="" class="wp-image-401" style="width:487px;height:auto" /></figure>

<h3>Projektõpe ja rollid</h3>

<p>Loengus rääkisime, kuidas tarkvaratiimid päriselt töötavad. Kohandasime seda IoT projekti jaoks ja panime paika kolm rolli:</p>

<ul class="wp-block-list">
<li><strong>Projektijuht / Analüütik</strong>&nbsp;- koordineerib tööd, suhtleb juhendajaga, uuendab Projects board'i</li>

<li><strong>Disainer</strong>&nbsp;- stendi väljanägemine, kasutajakogemus, fotod ja videod dokumenteerimiseks</li>

<li><strong>Riistvara / IoT integratsioon</strong>&nbsp;- seadmete valik, füüsiline ehitus, kood, testimine</li>
</ul>

<p>Wiki lehel on iga rolli kohta detailsed ülesanded ja vajalikud oskused. Lisasime ka paindlikkuse - väiksema meeskonna puhul võib üks liige võtta 2 rolli, rollid pole jäigad ja kõik aitavad kõiki.</p>

<figure class="wp-block-image size-large is-resized"><img src="{{ '/assets/uploads/2025/12/screenshot-2025-12-13-at-19.44.53.png' | relative_url }}" alt="" class="wp-image-404" style="aspect-ratio:1.539876866463803;width:574px;height:auto" /></figure>

<h3>GitHub Actions</h3>

<p>See oli meie lahenduse kõige huvitavam osa pedagoogilisest vaatepunktist. Tegime<strong> 8 workflow'd</strong>, mis töötavad ahelana - kui õpilane sulgeb ühe etapi Issue, tekib automaatselt järgmine. <strong>Automatiseerimine</strong> annab tellingud (scaffolding) - õpilane teab alati, mis on järgmine samm, aga peab ikkagi ise sisu tegema. See toetab ka <strong>raalmõtlemise komponente - dekompositsioon</strong> (projekt on jagatud 8 etapiks), algoritmid (kindel järjekord), abstraheerimine (iga etapp on üldistatud nii, et sobib erinevatele projektidele).</p>

<div class="wp-block-jetpack-tiled-gallery aligncenter is-style-rectangular"><div class=""><div class="tiled-gallery__gallery"><div class="tiled-gallery__row"><div class="tiled-gallery__col" style="flex-basis:100.00000%"><figure class="tiled-gallery__item"><img alt="" data-height="365" data-id="419" data-link="https://matalvik.wordpress.com/?attachment_id=419" data-url="https://matalvik.wordpress.com/wp-content/uploads/2025/12/screenshot-2025-12-13-at-19.46.36-2.png?w=1024" data-width="1235" src="{{ '/assets/uploads/2025/12/screenshot-2025-12-13-at-19.46.36-2.png' | relative_url }}" /></figure></div></div><div class="tiled-gallery__row"><div class="tiled-gallery__col" style="flex-basis:58.62411%"><figure class="tiled-gallery__item"><img alt="" data-height="492" data-id="418" data-link="https://matalvik.wordpress.com/?attachment_id=418" data-url="https://matalvik.wordpress.com/wp-content/uploads/2025/12/screenshot-2025-12-13-at-19.46.58-1.png?w=591" data-width="591" src="{{ '/assets/uploads/2025/12/screenshot-2025-12-13-at-19.46.58-1.png' | relative_url }}" /></figure></div><div class="tiled-gallery__col" style="flex-basis:41.37589%"><figure class="tiled-gallery__item"><img alt="" data-height="862" data-id="420" data-link="https://matalvik.wordpress.com/?attachment_id=420" data-url="https://matalvik.wordpress.com/wp-content/uploads/2025/12/screenshot-2025-12-13-at-19.47.13-4.png?w=730" data-width="730" src="{{ '/assets/uploads/2025/12/screenshot-2025-12-13-at-19.47.13-4.png' | relative_url }}" /></figure></div></div></div></div></div>

<p>Tegime Wiki lehele "Hindamine" punktisüsteemi.</p>

<figure class="wp-block-image size-large is-resized"><img src="{{ '/assets/uploads/2025/12/screenshot-2025-12-13-at-19.55.35.png' | relative_url }}" alt="" class="wp-image-425" style="aspect-ratio:0.9277537359568526;width:407px;height:auto" /></figure>

<p>Kokku 100 punkti. Õpilane näeb kohe, mille eest hindeid saab. Tehniline teostus on kõige suurema kaaluga, aga projektijuhtimine ja disain on ka olulised - see peegeldab päris tarkvaraarenduse väärtusi.</p>

<h2>Kanban ja töökorraldus</h2>

<p>Kasutasime GitHubi Projects board'i neljas tulbaga: Ootel, Töös, Ülevaatus, Tehtud.</p>

<figure class="wp-block-image size-large"><img src="{{ '/assets/uploads/2025/12/screenshot-2025-12-13-at-19.58.19.png' | relative_url }}" alt="" class="wp-image-427" /></figure>

<p>"Ülevaatus" tulp on teadlik valik - see simuleerib code review praktikat. Digiloovtöö õpiväljundites on kirjas, et õpilane "panustab meeskonnaliikmena" - see tähendab ka teiste töö ülevaatamist, mitte ainult oma osa tegemist.</p>

<h2>Discussions - kogukonna loomine</h2>

<p>Seadistasime neli kategooriat: Ideed, Küsimused, Näita tööd, Teated.</p>

<figure class="wp-block-image size-large"><img src="{{ '/assets/uploads/2025/12/screenshot-2025-12-13-at-19.59.09.png' | relative_url }}" alt="" class="wp-image-429" /></figure>

<p>See toetab suhtlus- ja koostööpädevust, mis on üks digipädevuse viiest valdkonnast. Õpilased harjuvad professionaalse suhtlusega - küsimused ühes kohas, mitte laiali e-mailides ja Messengeri gruppides.</p>

<h2>Digiloovtöö õpiväljundite täitmine</h2>

<p>Vaatasin üle RÕK digiloovtöö õpiväljundid ja kuidas meie mall neid toetab:</p>

<figure class="wp-block-image size-large"><img src="{{ '/assets/uploads/2025/12/screenshot-2025-12-13-at-20.00.09.png' | relative_url }}" alt="" class="wp-image-431" /></figure>

<p><strong>Seotud õppematerjalid:</strong></p>

<ul class="wp-block-list">
<li>Digiloovtöö õpik:&nbsp;<a href="https://web.htk.tlu.ee/informaatika/digiloovtoo/">https://web.htk.tlu.ee/informaatika/digiloovtoo/</a></li>

<li>DigiTaru: <a href="https://web.htk.tlu.ee/informaatika/digiloovtoo/chapter/digiloovtoo-konstseptsioon/">https://web.htk.tlu.ee/informaatika/digiloovtoo/chapter/digiloovtoo-konstseptsioon/</a></li>
</ul>

<p></p>
