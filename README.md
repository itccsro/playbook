[![Slack](https://img.shields.io/badge/slack-%23playbook-green.svg)](https://civictechro.slack.com/messages/CAFLVGYJ0/) 
[![GitHub license](https://img.shields.io/github/license/civictechro/playbook.svg)](https://github.com/civictechro/playbook/blob/master/LICENSE) 

[![GitHub issues by-label](https://img.shields.io/github/issues-raw/civictechro/playbook/help%20wanted.svg)](https://github.com/civictechro/playbook/issues) [![GitHub issues by-label](https://img.shields.io/github/issues-raw/civictechro/playbook/good%20first%20task.svg)](https://github.com/civictechro/playbook/issues) 

# Strategii pentru Servicii Digitale

*https://civictechro.github.io/playbook/*

CivicTech România își dorește să folosească potențialul tehnologiei Open Source și talentul specialiștilor români pentru a dezvolta noi servicii digitale de utilitate publică.

România este pe ultimul loc în Europa în ceea ce privește [gradul de utilizare al serviciilor publice digitale către cetățeni](http://bit.ly/desireport). Prin strategiile pe care le adoptăm în dezvoltarea proiectelor noastre, credem că putem livra servicii digitale funcționale, moderne, cu un impact pozitiv direct pentru cetățeni. Fiecare proiect dezvoltat în cadrul CivicTech România trebuie să răspundă cerințelor de mai jos, iar acolo unde nu este posibil din prisma constrângerilor specifice fiecărui proiect, trebuie tratat ca o excepție de la regulă.

***
*Acest document este în continuă dezvoltare, folosind ca sursă de inspirație [The US Digital Services Playbook](https://playbook.cio.gov/), [principiile CivicTech România](https://civictech.ro/cine-suntem#principii), cât și metodele de lucru care s-au dovedit eficiente în cadrul organizației.*

## Detalii tehnice

Conținutul este compilat din fișiere [Markdown](https://help.github.com/articles/github-flavored-markdown "Link to More Information About Markdown"), folosind [Jekyll](https://github.com/jekyll/jekyll "Link to More Information about Jekyll").

### Cum rulez site-ul local?

Dacă vrei să rulezi site-ul local, va trebui să instalezi [Jekyll](https://github.com/jekyll/jekyll "Link to More Information about Jekyll") și dependințele sale.

1. Dacă nu ai deja Ruby și Bundler instalate, urmărește [cei doi pași pentru instalare](https://help.github.com/articles/using-jekyll-with-pages#installing-jekyll "Installation instructions for Jekyll").
2. Apoi, ai nevoie de [un fork al acestui repository](https://help.github.com/articles/fork-a-repo/ "Instructions for Forking Your Repository") pe care îl poți clona local.
3. Din root-ul proiectului, pe calculatorul tău, poți rula `bundle install` în terminal.

Pentru a rula site-ul local, rulează `jekyll serve --watch` din terminal, apoi deschide `http://localhost:4000/` în browser.

### Cum editez stylesheets?

Proiectul folosește [Sass](http://sass-lang.com/ "Link to Learn More About Sass") pentru management de CSS. Codul îl poți găsi în [`styles.scss` file](assets/_sass/styles.scss). Folosim [suportul SASS nativ pentru Jekyll](https://jekyllrb.com/docs/assets/) pentru a genera fișierele CSS, când rulezi site-ul local.

## Cum pot propune o schimbare de conținut?

Dacă vrei să propui o schimbare, trimite un [pull request](https://help.github.com/articles/creating-a-pull-request "More Information on Submitting Pull Requests"), cu o schimbare într-unul dintre fișierele Markdown. Fiecare strategie se poate găsi în [folderul `_plays`](https://github.com/civictechro/playbook/tree/master/_plays). Introducerea se află în [folderul `_include`](https://github.com/civictechro/playbook/tree/master/_include).

Fișierele se pot edita și direct în browser, fără a fi necesară instalarea de software adițional.

----------

**Made with :heart: & :coffee: by [CivicTech România](https://civictech.ro/)**
