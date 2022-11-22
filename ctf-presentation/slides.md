---
# try also 'default' to start simple
theme: bricks
# random image from a curated Unsplash collection by Anthony
# like them? see https://unsplash.com/collections/94734566/slidev
background: https://source.unsplash.com/collection/94734566/1920x1080
# apply any windi css classes to the current slide
class: "text-center"
# https://sli.dev/custom/highlighters.html
highlighter: shiki
# show line numbers in code blocks
lineNumbers: false
# some information about the slides, markdown enabled
info: |
  ## CTF
  Qu’est-ce qu’un CTF

# persist drawings in exports and build
drawings:
  persist: false
# use UnoCSS
css: unocss
---

# CTF

Qu’est-ce qu’un CTF

<div class="pt-12">
  <span @click="$slidev.nav.next" class="px-2 py-1 rounded cursor-pointer" hover="bg-white bg-opacity-10">
    let's go <carbon:arrow-right class="inline"/>
  </span>
</div>

<!-- <div class="abs-br m-6 flex gap-2">
  <button @click="$slidev.nav.openInEditor()" title="Open in Editor" class="text-xl icon-btn opacity-50 !border-none !hover:text-white">
    <carbon:edit />
  </button>
  <a href="https://github.com/slidevjs/slidev" target="_blank" alt="GitHub"
    class="text-xl icon-btn opacity-50 !border-none !hover:text-white">
    <carbon-logo-github />
  </a>
</div> -->

<!--
The last comment block of each slide will be treated as slide notes. It will be visible and editable in Presenter Mode along with the slide. [Read more in the docs](https://sli.dev/guide/syntax.html#notes)
-->

---

# Qu’est-ce qu’un CTF?

CTF est l’abbreviation de _Capture The Flag_ (Capture de Drapeau)

Capture the Flag (CTF) : il s'agit d'une activitée gamifiée consistant en l'obtention d'une information sensible, le drapeau ou flag.

Le drapeau est généralement sous la forme d'une chaîne de caractères alphanumériques.

Pour obtenir cette chaîne de caractère, il faut relever un défi.les participants doivent s’introduire dans un système afin de récupérer le drapeau (flag).

Ceci s’apparente à une intrusion dans un système réel, avec vol de données … sauf qu’ici le drapeau n’a pas de valeur monétaire, et personne ne vous en voudra.

---

# Un peu d'infos utiles?

Les CTFs sont des évenements en live et souvent en équipe mais il est possible de s'entrainer, d'apprendre et de s'amuser en dehors de ces événements live

- 🔴 **CTF en live** - [CTF Google](https://capturetheflag.withgoogle.com/), **Defcon** **wargame**. En France il y a par exemple un evenement célèbre: la **NuitDuHack**
- 🗂 **ctftime.org** - Ce site répertorie tous les CTFs
- 🧑‍💻 **Site pour s'entrainer ou apprendre** - **[TryHackMe](https://tryhackme.com/)** super pour apprendre, **[Root-Me](https://www.root-me.org/)**, **[HackTheBox](https://www.hackthebox.eu/)**

<br>
<br>

<!--
You can have `style` tag in markdown to override the style for the current page.
Learn more: https://sli.dev/guide/syntax#embedded-styles
-->

<style>
h1 {
  background-color: #2B90B6;
  background-image: linear-gradient(45deg, #4EC5D4 10%, #146b8c 20%);
  background-size: 100%;
  -webkit-background-clip: text;
  -moz-background-clip: text;
  -webkit-text-fill-color: transparent;
  -moz-text-fill-color: transparent;
}
</style>

<!--
Here is another comment.
-->

---

# À quoi s’attendre lors d’un CTF ?

🤔

Un CTF est en général composé de plusieurs épreuves réparties dans différentes catégories et pour différents niveaux, du plus facile au plus difficile. Savoir dans quelle catégorie se trouve un challenge peut aider à l’appréhender.

---

### Les catégories que l’on retrouve en général; avec un exemple de challenge

|                                     |                                                                                                                      |
| ----------------------------------- | -------------------------------------------------------------------------------------------------------------------- |
| Binary Analysis/Reverse Engineering | on vous fournit un executable et vous devez extraire le drapeau.                                                     |
| Web                                 | exploitation du service web avec les vulnérabilités classiques (OWASP)                                               |
| Forensic                            | une machine a été compromise, on vous fournit RAM/Disque/Logs/… et vous devez trouver une information précise dedans |
| Réseau                              | votre réseau a subi une attaque DoS et vous devez trouver qui l’a attaqué et comment.                                |
| Cryptographie                       | implémentation d'un algorithme de chiffrement avec une faille et vous devez exploiter cette faille.                  |
| Stéganographie                      | une information est cachée dans une image, à vous de la retrouver.                                                   |

---

# Quel matériel préparer pour un CTF ?

Le matériel dépendra du CTF

s’il se déroule en ligne votre ordinateur suffira, Les outils parfaits pour réaliser un pentest sont globalements les mêmes pour participer à un CTF : une machine Linux de préférence, encore mieux si c’est [Kali Linux](https://www.kali.org/get-kali/).

Des liste d’outils utiles pour les CTF sont disponibles : [github.com/zardus/ctf-tools](https://github.com/zardus/ctf-tools) et [awesome-ctf](https://github.com/apsdehal/awesome-ctf#solve). N’hésitez pas à les consulter pour avoir une idée des armes à votre disposition.

Beaucoup d’entre eux sont déjà intégrés à Kali Linux.

Pour ma part j'utilise Kali en virtual machine sur un mac m1

---

# Sources et liens

- [le petit guide du chasseur de drapeaux](https://ungeek.fr/le-petit-guide-du-chasseur-de-drapeaux/)
- [What is CTF and how to get started!
  ](https://dev.to/atan/what-is-ctf-and-how-to-get-started-3f04)
- [A fun way to learn cyber security](https://tryhackme.com/)
- [Quelques conseils pour créer un (bon) CTF
  ](https://osintfr.com/fr/quelques-conseils-pour-creer-un-bon-ctf/)
- [P'Hack CTF 2021
  ](https://github.com/phackctf/phack-ctf-2021-public)

  ## Amusez-vous
