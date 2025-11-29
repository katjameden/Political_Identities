# Discourse Analysis

# Basic distributions of the subcorpora

- 3 subcorpora - Naš (Ours), Vaš (Yours) and Naš/Vaš (Ours vs. Yours, subcorpus including both lemmas within one sentence); or N, V and NV from here on out.
- Overall corpus size of ParlaMint-SI 5.1: 81,683,385 (tokens)

To determine whether to exclude procedural speeches from the analysed subcorpora, we also examined the frequency distributions of speeches according to the Speaker_role text type, which includes “Regular” (i.e. speeches made by speakers not in the Chairperson role) and “Chairperson” values (i.e. often procedural speeches given by the chairperson of the session):

Additionally, given the different discourse frames, we, as with the metadata analysis, focused only on MP speeches. Therefore, we removed procedural speeches and excluded speeches made by ministers and non-MP (guest) speakers. The final distributions of the subcorpora used for the discourse analysis are shown in Table 1.

| Subcorpus | Hits | % in corpus | Freq per million tokens | Tokens | Words (approx.) | % of total corpus tokens |
| --- | --- | --- | --- | --- | --- | --- |
| Naš (N) | 119,440 | 0.15 | 1462.23 | 37,383,574 | 31,593,806 | 45.8 |
| Vaš (V) | 38,362 | 0.047 | 469.64 | 14,473,892 | 12,232,253 | 17.7 |
| Naš_Vaš (NV) | 2,578 | 0.0032 | 31.56 | 1,829,072 | 1,545,795 | 2.2 |

As some speeches may include both “naš” and “vaš” concordances within a single sentence, these are present in both subcorpora, resulting in some overlap between the two main subcorpora. Therefore, we also created an additional subcorpus (NV), which contains only those speeches that include both “naš” and “vaš” concordances in a single speech, and calculated the percentage of speech-based overlap, as shown in Table 2.

| Subcorpus | Hits | Unique Speech_IDs | Unique Session_ID | Naš_/Vaš_only (count, %) | Overlap (count, %) |
| --- | --- | --- | --- | --- | --- |
| NR | 119,440 | 50,951 | 1,543 | 49,052 (96.27%) | 1,899 (3.72%) |
| VR | 38,362 | 20,038 | 1,477 | 18,13 (91.52%) | 1,899 (9.47%) |
| NVR | 2,578 | 1,899 | 859 |  /| / |

Effectively, the overlapping speeches in the NV subcorpus represent only 3.74% of the N subcorpus and 8.99% of the V subcorpus. While the N and V subcorpora are used to investigate different trends distinctly connected to and typical of their respective pronouns, the NV subcorpus allows investigation of trends common to the joint usage of both pronouns in a single sentence, as well as the “vaši in naši” phenomenon and the identities within.

# Text types analysis

To establish basic characteristics of the subcorpora, we examined several metadata fields (and their frequencies, RF and relative density), related to the political identity and sentiment, which can give us insight/comparison with overall trends identified in metadata analysis:

- Sentiment related metadata (speech-level 3-class sentiment)
- Coalition/opposition (Group relations)
- Minister status (Membership)
- Political orientation (Ideology)

**Sentiment** 

| Sentiment | Naš |  |  | Vaš |  |  | Naš_Vaš |  |  |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|  | F | RTT | RD (%) | F | RTT | RD (%) | F | RTT | RD (%) |
| Positive | 17,404 | **1,948.13** | **133.23** | 1,211 | 135.55 | 28.86 | 137 | 15.34 | 48.59 |
| Negative | **83,080** | 1,597.79 | 109.27 | **34,658** | **666.54** | **141.92** | **2,240** | **43.08** | **136.50** |
| Neutral | 18,956 | 913.42 | 62.47 | 2,493 | 120.13 | 25.58 | 201 | 9.69 | 30.69 |

While the majority of the N speeches belong to the Negative sentiment (F), the concordance appears typical of the Positive sentiment, which is logical as “naš” and related “ Us” concepts generally carry positive sentiment and viewpoints compared to “Them” or the comparison between “Us and Them”. Conversely, the speeches in V and in the NV subcorpus are both most frequent and representative of Negative sentiment. 

**Party status (Coalition/Opposition)**

