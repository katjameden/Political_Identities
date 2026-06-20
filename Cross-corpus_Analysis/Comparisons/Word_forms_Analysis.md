# Cross-corpus comparison --  Word forms Analysis 

The documents records observations on the patterns of word forms across all of the corpora compared. 

## Settings
- CQL query: ([lemma="naš"][]{1,3}[lemma="vaš"])|([lemma="vaš"][]{1,3}[lemma="naš"])within<s/>
- Word forms: top 20 (metric: % of concordance)
- Comparison table: Matching top 5 word forms (due to very small numbers) and their percentages of concordance lines (``% of concordance``) among the corpora.
    
## Table

| **Form** | **ParlaMint (% of concordance)** | **siParl (%)** | **Trendi (%)** | **CLASSLA (%)** | **JANES (%)** |
| --- | --- | --- | --- | --- | --- |
| **naše  in  vaše** | **8.51** | **6.65** | **12.01** | **3.6** | **6.68** |
| **vaše  in  naše** | **5.06** | **3.22** | **3.99** | **2.03** | **3.2** |
| *naše  ,  vaše* | *2.64* | *2.02* |  |  |  |
| *naši  ,  vaši* | *2.3* | *1.82* |  |  |  |
| vaši  in  naši | 1.38 |  |  |  |  |
| *naših  in  vaših* |  | *1.3* |  | *0.8* |  |
| Naša  prihodnost  bo  tudi  vaša |  |  | 3.62 |  |  |
| naše  "  in  "  vaše |  |  | 2.71 |  |  |
| vašo  plačo  z  našim |  |  | 2.24 |  |  |
| Vaše  zadovoljstvo  je  naša |  |  |  | 0.9 |  |
| Vaše  zadovoljstvo  je  naše |  |  |  | 0.88 |  |
| vaša  vprašanja  in  naše |  |  |  |  | *34.45* |
| naši  in  vaši |  |  |  |  | 2.2 |
| naši  /  vaši |  |  |  |  | 1.76 |


- The first and most obvious observation pertains to the "naše in vaše", as well as the opposite form "vaše in naše" appearing in every single corpus, in most cases as the two top word forms: 
    - In most cases, these specific word forms (no matter the corpus) relate to political division and polarisation (delitev na; ločevanje na ... naše in vaše, ...):
        -   "*In nehajmo se deliti na **naše in vaše** ter na prvo- in drugorazredne.*" (“And let us stop dividing ourselves into **ours and yours**, and into first- and second-class citizens.”)
        -   "*...sem se naposlušal v tem Državnem zboru govoriti o **naši, vaši**, oni, mi, vi.*" (“...I have heard enough in this National Assembly about **ours, yours**, they, us, you.”)

    - There are also quite some references to children (and future) in some of these top forms: 
        - "*Vi pa tudi premislite ali se splača uničevati prihodnost **vaših in naših otrok**, kakorkoli želite.*" (“And you should also consider whether it is worth destroying the future of **your and our children**, however you may wish to do so.”)
        - "*Javni interes je, da se **naši, vaši, katerikoli otroci** kvalitetno izobražujejo.*" (“It is in the public interest that **our, your, or any children** receive a quality education.”)
    - In the case of CLASSLA, while political polarisation is still the dominating pattern, there are also quite some references to additional topics and positive common experiences: 
        - "*Avtorske pesmi z nepozabnimi zgodbami, humor, ki poživlja, in glasba **naše in vaše mladosti***" (“Original songs with unforgettable stories, refreshing humour, and the music of **our and your youth**.”)
        -  "*'Pijača **naše in vaše mladosti**' ima za sabo številne vzpone in padce*" (“The '**drink of our and your youth**' has experienced numerous ups and downs.”) 
        - "*Kdo je človek, ki je ustvaril **pijačo vaše in naše mladosti***" (“Who is the man who created the **drink of your and our youth**?”)

    - The only exception to this is the JANES corpus, where the most common form (and the highest percentage overall) is "*vaša vprašanja in naše (odgovore)*" (your questions and our [...responses]), which is due to high amount of repetitive and urelated texts (noise)
- Additionaly, overall percentages (again, with the exception of JANES and to lesser degree also Trendi corpus) are relatively low , showing that the concordances are very diverse. 
- Otherwise, there is no additional exact overlap between any of the forms and corpora; however, there are many forms of "naši" and "vaši": ("naše in vaše"; "vaše in naše"; "naše , vaše"; ... "naši / vaši"), where political division is detected: 
    - Živeli naši in vaši ! - [URL] [URL]
