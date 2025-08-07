# Helló kedves látogató! (per önkéntes tartalom szerkesztő)

#### Ez a repository szolgálja a lelkét a Project Athena programnak, itt gyűjtök össze minden érdekesebbnél érdekesebb infót, leírást, ismeretterjesztőt és egyebeket a világról, filozófiai, pszchológiai, történelmi, művészeti és egyéb témákban.

Az adat halmaz, mint gondolom sejtitek a [datas.json](datas.json) file-ban találhatóak, és onnan kerülnek beolvasásra...
- Terveim szerint ezt az adathalmazt majd katyvaszként is lehet bővíteni, mert megfelelően felcímkézve és dátumkozva a Project Athena megfelelően fogja tudni szortírozni.

Jelenlegi formátum:
```json
[
    {
        "title": "10 Megoldhatatlan paradoxon, amire sosem kapunk választ", 
        "url": "https://www.youtube.com/watch?v=9J9DmFtN5Qo&pp=ygUJcGFyYWRveG9u",
        "tags": ["philosophy", "video", "paradoxon", "youtube"],
        "format": "video",
        "source": "10-es lista",
        "language": "hu",
        "recordDate": "2019-10-18",
        "sourceDate": "2025-08-02"
    },
]
```
### Megeshet hogy valamiben nem egyértelmű a dolog, ezért leírom itt elmagyarázva:
```js
"title": "10 Megoldhatatlan paradoxon, amire sosem kapunk választ",  
/* A bejegyzés címe. Ez általában legyen a Youtube videó címe, a cikk/poszt címe, illetve ha nincs, akkor valamikomolyan vehető címet adjunk neki */
"url": "https://www.youtube.com/watch?v=9J9DmFtN5Qo&pp=ygUJcGFyYWRveG9u", 
/* Az elérési útvonal */
"tags": ["philosophy", "video", "paradoxon", "youtube"],
/* tag-ek (vagy címkék) amik szerint lehet csoportosítani, legyenek angol slug megnevezések, amikhez tudunk majd forításokat rendelni a későbbiekben*/
"format": "video",
/* a tartalom formátuma, amire számíthat a felhasználó a linken */
"source": "10-es lista",
/* forrás megnevezése, youtube csatorna neve, weboldal neve */
"language": "hu",
/* próbáljuk meg tartani a ISO 639-1 nyelvkódok használatát a könnyű azonosítás érdekében (angol esetében inkább használjuk az "en-us" kódot, hogy brit és amerikai zászlót vegyítve jelenítsük meg) */
"recordDate": "2019-10-18",
/* bejegyzés dáruma */
"sourceDate": "2025-08-02"
/* opcionális (ismert adat esetén igényelt info) mikor jelent meg a forrás */
```

[ISO 639-es nyelvi kód szabvány](https://www.wikiwand.com/en/articles/List_of_ISO_639_language_codes)