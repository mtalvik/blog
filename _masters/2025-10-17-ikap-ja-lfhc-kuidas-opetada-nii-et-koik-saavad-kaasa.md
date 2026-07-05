---
title: "IKAP ja LFHC: Kuidas õpetada nii, et kõik saavad kaasa"
date: 2025-10-17 19:38:42 +0200
course: "Õppija ja õppimise mõistmine"
tags: []
---

<p><a href="https://moodle.tlu.ee/course/section.php?id=65006">11.oktoober loen "Tähelepanu ja mõtlemise kaasamine</a>", õppisime kolm asja: kognitiivne kaasatus (IKAP), tähelepanu ja "madal lävi - kõrge lagi" (LFHC) meetod. </p>

<h2>Probleem, mida kõik tunneme</h2>

<p>Oled kindlasti samas olukorras olnud: pead õpetama midagi uut. Osa inimesi ei tea põhitõdesid. Teised on juba kaugel ees ja igavlevad.</p>

<p>Õpetaja probleem, et ei jõua kõiki aidata. Algajad jäävad kinni. Edasijõudnud istuvad ja ootavad.</p>

<h2>IKAP: Kui sügavalt sa mõtled?</h2>

<p>IKAP näitab 4 taset, kuidas inimesed infot töötlevad:</p>

<figure class="wp-block-table"><table class="has-fixed-layout"><thead><tr><th>Tase</th><th>Mis toimub</th><th>Näide workflow/monitoring'ust</th></tr></thead><tbody><tr><td><strong>Passiivne</strong></td><td>Kuulad/vaatad</td><td>Vaatan Grafana demo't</td></tr><tr><td><strong>Aktiivne</strong></td><td>Teed midagi, aga ei mõtle</td><td>Kopeerin YAML'i</td></tr><tr><td><strong>Konstruktiivne</strong></td><td>Mõistad seoseid, teed "enda omaks"</td><td>"Saan are, miks siin <code>needs: [build]</code>"</td></tr><tr><td><strong>Interaktiivne</strong></td><td>Arutlete, ehitate koos</td><td>"Kas peaks cron või event trigger?"</td></tr></tbody></table></figure>

<p><strong>Võtmekoht:</strong> Mida sügavam (P→A→K→I), seda paremini meelde jääb. Copy-paste ei õpeta. Arusaamine õpetab.</p>

<h2>Tähelepanu: Värav teadmisteni</h2>

<p>Tähelepanu on justkui värav -&nbsp;<strong>ainult see, mis läbi pääseb, võib teadmiseks saada</strong>.</p>

<h3>Kaks tüüpi</h3>

<p><strong>Tahtlik tähelepanu</strong>&nbsp;- keskendud sihilikult (nt loed dokumentatsiooni)<br><strong>Tahtmatu tähelepanu</strong>&nbsp;- liigub automaatselt (nt Slacki notification)</p>

<h3>Miks see oluline?</h3>

<p>Tähelepanul on omadused:</p>

<ul class="wp-block-list">
<li><strong>Valivus</strong> - fokusseerid õigele asjale (mitte kõrvalistele)</li>

<li><strong>Püsivus</strong> - hoiad fookust (mitte 30 sekundit, vaid 10+ minutit)</li>

<li><strong>Ümberlülitus</strong> - vahetad tegevusi (nt kuulad + teed märkmeid)</li>
</ul>

<p><strong>Kuidas toetada:</strong></p>

<ul class="wp-block-list">
<li>Aktiveeri eelteadmisi: "Mida teate CI/CD-st?"</li>

<li>Loo turvaline keskkond (ärevus hajutab tähelepanu)</li>

<li>Visualiseeri (graafik &gt; tekst)</li>
</ul>

<h2>LFHC: Üks ülesanne, kõik kaasatud</h2>

<p>"Madal lävi – kõrge lagi" (Low Floor High Ceiling) tähendab:</p>

<ul class="wp-block-list">
<li><strong>Madal lävi</strong> = igaüks saab alustada</li>

<li><strong>Kõrge lagi</strong> = võid süveneda lõputult</li>
</ul>

<p><strong>Pole</strong>&nbsp;"lihtne" ja "raske" ülesanne. On&nbsp;<strong>üks ülesanne</strong>&nbsp;mitme kihiga.</p>

<h3>Ajalugu</h3>

