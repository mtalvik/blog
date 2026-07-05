---
title: "GitHub kui Õpikeskkond: Automation Kursuse Kogemus"
date: 2025-10-02 18:22:22 +0200
course: "opikeskkonnad-ja-vorgustatud-ope"
tags: []
---

<h2>Miks ma ei valinud Moodle't?</h2>

<p>Olen insener ja õpetan automatiseerimist. Kui tuli aeg valida õpikeskkonda, teadsin kohe - Moodle või Canvas ei sobi. Liiga palju klikkimist, liiga vähe kontrolli, liiga kaugel päris tööst.</p>

<p>Kui õpilased peavad nagunii Git'i, Docker'i ja CI/CD'd õppima, miks mitte kasutada GitHubi ka õpikeskkonnana? See pole mitte ainult tööriist, vaid osa õppimisest.</p>

<h2>Kuidas see välja näeb?</h2>

<p>Kursuse materjalid hoian enda repos ja avaldan MkDocs'iga: </p>

<p><a href="https://mtalvik.github.io/automation/ansible_basics/lecture/">https://mtalvik.github.io/automation/ansible_basics/lecture/</a></p>

<p>Kirjutan Markdown'is, push'in, GitHub Actions build'ib automaatselt ja deploy'b GitHub Pages'i. Leian vea kell 21:00? Edit → commit → 2 minutit hiljem on parandus live. Õpilane, kes alustab kell 21:15, näeb juba õiget versiooni.</p>

<figure class="wp-block-image size-large"><img src="{{ '/assets/uploads/2025/10/screenshot-2025-10-02-at-18.15.40.png' | relative_url }}" alt="" class="wp-image-133" /></figure>

<p>Õpilaste töö toimub kooli organisatsiooni repos: </p>

<p><a href="https://github.com/Haapsalu-Kutsehariduskeskus/automatiseerimine-2025">https://github.com/Haapsalu-Kutsehariduskeskus/automatiseerimine-2025</a></p>

<p>Seal nad fork'ivad, loovad oma kausta ja teevad labisid. Eraldus on selge - minu materjalid ühes kohas, nende töö teises.</p>

<h2>Ülesannete esitamine</h2>

<p>Mitte ZIP failid - GitHub Issues. Õpilane loob Issue template'i järgi:</p>

<figure class="wp-block-image size-large is-resized"><img src="{{ '/assets/uploads/2025/10/screenshot-2025-10-02-at-18.00.29.png' | relative_url }}" alt="" class="wp-image-121" style="aspect-ratio:1.512581676630057;width:493px;height:auto" /></figure>

<p>Template sisaldab checklist'i (kas kõik töötab?), linki lahendusele, screenshot'i ja refleksiooni.</p>

<p>Kui õpilane submittib Issue, käivitub GitHub Actions automaatselt:</p>

<figure class="wp-block-image size-large is-resized"><img src="{{ '/assets/uploads/2025/10/screenshot-2025-10-02-at-18.02.02.png' | relative_url }}" alt="" class="wp-image-122" style="aspect-ratio:1.7029935433378987;width:526px;height:auto" /></figure>

<p>Actions testib: kas Docker konteinerid käivituvad? Kas API vastab? Kas andmed püsivad restart'i järel?</p>

<p>20 õpilast × 5 labidat = varem 50 tundi käsitööd. Nüüd? Actions teeb ära. Ma vaatan koodi kvaliteeti, mitte kas Docker üles käib.</p>

<h2>GitHub Education - tasuta asjad</h2>

<p>GitHub Education oli üks peamisi põhjuseid selle valiku taga - nii mina kui õpilased saame ligipääsu professionaalsetele tööriistadele täiesti tasuta. </p>

<p>Õpetajana saan unlimited GitHub Actions minutes'id (mis võimaldab labisid automaatselt testida), Copilot'i ja Codespaces'i, samas kui õpilased saavad Student Developer Pack'i kaudu Copilot'i, JetBrains IDE'd, cloud credits'id ja üle 50 muu tööriista. </p>

<p>See on sadu eurosid väärtuses ressursse, mis muidu oleksid kättesaamatud - piisab vaid kooli emaili aadressist registreerumiseks.</p>