| Party status | Naš |  |  | Vaš |  |  | Naš_Vaš |  |  |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|  | F | RTT | RD (%) | F | RTT | RD | F | RTT | RD (%) |
| Coalition | 48,216 | 1,438.97 | 98.41 | 9,778 | 291.82 | 62.14 | 716 | 21.37 | 67.71 |
| Opposition | **63,845** | **1,785.92** | **122.14** | **26,663** | **745.84** | **158.81** | 1,736 | 48.56 | 153.86 |
| None (-) | 7,379 | 593.78 | 40.61 | 1,921 | 154.58 | 32.91 | 126 | 10.14 | 32.13 |
- Error in metadata (SDS → Opposition → Term 3), other speakers that are also from different parties are actually speaking in their status change (not yet confirmed to be NP, but not part of the parliamentary group, but still affiliated with political party).
- In all three subcorpora, the concordances are both most frequent and most typical of the Opposition speeches.
- In all three subcorpora, the concordances seem to be even less typical of the speeches, that are produced by speakers that do not belong to a specific party (status) than of the Coalition speeches, even though there is a substantial difference in terms of raw frequencies (where there is at least twice as many Coalition speeches than None).

**Party Orientation**

| Party Orientation | Naš |  |  | Vaš |  |  | Naš_Vaš |  |  |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|  | F | RTT | RD (%) | F | RTT | RD (%) | F | RTT | RD (%) |
| Right | 27,501 | 1,380.38 | 94.40 | **13,642** | 684.75 | **145.80** | **837** | 42.01 | **133.12** |
| Centre to centre-left | **29,531** | 1,552.23 | **106.16** | 8,876 | 466.55 | 99.34 | 600 | 31.54 | 99.93 |
| Centre-left | 20,604 | 1,409.04 | 96.36 | 6,089 | 416.41 | 88.66 | 456 | 31.18 | 98.81 |
| - | 4,035 | 388.35 | 26.56 | 1,006 | 96.82 | 20.62 | 61 | 5.87 | 18.60 |
| Centre-right | **22,470** | **2,298.11** | **157.16** | 3,916 | 400.51 | 85.28 | 305 | 31.19 | 98.84 |
| Left | 6,203 | 1,726.98 | **118.11** | 2,564 | 713.84 | **152.00** | 174 | 48.44 | **153.49** |
| Right to far-right | 7,982 | 2,232.01 | **152.64** | 2,095 | 585.8 | **124.74** | 134 | 37.47 | **118.72** |
| Centre to centre-right | 945 | 1,318.34 | 90.16 | 162 | 226.00 | 48.12 | 11 | 15.35 | 48.62 |
| Centre | 169 | 2,783.86 | **190.38** | 12 | 197.67  | 42.09 | / | / | / |
- Naš: Concordance is most typical of the Centre (RD: 190.38%), but also typical of the Centre-right (157.16%), Right to far-right (152.64%), Left (118.11%) and Centre to centre-left (106.16%) speeches. In terms of raw frequency, concordance is most frequent in Centre to centre-left speeches. Concordance therefore seems typical for both right and left-wing parties, but less so for the centre and NP/NeP/MPs in transition. However, it is important to note the sizeable difference in the overall Left/Right speech distributions in the subcorpus.
- Vaš: Concordance is most frequently present in Right speeches, but is most typical of Left speeches (RD: 152.00%), as well as Right (145.80%) and Right to far-right (124.74%) speeches.
- Naš_Vaš: Lastly, concordance is most frequent in Right speeches, but is more typical of Left speeches (153.49%). Concordance is also typical for Right (133.12%) and Right to far-right (118.72%) speeches.
- In all three subcorpora, concordances are prominent in Right and Left speeches, which is not surprising given the political struggle between the two extremes.

# Collocation Analysis

## Methodology

The collocations, (series) of words pr terms that co-occur left or right of the keyword in context (KWIC) can help us answer the question of “who/what is ours or yours”? and by extension, help connect the sentiment and use of those collocates with the political identities. To allow for this, we analysed the colocations of individual subcorpus based on the following settings: 

