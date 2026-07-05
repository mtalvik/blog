---
title: "Kodutööd 3 ja 4: LePlanner Tunnikavad ja Digiõppevara"
date: 2025-10-12 23:55:33 +0200
course: "Informaatika didaktika"
tags: []
---

<p>Kodutööks oli vaja koostada kolm tunnikava informaatika ainekava juurde, kasutades LePlanner.ee platvormil. Iga tund peab demonstreerima erinevat didaktilist lähenemist ja vastama õppekava õpiväljunditele.</p>

<h3>Tunnikavad</h3>

<figure class="wp-block-table"><table class="has-fixed-layout"><thead><tr><th>#</th><th>Tund</th><th>Link</th><th>Kestus</th><th>Õpiväljund</th><th>Didaktiline lähenemine</th></tr></thead><tbody><tr><td>1</td><td>Docker konteinerite loomine</td><td><a href="https://leplanner.ee/en/scenario/5442">LePlanner 5442</a></td><td>90 min</td><td>ÕV2 - Oskab luua ja seadistada konteinereid</td><td>Avastusõpe + hands-on</td></tr><tr><td>2</td><td>Ansible automatiseerimine</td><td><a href="https://leplanner.ee/en/scenario/5443">LePlanner 5443</a></td><td>90 min</td><td>ÕV3, ÕV4 - Ansible PlayBook ja automatiseerimine</td><td>Probleemipõhine õpe + rühmatöö</td></tr><tr><td>3</td><td>CI/CD pipeline GitLabis</td><td><a href="https://leplanner.ee/en/scenario/5444">LePlanner 5444</a></td><td>90 min</td><td>ÕV7 - CI/CD automatiseerimine</td><td>Ümberpööratud klassiruum</td></tr></tbody></table></figure>

<h3>Didaktilised Lahendused</h3>

<p>Iga tunnikava kasutab erinevat didaktilist lähenemist:</p>

<ul class="wp-block-list">
<li><strong>Avastusõpe</strong>&nbsp;võimaldab õppijatel iseseisvalt uurida ja järeldusi teha (Docker Hub uurimine)</li>

<li><strong>Probleemipõhine õpe</strong>&nbsp;lähtub autentsest probleemist, mida rühmas lahendatakse (10 serveri seadistamine)</li>

<li><strong>Ümberpööratud klassiruum</strong>&nbsp;nihutab teoreetilise materjali koduseks õppeks, jättes tunni praktilisele rakendamisele (CI/CD video kodus, praktiline töö tunnis)</li>
</ul>

<h4>Võrdlustabel</h4>

<figure class="wp-block-table"><table class="has-fixed-layout"><thead><tr><th>Aspekt</th><th>Tund 1: Docker</th><th>Tund 2: Ansible</th><th>Tund 3: CI/CD</th></tr></thead><tbody><tr><td><strong>Lähenemine</strong></td><td>Avastusõpe</td><td>Probleemipõhine</td><td>Ümberpööratud klassiruum</td></tr><tr><td><strong>Töövorm</strong></td><td>Individual + Pair</td><td>Small group</td><td>Pair</td></tr><tr><td><strong>Algus</strong></td><td>Õpilased uurivad ise</td><td>Probleem esitatakse</td><td>Kodutöö kontroll</td></tr><tr><td><strong>Protsess</strong></td><td>Avastamine → harjutused</td><td>Planeerimine → rühmatöö → peer review</td><td>Demo → hands-on → debugging</td></tr><tr><td><strong>Lõpp</strong></td><td>Exit ticket (Menti)</td><td>Reflektsioon (Padlet)</td><td>Demo esitlused + vorm</td></tr><tr><td><strong>Õppematerjalid</strong></td><td>Cheat sheets, juhendid</td><td>Projektibriif, näidised, dokumentatsioon</td><td>Video (kodus), templates, docs</td></tr></tbody></table></figure>

<h3>Merrilli Põhiprintsiibid Tunnikavades</h3>

<p>Merrilli First Principles of Instruction (2002) väidab, et efektiivne õpe toimub läbi viie põhiprintsiibi:</p>

<ol class="wp-block-list">
<li><strong>Problem-centered</strong>&nbsp;- õppijad lahendavad autentseid probleeme</li>

<li><strong>Activation</strong>&nbsp;- aktiveerivad varasemaid teadmisi</li>

<li><strong>Demonstration</strong>&nbsp;- näevad oskuse demonstreerimist</li>

<li><strong>Application</strong>&nbsp;- rakendavad seda praktikas</li>

<li><strong>Integration</strong>&nbsp;- integreerivad uued oskused läbi refleksiooni</li>
</ol>

<p>Tunnikavades tagasin, et iga tund sisaldab kõiki viit printsiipi:</p>

