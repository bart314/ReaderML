# Reader machine learning

Met het toenemend belang van Machine Learning (ML) in de dagelijkse praktijk van de software engineer heeft dit onderwerp zijn weg inmiddels gevonden naar het HBO. Het onderwijsaanbod of de online courses richten zich evenwel nog steeds op ofwel de academicus (met veel wiskunde voorzien van rigoreuze bewijzen) ofwel op puur de dagelijkse gebruiker van specifieke frameworks (het in elkaar typen van Keras netwerken zonder achterliggend begrip). Er is dus behoefte aan onderwijsmateriaal dat deze twee extremen met elkaar verbindt: deze reader is een poging daartoe.

De reader behandelt functies en lineaire algebra, maar zonder de praktische toepassing hierbij uit het oog te verliezen. Er wordt een directe koppeling tussen de wiskundige theorie en de implementatie daarin in numpy gegeven. Verder wordt het principe van regressie-analyse toegelicht, wat wordt toegepast op classificatieproblemen. Tenslotte worden neurale netwerken en de *confusion matrix* besproken.

Deze reader is bedoeld als ondersteunend materiaal bij hoor- en werkcolleges over hetzelfde onderwerp in het vierde jaar van de opleiding Software Engineering van Hanzehogeschool Groningen; het is evenwel de hoop dat hij ook op zichzelf informatief is en studenten een beter inzicht geeft in de achterliggende theorie.


## Gebruikte packages en andere dependencies

Hieronder volgt de volledige lijst van packages die nodig zijn om de reader te maken. Het is allemaal niet heel spannend. De reader moet wel gemaakt worden met Lua(La)Tex, omdat anders bepaalde diakritische tekens niet goed doorkomen.

```
\usepackage[utf8]{inputenc}
\usepackage{polyglossia}
\usepackage[font={small,it}]{caption}
\usepackage{fontspec}
\usepackage{fancyhdr}
\usepackage{amsmath}
\usepackage{listings}
\usepackage{subfiles}
\usepackage{multicol}
\usepackage{titlesec}
\usepackage{tcolorbox}
\usepackage{color}
\usepackage{hyperref
```

## Opbouw
Om het werken met de tekst wat overzichtelijker te maken, is de reader opgebouwd uit verschillende losse bestanden – per hoofdstuk een separaat bestand. De \begin{document} en \end{document} zitten in reader.tex. De inhoudsopgave is als volgt:

```
\subfile{voorblad}
\subfile{functies}
\subfile{matrix_vector}
\subfile{rekenen_matrix}
\subfile{opgaven}
\subfile{numpy}
\subfile{lineaire_regressie}
\subfile{logistische_regressie}
\subfile{neural_nets}
\subfile{confusion_matrix
```

## Disclaimer
De tekst is aan continue verandering onderhevig: nieuwe inzichten, betere voorbeelden en uitbreidingen die tijdens discussies of lessen zijn bedacht of opgedaan vinden hun weg van de collegebanken naar hun tekstuele weerslag alhier. 

Hoewel de tekst met de grootste zorg is geschreven en gecontroleerd, is het niet ondenkbaar dat er fouten in zijn geslopen (zowel grammaticaal als inhoudelijk), of dat onderdelen niet volledig of onduidelijk zijn. Het staat vanzelfsprekend iedereen vrij om een pull request te doen.


