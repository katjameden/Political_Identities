# Cross-corpus comparison - Collocations Analysis

The document records observation on the collocations when compared among the corpora. 

## Settings: 
- CQL query: ([lemma="naš"][]{1,3}[lemma="vaš"])|([lemma="vaš"][]{1,3}[lemma="naš"])within<s/>
- lowercase lemma, range L5R5, min frequency in corpus: 5, min. frequency in range: 3 (default); top 20 collocates
- Comparison of the top 10 collocates in each corpus; additionally, common collocates that appeared outside the top 10 were also identified and matched with the existing set where relevant.


## Table

| Collocate | ParlaMint-SI |  | siParl |  | Trendi |  | CLASSLA |  | JANES |  |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|  | freq. | logDice | freq. | logDice | freq. | logDice | freq. | logDice | freq. | logDice |
| deliti | 63 | 8.39232 | 105 | 7.63226 |  |  |  |  | 87 | 6.71433 |
| delitev | 48 | 8.16632 | 66 | 7.16452 | 227 | 7.80674 | 334 | 6.65207 | 75 | 8.2634 |
| deljenje | 6 | 7.63077 | 7 | 6.68001 | 19 | 5.72412 |  |  |  |  |
| desen | 21 | 7.35958 | 37 | 7.02396 |  |  |  |  |  |  |
| lev | 23 | 7.25268 | 36 | 6.66498 |  |  |  |  |  |  |
| ločevanje | 5 | 7.18366 | 6 | 6.19318 |  |  |  |  |  |  |
| spodnji | 9 | 6.69267 | 10 | 5.4735 |  |  |  |  |  |  |
| zgornji | 8 | 6.62659 | 10 | 5.52002 |  |  |  |  |  |  |
| nevladnik | 3 | 6.45568 | 3 | 5.24178 |  |  |  |  |  |  |
| krasti | 3 | 5.99531 |  |  |  |  |  |  |  |  |
| preštevati |  |  | 5 | 6.1495 |  |  |  |  |  |  |
| katerekoli |  |  | 5 | 5.4389 |  |  |  |  |  |  |
| 🙏 |  |  |  |  | 101 | 10.04673 |  |  |  |  |
| kalkulator |  |  |  |  | 69 | 8.61517 |  |  |  |  |
| cockta |  |  |  |  | 13 | 6.97082 | 37 | 5.85941 |  |  |
| izračunati |  |  |  |  | 67 | 6.80216 |  |  |  |  |
| hvala |  |  |  |  | 128 | 6.48082 |  |  |  |  |
| nekomunist |  |  |  |  | 8 | 6.42399 |  |  |  |  |
| relativizem |  |  |  |  | 8 | 6.25265 |  |  |  |  |
| slepiti |  |  |  |  | 10 | 6.22785 |  |  |  |  |
| frljić |  |  |  |  | 7 | 6.12085 | 40 | 5.99634 |  |  |
| marijana@alphaluxegroup.com |  |  |  |  |  |  | 197 | 8.353 |  |  |
| povzdigniti |  |  |  |  |  |  | 315 | 8.26927 |  |  |
| prenrediti |  |  |  |  |  |  | 59 | 6.60129 |  |  |
| featuring |  |  |  |  |  |  | 65 | 6.43055 |  |  |
| pridih |  |  |  |  |  |  | 145 | 6.37694 |  |  |
| prioriteta |  |  |  |  |  |  | 163 | 6.25599 |  |  |
| poslovalnica |  |  |  |  |  |  | 109 | 6.24947 |  |  |
| prednosten |  |  |  |  |  |  | 161 | 6.09096 |  |  |
| mladost |  |  |  |  | 51 | 5.89389 | 155 | 6.06167 | 39 | 7.30419 |
| natisnjen |  |  |  |  |  |  |  |  | 861 | 12.81913 |
| prinesti |  |  |  |  |  |  |  |  | 864 | 9.76785 |
| forum |  |  |  |  |  |  |  |  | 865 | 9.51737 |
| preko |  |  |  |  |  |  |  |  | 863 | 9.41135 |
| odgovor |  |  |  |  |  |  |  |  | 866 | 8.49462 |
| razdeljen |  |  |  |  |  |  |  |  | 10 | 6.25449 |
| ići |  |  |  |  |  |  |  |  | 5 | 6.00678 |