<p><strong>1970ndad:</strong>&nbsp;MIT professor Seymour Papert lõi mõiste "madal lävi, kõrge lagi" programmeerimiskeele Logo jaoks. Ta tahtis, et lapsed saaksid kergesti alustada, aga täiskasvanud saaksid teha keerukaid asju sama keelega.</p>

<p><strong>2013:</strong>&nbsp;Suurbritannia Cambridge'i ülikooli matemaatika keskus NRICH hakkas seda meetodit kasutama matemaatika õpetamiseks.</p>

<p><strong>2014:</strong>&nbsp;USA matemaatikaõpetajate organisatsioon (NCTM) soovitas seda ametlikult kasutada.</p>

<p><strong>Praegu:</strong>&nbsp;Meetod on levinud - kasutan seda workflow automation'i ja monitoring'u õpetamiseks.</p>

<h2>Praktiline näide: GitHub Actions workflow</h2>

<p>Üks ülesanne, mis töötab kõikide jaoks:</p>

<p><strong>Põhiülesanne:</strong>&nbsp;"Seadista CI workflow"</p>

<h3>Madal lävi (sammud 1-5)</h3>

<figure class="wp-block-table"><table class="has-fixed-layout"><thead><tr><th>#</th><th>Ülesanne</th></tr></thead><tbody><tr><td>1</td><td>Mis on GitHub Actions?</td></tr><tr><td>2</td><td>Fork'i see repo</td></tr><tr><td>3</td><td>Vaata&nbsp;<code>.github/workflows/ci.yml</code>&nbsp;- mis seal toimub?</td></tr><tr><td>4</td><td>Tee commit, vaata Actions tab'i</td></tr><tr><td>5</td><td>Lisa oma nimi:&nbsp;<code>echo "Hello ${{ github.actor }}"</code></td></tr></tbody></table></figure>

<h3>Kõrge lagi (sammud 6-12)</h3>

<figure class="wp-block-table"><table class="has-fixed-layout"><thead><tr><th>#</th><th>Ülesanne</th></tr></thead><tbody><tr><td>6</td><td>Lisa teine job:&nbsp;<code>test</code></td></tr><tr><td>7</td><td>Tee job'id paralleelseks, siis järjestikuseks (<code>needs:</code>)</td></tr><tr><td>8</td><td>Matrix strategy: testi Python 3.9, 3.10, 3.11</td></tr><tr><td>9</td><td>Lisa secrets. Mis juhtub, kui paned tokeni YAML'i?</td></tr><tr><td>10</td><td>Cache dependencies. Mõõda aega enne/pärast</td></tr><tr><td>11</td><td>Deployment workflow testide järel</td></tr><tr><td>12</td><td>Võrdle: GitHub Actions vs Jenkins vs GitLab CI</td></tr></tbody></table></figure>

<h2>Miks see töötab?</h2>

<p><strong>Võrdsus:</strong>&nbsp;Kõik saavad alustada → vähem ärevust → parem tähelepanu</p>

<p><strong>Kasvumõtteviis:</strong>&nbsp;Igaüks võib areneda pingutades</p>

<p><strong>Sügav mõistmine:</strong>&nbsp;Pole copy-paste, vaid konstruktiivne kaasatus (IKAP!)</p>

<p><strong>Loomulik diferentseerimine:</strong>&nbsp;Üks ülesanne, erinevad sügavused</p>

<h2>Praktiline nõuanne</h2>

<ul class="wp-block-list">
<li><strong>Ära tee kõiki ülesandeid ümber.</strong> Piisab 1-2 LFHC ülesandest teema kohta.</li>

<li><strong>Koostöö:</strong> Jaga kolleegidega, vähenda töökoormust</li>

<li><strong>ChatGPT/Gemini:</strong> Võivad aidata LFHC ülesandeid luua (anna head näited sisendiks)</li>
</ul>

<h2>Kokkuvõte</h2>

<p><strong>IKAP</strong>&nbsp;näitab, et sügav kaasatus (konstruktiivne/interaktiivne) = parem õppimine</p>

<p><strong>Tähelepanu</strong>&nbsp;on värav - peab olema tahtlik, valivus + püsivus + ümberlülitus</p>

<p><strong>LFHC</strong>&nbsp;= üks ülesanne, madal lävi (kõik alustavad) + kõrge lagi (lõputu süvenemine)</p>

<p><strong>Tulemus:</strong>&nbsp;Ei ole enam "mõni ei saa alustada, teine igavleb" probleem.</p>

<p></p>