- Lemma lowercase -  the form allows capturing different forms of words
- Context window: L0R1 (checking the lemmas that appear directly next to the concordance in question, essentially capturing the “naš[a]/vaš[a] [vlada/družina/svoboda]”. The window is expanded (L3R3) for the NV subcorpus due to the multi-word KWIC.
- LogDice and other metrics: The main metric that ranks the collocations and the strength of their association we will be using to aid in interpretation is logDice. As described in Rychlý (2018) and Brezina (2018), logDice metric is one of the more popular and preferred statistical measures to identify the strength of co-occurrences of two words. The theoretical maximum value is 14 (in case when all occurrences of X co-occur with Y and all occurrences of Y co-occur with X. Usually the value is less than 10), value 0 means that there is less than 1 co-occurrence XY per 16,000 X or 16,000 Y, and negative values denote no statistical significance of the XY collocations (Rychlý, 2018). Additionally, we will also be checking supporting metrics in the concordancer (MI3, …) to aid in the assessment of the collocation stability.
- Top 20 collocations will be manually checked to investigate their use in context of parliamentary debates. Given that some collocations can indicate connection with specific political identity building categories, the collocations will be annotated with their respective PI categories. As some collocations can (in different context) correspond to different PI categories (Dominant PI category). It is important to note here that the categories assigned  (Dominant, Secondary/Alternative) represent functional tendencies of collocations in parliamentary speech. They should be interpreted as **markers of political identity**, often operating indirectly: the collocation signals alignment, values, or group belonging, rather than explicitly stating identity. This classification is meant to capture typical functions in discourse and may vary depending on context, therefore additional secondary and tertiary categories can be provided if needed. These annotations are accompanied by explanation or reasoning behind the annotation and an example of use.
- Naš/Vaš (NV subcorpus) collocations: Given the multi-word KWIC in the subcorpus and to confirm the trends identified, we also checked different settings (higher DF settings, broader context window (-5,5) and (-10,10)) and restricting the CQL of the subcorpus ({0,5}, {0,3}, one token), which substantially lowered the hits (0,5: } – 1,078 hits, {0,3} – 801 hits and one token between lemmas – 412 hits.

## Naš collocations 

The top 20 collocations, alongside their PI annotations and examples can be found in the [Nas_collocations](../Discourse_Analysis/Collocation_Analysis/Nas_collocations.tsv), [Vas_collocations](../Discourse_Analysis/Collocation_Analysis/Vas_collocations.tsv), and [Nas_Vas_collocations](../Discourse_Analysis/Collocation_Analysis/Nas_Vas_collocations.tsv)TSV files.
- Top 5 collocations with high logDice score:
    -  Država (Our country): Higest logDice score, score of over 10, suggesting almost formulaic association for parliamentary speech. "Naša država" also carries a connotation of national pride, and denotes important political identity building block (Norms and Values). The collocation is used in various context, from neutral statements (e.g. "V naši državi imamo tri univerze, ki so dejansko z vidika financiranja, z vidika ustanoviteljstva in z vidika tudi načina upravljanja državne univerze."), to explicit identity-signaling (e.g. "Žal s predlogom zakona, ki bi pomagal najrevnejšim prebivalcem naše države, nismo uspeli. / "Unfortunately, we have not succeeded in passing a bill that would help the poorest residents of our country.").
    - Mnenje (Our opinion): Relatively strong logDice score, denoting a firm association. The collocation "naše mnenje" is relatively strong, and is also part of the phrase "po našem mnenju", which is the more common form, present in the results. 
    - Poslanski (Our deputy/parliamentary (group)): "V naši poslanski (skupini)": High no. of the collocation frequencies and high logDice denote the strong association in the phrase. 
    - Ocena (Our assesment): "(Po) naši oceni"/"Naša ocena" (je)" serves a similar function as "naše mnenje" - expressing distinct opinion, however the identity of the speaker (who is "us"?/"naš") is not explicitly clear from the speech.
    - Družba (Our society): the collocation "Naša družba" relates to the notion of society, and serves a similar function as "naša država". However, while "država" can still to some degree relate to neutral statements, the "naša država" signals distinct connotation of our common value and identity (e.g."Izobraževanje kot ključna vrednota v naši družbi ostaja javno dobro. / Education remains a public good as a key value in our society.").
- Additionally, there are other collocations, that are strong in association and relate to specific political identity building blocks (as well as conveying this through the use of virtue signalling), where the category “norms and values” seem to be very strongly present.
    -  Country/People/Social constructs-related collocations: država (country), domovina (homeland), (državljan, državljanka (citizen) – also related to človek (people)) 
-  *Detected dual function of "Naš" (vlada, medij, otroci...)*: on one hand it refers to the common values/virtues (people, country, future) to one hand position the speaker (and by extension their party/parliamentary group or other forms of membership) as the defenders of those values, evoking feeling of empathy (example). On the other hand utilising the same collocates to attack the opposing side, by using these values to underline the (negative) opposing side’s actions that will/has/had (negative) consequences for these values (e.g. Vi pa tudi premislite ali se splača uničevati prihodnost naših otrok, kakorkoli želite) as well as deflection. This function also relates to other expressions of (political) power and activities, e.g. medij ("Kako boste zaustavili to agonijo hrbtenice naših medijev, kar STA je?"), vlada ("O priporočilih Računskega sodišča pa ne bomo glasovali, ker ni potrebe, ker je ta naša vlada tako dobra, da teh priporočil ne rabi"), politika ("To ni zraven naše politike, naše ideologije").

Additional collocations outside the range that do carry specific PI connotations (but within logDice score ≥ 5)

- “medij” (our media): mostly relate to the media landscape in the country, and mostly relate to the very negative image (non-objectivity, hiding of information) of the media state. However, this is also to some degree a political strategy (e.g. “To, da ropajo, da požigajo, da uničujejo, da posiljujejo, to naši mediji skrivajo.”/ “The fact that they rob, burn, destroy, and rape is hidden by our media.”; “Ko berem v kakšnem tujem mediju – ker naši mediji ne upajo napisati krute resnice.”/ “[..] I read about it in foreign media—because our media don't dare to write the cruel truth”).
- “sosed” (our neighbours):  A collocation mostly associated with the national identity of Them, specifically, neighbouring countries (e.g. “Na senčni strani Alp pri naših sosedih, Avstrijci – [...]”). It can, of course, refer to actual neighbours. A directly related collocation with a stronger negative connotation is “Naš južni (sosed/naša južna soseda/meja/...)”, which usually refers explicitly to Croatia (and its border), or to the countries or people of the former Yugoslavia, mostly in a negative context, often relating to migration issues and the protection of the southern border.
    - *Here, the dual nature of the function of »Naš« is expressed. »Naš/a sosed/a« can be used either to neutrally denote one of the neighbouring countries or, more commonly, to refer to a negative outlook or the common expression of »Them«, effectively assuming the role of »Vaš«. This is also seen in other instances, for example, »naša vlada« (our government; when expressing dissatisfaction or criticism directed towards the current government in power), »naši mediji« (our media), »naša zakonodaja« (our legislation), and so on.*
- “stran” (our side): Refers mostly to a parliamentary group, party, coalition, or opposition, usually indicating support for or lack of support for proposals from “the other side”. However, it can also denote political or ideological positioning. Additionally, it may refer to various other concepts without inherit political connotation (e.g. “ceste na naši strani (meje, države)” / “roads on our side (borders, countries)”, “naša stran Trojan” / “our side of Trojane”).
- Naša politika/naši politiki/… → Can refer to either politics in general (e.g. Slovenian politics, “skrajni čas, da **naša** politika stopi v korak s časom”), specific politicians (our politicians from our Party/PG), internal politics (Our politics relate to the…, e.g. “To ni zraven **naše** politike, naše ideologije”)
- Additional collocations outside top 20 that have explicit relation to Aims category (as a dominant PI reference): cilj, namen, interes, zahteva, pobuda, želja, prizadevanja

## Vaš collocations
- Top 5 collocations with high logDice score:
    - “Vaš odgovor” (Your answer): The collocation with the highest logDice is (vaš) odgovor does not exceed 10, suggesting that while the association between “vaš” and  “odgovor” is high, it is not formulaic or fixed phrase. However, it is often used to express typical polite phrase “Hvala za vaš odgovor”, though not exclusively, and can in addition to prompting a speaker to give an answer can also function as indirect form of attack (e.g. "V vašem odgovoru nisem zaznal neke jasne opredelitve in stališča do tega."; "Prosim, če mi daste konkreten odgovor na konkretno vprašanje, kajti enačenje in posploševanje vaših odgovorov,[...]"). 
    - “Vašo pozornost” (Your attention): If both previous collocations serve dual function, this is not the case for “pozornost”, which is almost exclusively used to thank the audience for their attention (“Hvala za vašo pozornost).
    - "Vaše ministrstvo" (Your Ministry): Still high in association, and first collocation in the list that serves as direct form of attack to criticise the work of the Ministry (and by extension, a particular coalition party/speaker etc).
    - “Vaša stran” (Your side): Can refer directly to a particular party/parliamentary group (from the opposing side), ideological positioning (e.g. "Na vaši strani so pa nekateri taki, ki jim samostojnost in neodvisnost Slovenije nista intimna opcija. ") or speaker ("Spoštovani gospod Vrtovec, ko je bilo tudi iz vaše strani rečeno, da [...]").  
    - “Vaše mnenje” (Your opinion): Questions, relating to the opinion of the MP/Minister ("Spoštovani minister, zato me zanima vaše mnenje: […]") during MP questions, or use it as political strategy to delegitimize and frame the opposing side viewpoint as subjective (" Takih informacij, veste, jaz slišim vsak dan sto, torej bi po vašem mnenju moral vsak dan napisati sto kazenskih prijav"). Similar functions can be seen in collocations such as: izjava, trditev, odločitev, stališče, argument, pobuda, … all activities (from the opposing side) which serve as an (in)direct form of attack (and refering either to speaker/party/group/coalition/opposition.
- Collocates in the "vaš" list mostly relate to the opposing side and functions as a direct attack and blame shifting.

Additional collocations of interest/observations:

- Many adjectives: poslanski (skupina, vprašanje, kolega), strankarski (kolegi, interesi, trobila), koalicijski (poslanci, kolegi, vlada, pogodba), ministrski (kolega, ekipa, kandidat, kolegi): very similar function to “vaše ministrtsvo”; i.e. the object of attack (of the opposing side), though here the role is explicitly given (stranskarski = political party, poslanski = parliamentary group, koalicijski = coalition, ministrski = minister/Ministry)
- Vaši otroci (Your children): In contrast to the expression “naši otroci”, which conveys shared values and collective responsibility for the future (our children as our common future), this collocation mainly serves to highlight a bleak or uncertain future projected onto the opposing side as a direct consequence of their actions, or as a broader warning about the potential impact of such actions on future generations.
- Additional Aims PI category (Dominant): namen (intent), interes (interest), vladavina (ruling/reign), vladanje (to rule/to reign), pobuda (inicitative)... which directly describe political gains (or, aims) that the 


## Naš/Vaš collocations

Additional collocations of interest/observations:

- Across all window sizes and pattern restrictions, only a small set of lexemes consistently co-occurred with the naš/vaš pattern. Outside this stable core, the collocation lists contained a large number of low-frequency content words and high-frequency function words. This behaviour indicates that the naš/vaš contrast does not form formulaic multiword expressions but functions as a flexible discursive resource that appears in a wide variety of syntactic and argumentative contexts
    - Stable collocations: deliti, delitev, domovina, lev, desen, razlika, skupen, vaš. Of those the Ideology category is the dominant category of all of them, with the exception of “domovina” (Norms and values)
- **Ideology**: Collocations that clearly denote political polarisation and the phenomenon of “naši in vaši” include collocates such as delitev, deljenje, etc. These refer to both political division and the actual act of dividing people or political actors into “Us” and “Them”. However, given the strong link to ideology and reference to the phenomenon itself, this is more connected to Ideology than to Activity or Discourse. Additionally, the collocate “razlika” is probably the strongest example of division. While deljenje, deliti, and ločevanje often also relate to calls to overcome political or ideological division, “razlika” (difference) explicitly underscores the in-group/out-group concept – highlighting our good qualities and emphasising their bad qualities, while minimising our bad qualities and downplaying their good qualities, for example.:

> *Ampak veste, kaj je razlika med vašo in našo vlado? Razlika je v tem, da je nas zavezovalo fiskalno pravilo, vas pa ne. Razlika med našo in vašo vlado je v tem, da smo mi pustili plus na računu, ko ste vi vlado dobili. Vi ste pa naredili takšen puf, da ga bodo moji in vaši vnuki pa še njihovi vnuki plačevali. To je razlika med vašo in našo vlado.*
>
> *But do you know what the difference is between your government and ours? The difference is that we were bound by fiscal rules, while you were not. The difference between our government and yours is that we left a surplus in the account when you took over the government. You, on the other hand, ran up such a huge debt that my grandchildren, your grandchildren, and even their grandchildren will be paying it off. That is the difference between your government and ours.*
    

## Top 20 Dominant PI categories

| Category | Naš | Vaš |
| --- | --- | --- |
| Membership | 3 (15%) | 1 (5%) |
| Activities/Discourse | 4 (20%) | 8 (40%) |
| Aims | 0 | 0 |
| Norms and values | 11 (55%) | 0 |
| Ideology | 0  | 1 (5%) |
| Group relations | 1 (5%) | 7 (35%) |
| Power resources | 1(5%) | 2 (10%) |
| None | 0 | 1(5%) |

- N: Norms and Values category represents more than 50% of the collocations on the list (11, 55%), followed by Activities/Discourse collocations (4, 20%). There are no Aims or Idology-related collocations among top 20. 
- V: Most representative category: Activities/Discourse (8, 40%), followed by Group relations-related collocations (7, 35%).  In both N and V collocations, there are no words that would carry Aims as dominant PI category.
- NV: Due to many unstable collocations, the PI categorisation for NV collocations cannot be used for comparison with N and V PI dominant categories (are analysed separately). 
- A considerable number of collocates in the subcorpora also have secondary or alternative PI categories, either because they appear in different contexts or because their usage varies. Consequently, a single collocate can signal different relationships or PI-building functions. This also reflects that PI categories can overlap: for example, parliamentary group may indicate an MP’s formal affiliation, but in a given sentence it may function more like a Group resources item, especially when it implies alignment with, or opposition to, entities such as the coalition or the opposition.

| Category | Naš | Vaš |
| --- | --- | --- |
| Membership | *stranka, vlada, stališče* | *stranka*, poslanec, minister, kandidat |
| Activities/Discourse | *mnenje, ocena, amandma, predlog* | *odgovor, mnenje, izjava, trditev, odločitev, predlog, nastop, stališče,* argument |
| Aims | cilj, namen, interes, zahteva, pobuda, želja | namen, interes, zahteva, želja, vladavina, vladanje, pobuda |
| Norms and Values | *država, družba, državljan, skupen, državljanka, gospodarstvo, otrok, prepričanje, človek, praven, zakonodaja,*    nacionalen, ozemlje, narod, kmet, odgovornost | otroci |
| Ideology | vaš, stran | *predsednik*, vaš (repetition), naš |
| Group relations | *vlada*, koalicijski, sosedje | *ministrstvo*, *stran*, *predhodnik, koalicijski, vlada, političen, kolega,* |
| Power resources | *ustava*, medij, moč, volivec | *mandat, resor*, volivec |
| None | / | *pozornost* |

**Analysis**
- **Naš PI categories**: The top 20 N collocations most frequently refer to the Norms and Values PI category, followed by Activities/Discourse. However, within this range, there are no collocations that identify Aims or Ideology as the dominant PI category. This does not mean that such collocations do not exist, but rather that they may be ranked lower (and are indeed present outside the top 20), which is the case for the Aims category.
    - The abundant presence of Norms and Values-related collocations indicates that, for "our" side, norms and common virtues are extremely important and can be used to highlight the good work of our group (such as our good care for our people, homeland, etc.), while also contrasting these norms and values to criticise the opposing side (Them) and emphasise their poorly considered actions or negative traits.
    - The fact that Aims-related collocations fall outside the top 20 may also suggest that these aims (often the result of discursive acts such as assessments or statements) are a secondary aspect of "our" speech patterns. They are used to defend our own actions and explain the benevolent or honourable intentions of our side (e.g. "Zdi se mi pomembno, ko govorimo o tej noveli, da se poslušamo, da prisluhnemo ministrstvu, stroki in na drugi strani tudi vidim pa slišim naše želje tukaj.") or to attack the opposing side. 
    - Additionally, most of the same collocations appear in both N and V, with the function of the collocation changing according to the pronoun used ("naša želja" / our wish → positive, indicating good intentions within our side; "vaša želja" / your wish → negative, indicating negative aims attributed to the opposing side).
- **Vaš PI categories**: The top 20 V collocations fall mainly under the Activities/Discourse PI category, followed closely by Group relations. In this range, there are no collocations indicating a relation to the Aims or Norms and Values PI categories. Additionally, one particular collocation (Pozornost) does not relate to any PI category; it appears only in the polite phrase "Hvala za vašo pozornost" ("Thank you for your attention"), which was the sole usage found in the manual review.
    - Collocations in the Activities/Discourse category are used to highlight the actions of the opposing side as a point of blame, or to frame responsibility, caution, or criticism regarding decisions made by the opposing side. 
    - Collocations in the Group relations category refer to various political groups – most often political opponents rather than allies – such as the government, the coalition, or the opposition. They are used to assign blame, criticise current or previous governments or parties, or imply that a subject belongs to a particular political camp. These expressions also reference shared political allies and often suggest that the opposing side benefits from the support or authority of these allies.
    - The collocations in the two most prominent categories are often interconnected: one denotes the activity or behaviour of the opposing side, while the other identifies the explicit or implicit political group being blamed or targeted.
- **Naš_Vaš (NV) PI categories**: There are only a few stable collocations, with a long tail of low-frequency collocates or function words. (Semi-)stable collocations include deliti (to divide), delitev (division), domovina (homeland), lev (left), desen (right), razlika (difference), skupen (common), and vaš (yours). Among these, the Ideology category is dominant for all except “domovina” (Norms and values).
- In both N and V collocations, there are no words that would carry Aims as dominant PI category.
- A fair share of collocates in subcorpora also have secondary/alternative PI categories, either to difference context or use of the collocate, or can denote different relations (and signal different PI building characteristics).


# Keyword Analysis

## Methodology

Parameter setting:
 - Scenario 1: Focus subcorpus: Naš, reference corpus: ParlaMint-SI 5.1, Reference subcorpus: Vaš
 - Scenario 2: Focus subcorpus: Naš_Vaš, reference corpus: Vaš, Reference subcorpus: Naš
 - Attribute: lemma (lowercase), only alphanumeric values
 - Smoothness parameter (N=20)

The focal metric that that was used to evaluate the most representative keywords for specific focus sobcorpus in relation to the reference subcorpus is based on the simple maths calculation (Score) used within within NoSketch Engine. The keyness score is used to identify keywords, terms, and key n-grams, typical of the corpus or that represent the corpus best. It compares the (normalized) frequencies in the focus (sub)corpus with the frequencies in the reference (sub)corpus (Kilgariff, 2009, 2015). One of the key elements for calculation is the N smoothing parameter to define words that are typical for (sub)corpus. The default value of the parameter is 1 (N = 1), the higher N value shifts focus on the higher-frequency/more common words, while lower value focusses on the lower-frequency (or rare words). Additionally, the values that reflect the changes in magnitude should follow 0.1, 1, 10, 100, 1000, 10000 etc, as smaller changes rarely produce noticeable effect (Kilgariff, 2009, 2015). 
For our keyword analysis, the smoothing parameter was set to moderate smoothing (N=20) in order to suppress noise from very low-frequency words (lowercase lemmas) while still retaining mid-frequency items, which are relevant to identity-related discourse analysis.
The analysis is limited to two targeted comparisons in order to maintain interpretability and avoid analytical redundancy. First, the naš vs vaš comparison captures the contrast between ingroup and outgroup identity construction, revealing how speakers linguistically differentiate “us” from “you” when each pronoun occurs in isolation. 
 
## Focal subcorpus: Naš, Reference subcorpus: Vaš
Full list of keywords can be found in [Nas_Vas_keywords](../Discourse_Analysis/Keyword_Analysis/Nas_Vas_keywords.tsv) TSV file.

- Five keywords with the highest Score: predlagan (adj. proposed), novela (amendment), dopolnitev (amendment), direktiva (directive), naroden (national). All but the last keyword are related to various parliamentary activities (e.g. proposing an amendment to current legislation) and actions undertaken by MPs. This trend is also evident throughout the list of keywords.
In addition, there are several keywords referencing speakers' parliamentary groups, which include both implicit and  explicit mentions of specific parties (e.g. sab → SAB (SAB party), desus (DeSUS party), demokrat (democrat), skupina (group), poslanski (deputy), klub (club)), as well as their parliamentary role-related memberships (matičen / parent, telo / body (parliamentary body).
- Additionally, many of these words can relate to many different concepts, which is heavily related to the context of the speech. 
    - skupina (group): mostly refers to Poslanska skupina (parliamentary group), also referring to social groups (etnične / ethnic, ranljive / vulnerable, ciljne / target, družbene / social)
    - klub (club): either interest groups (e.g. Alpinistični, študentski, športni klub) or club of regional parliamentary deputies (Klub primorskih/pomurskih/podravskih poslancev) or another way of reffering to parliamentary group (Poslanski klub Liberalne demokracije Slovenije). which were investigated in the collocation analysis.
    - Ljudski (people's) – ljudski jezik (language), ljudska iniciativa (initiative), ljudsko mnenje (opinion), Ljudska republika (People's Republic), ljudska univerza (university)

Overall, there are not many words that reveal specific themes in these speeches, nor are there any strongly sentiment-laden words, which were detected in the other comparison. This is understandable, as the speeches would at most emphasise their work with words related to their activities (Predlagane rešitve bodo po našem mnenju prispevale k izboljšanju tudi demografske slike/ In our opinion, the proposed solutions will also contribute to improving the demographic picture.), or use these to defend their work, which are basic discursive functions of MPs on both “sides”.


## Focal subcorpus: Vaš, Reference subcorpus: Naš
Full list of keywords can be found in [Vas_Nas_keywords](../Discourse_Analysis/Keyword_Analysis/Vas_Nas_keywords.tsv) TSV file.

While the previous scenario gives relatively generic words, associated with the MP/parliamentary activities and membership, this is not the case with the keywords of the Vaš focus corpus, where the representative lemmas are much more charged in terms of sentiment.
- Five keywords with the highest Score: vaš (yours), ti (you), zanimati (interest), prositi (to ask), odgovor (answer)
    - First two lemmas with the highest scores are “vaš” which was expected, given the contents within the Vaš subcorpus and the nature of the speeches, and the “ti” lemma, which refers to different pronoun forms of “You” (e.g. vi, vam, vas, vami).
    - The next few lemmas do outline the classic parliamentary activities (e.g. prositi (to ask, verb), odgovor/answer, odgovoriti (answer, verb)
- The list includes many explicitly or contextually negative keywords, as well as politically charged keywords, which serve as attacks on the opposing side.    - Many negative lemmas, which function as an attack of the opposite side:
        - Verbs: zavajati(to lead on), očitati (to blame), odstopiti (to resign), lagati (lie), žaliti (to insult), oprostiti (to forgive/excuse), hvaliti (to praise/boast), sprenevedati (evade), kadrovati (to recruit), izjaviti (to express) …
        - Nouns: interpelacija (interpelation), magnetogram, laž (lie), izjava (statement), obtožba (accusation), ovadba (indictment), protest, neresnica (falsehood, untruth - lie), norec (lunatic), tožilstvo (prosecution), neumnost (stupidity)...    
        - Adjectives; proceduralen (procedural), levičar (left), koalicijski (coalition), ministrsko (ministerial) ...)
    - Keywords that denote specific themes: Covid-related lemmas (Maska, ventilator), rtv (media landscape, financing of the biggest public media house), arhiv -> odprtje gradiv arhivov (referendum)
    - Surnames/names of MPs (janša, grims, gorenak, tanko, janez, vizjak, klemenčič, erjavec, möderndorfer), which are the names of the MPs being adressed/mentioned (and often the target of attack)
    - Reference to specific parliamentary groups/parties (sd), reference to specific speaker and their roles (minister, ministrica, gospod), 
    - Figurative use of certain lemma (usta -> “polna usta so vas”, also “živeti iz rok v usta”, “iz ust vaših …” “zapiranje ust”) 
- The list includes keywords that inherently carry (lexical) negative sentiment (e.g. zavajati, laž), as well as lexically neutral (or even positive) words that are used in a negative context (e.g. hvaliti (to praise): "To so posledice takšne politike, smrti. [...]. In vi se hvalite s politiko" / "These are the consequences of such policies, death. [...]. And you praise/boast about your policies"), though they are rarer.

