### Observations: 

- The most notable observation is that the collocate **"delitev"** ("division") appears across all corpora.
    - In the parliamentary corpora, **"delitev"** is the second strongest collocate, surpassed only by **"deliti"** ("to divide").
    - In the other corpora, **"delitev"** also ranks among the strongest collocates. However, the highest-ranking collocates in these corpora are often associated with recurring texts and other sources of noise, which partially obscure the prominence of **"delitev"**.
- Other matched collocates (which mostly fall outside the logDice threshold) are shared between:
    - parliamentary corpora: nevladnik (non-government official): While based only on 3 speeches (so, not eligable for a generalisation), this seems to denote another dimension of divisions. In this case all three instances belong to Violeta Tomič (Levica) in Term 8:
        - "*In kar naprej se gremo **naši-vaši**; naši nevladniki, vaši nevladniki in tako naprej.*" (“And we keep playing at **ours–yours**; our NGOs, your NGOs, and so on.”)
    - web corpora: cockta
    - Trendi, CLASSLA and JANES - mladost (youth): Collocates "cockta" (name of a popular drink) and "youth" are part of a slogan: 
        - "*[@per] mah.. Mislim da je cockta kar pijača **naše in vaše mladosti**. :-))*" (“[@per] well.. I think *Cockta* is really the drink of **our and your youth**. :-))”) 
        - Indicating the function of the terms "ours" and "yours" also in relation to positive, shared experiences.
- With respect to the logDice metric, where strong collocations are typically defined as those with a score of 7 or above, the strong collocations for the corpora appear to be:
   - ParlaMint-SI: deliti (to divide), delitev (division), deljenje (division), desen (right), lev (left), ločevanje (to separate; however, this collocate is based on a low frequency of speeches)
        - All these collocates relate to the concept of political division (either as an accusation against the opposing side of dividing, criticism of division, or a call for unity).
    - siParl: most of the strongest collocates that appear in ParlaMint-SI also appear in siParl: deliti, delitev, desen, with slightly lower logDice scores.
        - This is unsurprising due to the overlap in data between the corpora.
    - Trendi: The strongest collocate is not a word, but an emoji (); among the strong collocates are also: kalkulator (calculator) and **delitev**. The first two collocates refer to repeated texts:
        * "*Izračunajte si **vašo plačo z našim** kalkulatorjem!*" (“Calculate **your salary with our** calculator!”)
        * "*Naša prihodnost bo tudi vaša. Hvala vam! *" (“**Our future will also be yours**. Thank you! ”)
    - CLASSLA: The strongest collocates include an email address (*marijana...*) and *povzdvignil* ("raised"), both of which appear to be artefacts of noise rather than meaningful semantic associations.
        * The collocate **"delitev"** ("division") falls below the logDice threshold, likely due to the large amount of noise in the corpus. Nevertheless, as with Trendi, it is the first collocate that directly relates to the semantic content under investigation, with most occurrences referring to political polarisation and divisions.
        * "*Delitev na '**vaše**' in '**naše**' je treba ukiniti.*" (“The division into '**yours**' and '**ours**' should be abolished.”)
        * "*Kritizirajo vlado, ker se loteva odpravljanja nezakonitosti, vzpodbujajo delitev ter kulturni boj, ideološke polarizacije, delitev na '**vaše in naše**'.*" (“They criticise the government for addressing illegalities, while promoting division, culture wars, ideological polarisation, and the division into '**yours and ours**'.")
    - JANES: prinesti, forum, preko, odgovor, delitev – as with the web corpora, here too, a large proportion of the highest-rated collocates are noise.
        * "delitev", as with the web corpora, seems to be the only collocate actually connected with the terms under observation; it is also the last collocate that is still above the threshold for strong collocation.