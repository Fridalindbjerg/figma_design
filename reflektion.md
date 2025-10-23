# Reflektioner over opgaven

## Uorganiseret arbejde

Hvis jeg skulle gøre det hele om igen, ville jeg gå meget mere strategisk og organiseret til værks. Når opgaven er så opdelt i komponenter, og derfor har det været nemt at hoppe fra komponent til kompenent, når jeg er løbet ind i et problem. Det har blandet andet gjort, at jeg ikke har organiseret mine font-sizes globalt og givet mine sections margins i gloabl, så de alle sammen er ens.

## Global og componentbaseret css

Jeg har organiseret så mine fontsizes, spaces og min 'skelet' er indsat i global, som er linket i min Layout, så jeg kan bruge mine forskellige classes på alle componenter.

```astro
<img src="/src/assets/images/spacefonts.png" alt="">
<img src="/src/assets/images/bodygrid.png" alt="">
```

(jeg kan ikke finde ud af at sætte det ægte billede ind ???)

## Kode fra undervisningen

##### Flexwrap:wrap til @media

```astro
     @media (max-width: 768px) {
        flex-wrap: wrap;

        li {
          flex-direction: row;
        }
      }
```

##### Details

```astro
<details name="accordion">
    <summary> {question.question} </summary>
        <div>
            <p>{question.answer}</p>
        </div>
</details>
```

##### Scroll snap på x-asken med costum props

```astro
ul{
    overflow-x: auto;
    --scroll-padding: max(1rem, 50% - var(1200px) / 2);
    scroll-padding-inline: var(--scroll-padding);
    padding-inline: var(--scroll-padding);
    scroll-snap-type: x mandatory; /* Aktiver snap på x-aksen */
    scroll-behavior: smooth;
    }
```

## Udfordringer

##### Props til at ændre farve i CoreValues.astro.

- Fik det aldrig rigtig til at virke. Kan godt bruge props, men kunne ikke få det til at ramme de rigtige ting

##### Brug af de små grønne bokse med position: absolute

- Jeg endte med helt at skrotte de grønne bokse, da de responsivt ikke var til at arbejde med. Måske vi kan snakke om, hvordan man løser det på en god måde?

##### Brug af DynamicImage

- Virkede kun nogle gange??

##### Stier i Astro

- Driller altid, når jeg skal deploy. Det er noget med root og sjov, som ikke rigig virker? Kan vi evt snakke om fælles

##### Minus-margin på fx index ved service-bokse

- Er ikke super responsivt. Snakkede med Chattie, som sagde, at man kan gøre noget med at ligge den position: relative i stedet for, men kastede mig ikke ud i. Tænker du viser en top dollar løsning i morgen.

##### Drilleri med casestudie ved responsivitet

- Der er noget med et skelet, der ikke helt virker. Snakkede igen med Chattie, men blev enig med mig selv om, at det gik nok.

##### Sikkert flere, men jeg kan ikke huske lige nu

## Succeser

##### Brug af .map

- Den sidder på rygraden nu !!

##### Brug af skelet med full-bleed, content osv

- Godt at få i hænderne og forstå hvordan det virker ift til direkte børn.

##### Masser af leg med flex og grid

- Jeg ved mange har været trætte af opgaven. Jeg har ikke. Måske jeg grundlæggende har misforstået noget ?? Men if it works it works i guess ;)