<figure class="wp-block-image size-large is-resized"><img src="{{ '/assets/uploads/2025/10/screenshot-2025-10-02-at-18.04.39.png' | relative_url }}" alt="" class="wp-image-125" style="aspect-ratio:1.9926739926739927;width:509px;height:auto" /></figure>

<h2>Copilot tuleb mängu</h2>

<p>Copilot on nüüd GitHub Education kaudu tasuta ja kuigi pole veel jõudnud kõiki võimalusi katsetada, plaanin seda aktiivselt kasutada mitmel viisil. </p>

<p>Mõtlen panna Copilot Workspace'i õpilaste käsutusse, et nad õpiksid AI-assisted development't päris workflow'ga, samuti kasutada Copilot'i code review'de kiirendamiseks ja CLI'd terminalis. </p>

<p>Eesmärk pole AI'ga laisklema, vaid õpetada kuidas insenerid 2025. aastal päriselt töötavad - koos AI'ga.</p>

<h2>Project Board</h2>

<p>Project Board annab kanban-stiilis ülevaate kõigist esitustest, kus Issues liiguvad automaatselt Todo → In Progress → Done. </p>

<figure class="wp-block-image size-large"><img src="{{ '/assets/uploads/2025/10/screenshot-2025-10-02-at-18.08.10.png' | relative_url }}" alt="" class="wp-image-129" /></figure>

<p>Mulle kui insenerile meeldib täielik kontroll ja kiire Markdown + Git workflow, kus Actions automatiseerivad igava töö ja kõik on tekstipõhiselt version control'is. </p>

<p>Õpilased saavad päris tööriistadega kogemuse, kohese feedback'i ja nende GitHub profile täitub projektidega, samas kui automation kursus ise kasutab automation'i - CI/CD pole slides'id vaid reaalne pipeline.</p>

<h2>Discussions</h2>

<p>GitHub Discussions toimib kui kursuse foorum, kus õpilased saavad esitada küsimusi, jagada lahendusi ja anda peer feedback'i - kõik seotud sama repository'ga, kus code snippet'id ja linkid töötavad automaatselt.</p>

<figure class="wp-block-image size-large is-resized"><img src="{{ '/assets/uploads/2025/10/screenshot-2025-10-02-at-18.20.20.png' | relative_url }}" alt="" class="wp-image-136" style="aspect-ratio:1.876428232656405;width:501px;height:auto" /></figure>

<h2>Mis on ebamugav?</h2>

<p>Õpilastele on esimesed paar nädalat rasked - Git, GitHub, Markdown ja terminal on kõik uus korraga, ning kes pole varem GitHubi näinud, peavad palju õppima enne kui päris tööle saavad hakata. </p>

<p>Seadistamine nõuab aega, eriti Actions workflow'de kirjutamine, ning pead ise kõik üles ehitama.</p>

<h2>Kas soovitan?</h2>

<p>Soovitan GitHubi õpikeskkonnana jah, kui õpetad tehnilist ainet (coding, DevOps, automation), oled ise tehniline inimene ja tahad, et õpilased saavad päris kogemuse ning automatiseerimise eeliseid. </p>

<p>Ei soovita, kui õpetad mittetehnilist ainet, tahad quick setup'i ilma seadistamiseta või vajad rich multimedia nagu videod ja interaktiivsed quizz'id.</p>

<h2>Kokkuvõte</h2>

<p>GitHub pole traditsioniline LMS ja see ongi punkt - automation kursusele on ideaalne, sest õpime real tools'iga real workflow'd, GitHub Education annab kõik tasuta, Actions automatiseerib kontrolli ja Copilot tuleb peale. </p>

<p>Teen juba kõik oma kursused seal - automation, DevOps, koodimine - kõik mis on seotud tänapäeva IT'ga, sest see annab õpilastele võimaluse harjuda GitHub'i käsitlemisega läbi mitme kursuse, nad saavad praktikat enda materjalide jagamisel ning õpivad kuidas projekte dokumenteerida ja Git'i kasutada - oskused, mida nad igas IT rollis vajavad.</p>

<p>Esimene setup võttis aega, aga nüüd on tulemus võimas ja soovitan igaühele, kes õpetab tehnilist ainet!</p>

<p></p>