<figure class="wp-block-table"><table class="has-fixed-layout"><thead><tr><th>Printsiip</th><th>Tund 1</th><th>Tund 2</th><th>Tund 3</th></tr></thead><tbody><tr><td><strong>Problem-centered</strong></td><td>Praktiline Dockerfile ülesanne</td><td>10 serveri stsenaarium</td><td>Pipeline loomine</td></tr><tr><td><strong>Activation</strong></td><td>Docker Hub uurimine</td><td>Ansible aluste kordamine</td><td>Kodutöö + video</td></tr><tr><td><strong>Demonstration</strong></td><td>Dockerfile demo</td><td>Manuaalne vs auto võrdlus</td><td>Live pipeline demo</td></tr><tr><td><strong>Application</strong></td><td>Hands-on harjutused</td><td>Rühmatöö + testimine</td><td>Hands-on + debugging</td></tr><tr><td><strong>Integration</strong></td><td>Kokkuvõte + reflektsioon</td><td>Peer review + exit ticket</td><td>Demo + refleksiooni vorm</td></tr></tbody></table></figure>

<p>Kodutöös oli vaja teha kolme tüüpi digiõppevara loomist Docker põhimõtete mooduli jaoks:</p>

<ol class="wp-block-list">
<li>H5P interaktiivsed enesekontrolli küsimused</li>

<li>Ekraanivideo (10-15 min)</li>

<li>Töölehted</li>
</ol>

<h3>1. Interaktiivne Quiz (Google Forms)</h3>

<p>Kuna H5P Lumi Desktop eksportimine osutus aeglaseks, valisin alternatiivse lahenduse - Google Forms quiz'i.</p>

<ul class="wp-block-list">
<li><strong>Küsimuste arv:</strong>&nbsp;10 multiple choice</li>

<li><strong>Teemad:</strong>&nbsp;Container vs VM, docker build/run, Dockerfile süntaks, image vs container</li>

<li><strong>Hindamine:</strong>&nbsp;Automaatne</li>

<li><strong>Tulemused:</strong>&nbsp;Salvestatud Google Sheets'is</li>
</ul>

<p><strong>Integratsioon MkDocs'iga:</strong></p>

<pre class="wp-block-syntaxhighlighter-code">**[➡️ Ava Docker Quiz](https://docs.google.com/forms/d/e/.../viewform)**

!!! info "Quiz sisaldab"
    - 10 multiple choice küsimust
    - Automaatne hindamine
    - Kohese tagasiside
    - Aeg: ~5-10 minutit
</pre>

<p><strong>Asukoht:</strong>&nbsp;<code>docs/docker_basics/loeng.md</code>&nbsp;(lõpus, pärast teoreetilist materjali)</p>

<h3>2. Ekraanivideo - Docker Praktiline Demo</h3>

<ul class="wp-block-list">
<li><strong>Kestus:</strong>&nbsp;10 minutit</li>

<li><strong>Formaat:</strong>&nbsp;MP4, embedded otse MkDocs'iga</li>

<li><strong>Sisu:</strong>&nbsp;Dockerfile loomine → build → run → testimine</li>

<li><strong>Stiil:</strong>&nbsp;Screen recording ilma hääletä, TODO checklist ekraanil</li>
</ul>

<p><strong>Integratsioon MkDocs'iga:</strong></p>

<pre class="wp-block-syntaxhighlighter-code">&lt;video width="100%" controls&gt;
  &lt;source src="videos/docker-demo.mp4" type="video/mp4"&gt;
&lt;/video&gt;
</pre>

<p><strong>Asukoht:</strong>&nbsp;<code>docs/docker_basics/labor.md</code>&nbsp;(alguses, enne praktiliste harjutuste alustamist)</p>

<h3>3. Töölehted</h3>

<p>Töölehted on juba olemas&nbsp;<code>labor.md</code>&nbsp;ja&nbsp;<code>kodutoo.md</code>&nbsp;failides.</p>

<h3>Järeldused</h3>

<p>Mõlemad kodutööd tehtud arvestades:</p>

<ol class="wp-block-list">
<li><strong>Mitmekesised õppemeetodid</strong>&nbsp;- avastusõpe, probleemipõhine õpe, ümberpööratud klassiruum</li>

<li><strong>Digitaalsed tööriistad</strong>&nbsp;- LePlanner tunnikavadele, Google Forms quiz'ile, video embedded MkDocs'iga</li>

<li><strong>Praktilisus</strong>&nbsp;- iga tund ja iga õppematerjal on rakendatav reaalses klassiruumis</li>

<li><strong>Refleksioon</strong>&nbsp;- Merrilli Integration printsiip tagatud kõikides materjalides</li>
</ol>

<p>Materjalid on kättesaadavad GitHubis ja MkDocs'i lehel, võimaldades teistel õpetajatel neid kasutada ja kohandada.</p>

<hr class="wp-block-separator has-alpha-channel-opacity" />

<p><strong>Allikad:</strong></p>

<ul class="wp-block-list">
<li>Merrill, M. D. (2002). First principles of instruction. Educational Technology Research and Development, 50(3), 43-59.</li>

<li>LePlanner.ee platvorm: https://leplanner.ee</li>

<li>Projekti repository: https://github.com/mtalvik/automatiseerimine_ext ja site: <a href="https://mtalvik.github.io/automatiseerimine_ext/">https://mtalvik.github.io/automatiseerimine_ext/</a></li>
</ul>

<p></p>
