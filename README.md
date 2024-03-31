# Corpws-Brawddegau-Tagiedig

[![DOI](https://zenodo.org/badge/308364293.svg)](https://zenodo.org/badge/latestdoi/308364293)

(see *Corpus of Tagged Sentences* below for English)

Dyma gorpws cychwynnol o frawddegau CC0 Cymraeg mewn fformat jsonl, gyda rhannau ymadrodd y tocynnau (geiriau etc.) wedi'u tagio â thagiau Universal Dependencies.

Fersiwn alffa o'r corpws yw hwn - bydd yn cynyddu o ran ei faint ac yn gwella o ran ei gywirdeb wrth i broject Iriaith fynd yn ei flaen.

Pwrpas y corpws hwn yw galluogi hyfforddi tagiwr ystadegol Cymraeg ar sail dulliau dysgu peirianyddol.

Ar hyn o bryd mae'n cynnwys 79,442 o 'frawddegau' hyfforddi tagiedig, sef 3,345 brawddeg unigryw gyflawn ac 76,097 o eiriau unigol er mwyn atgyfnerthu geirfa'r model (1% yn fwy cywir). Mae metadata pob brawddeg yn glwm wrth ei gofnod jsonl.

Mae'r data yn cynnwys brawddegau cyffredinol a awdurwyd gan aelodau'r Uned, yn ogystal â sgyrsiau ar-lein, cyfieithiadau o straeon ac erthyglau newyddiadurol CC0, trydariadau ac erthyglau gwyddoniadurol a gyfranwyd gan eu hawduron o dan drwydded CC0.

Ym mis Gorffennaf 2022 ychwanegwyd 9,109 brawddeg tagiedig ychwanegol yn y ffeil `brawddegau_tagiedig_cc0_covost_ltu.jsonl`. Mae'r brawddegau hyn yn gyfieithiadau i'r Gymraeg gan Facebook o frawddegau Saesneg Common Voice fel rhan o CoVOST2 (https://ai.facebook.com/blog/covost-v2-expanding-the-largest-most-diverse-multilingual-speech-to-text-translation-data-set/). Yn dilyn archwiliad ieithyddol, barnwyd gan ein ieithyddion eu bod o safon digonol i'w cynnwys yma.  

Ym Mawrth 2024 ychwanegwyd detholiad o'r brawddegau byr mwyaf cyffredin yn y Gymraeg.

Gyda'r data 79k brawddeg cynnar, rydym eisioes wedi llwyddo i hyfforddi tagiwr cychwynnol gyda chywirdeb o dros **91%** ar destun a gasglwyd ar hap ac nad oedd yn y data hyfforddi.

Mae model parod y tagiwr hwnnw ar gael yma:

https://github.com/techiaith/model-tagiwr-spacy-cy

Bwriadwyd y ffeil o frawddegau tagiedig hon ar gyfer ei ddefnyddio gyd spaCy, un o'r llyfrgelloedd NLP cyfoes amlycaf.

I ddefnyddio'r data i hyfforddi model spaCy, yn gyntaf defnyddiwch y gorchymyn `convert` i drosi'r ffeil:

https://spacy.io/api/cli#convert

Yna defnyddiwch y gorchymyn `train` i hyfforddi'r model:

https://spacy.io/api/cli#train

Ar hyn o bryd, bydd angen i chi osod ffolder iaith `lang` Cymraeg yn spaCy i hyn weithio. Mae ffolder ddrafft a chyfarwyddiadau ar sut i'w osod yn spaCy ar gael gennym yma:

https://github.com/techiaith/spacy-cy-lang

Byddwn yn cyfrannu'r ffeiliau hyn i spaCy yn y dyfodol agos er mwyn gwneud i ffwrdd â'r angen am y cam hwnnw.

Ariannwyd y gwaith hwn gan Lywodraeth Cymru.

# Corpus of Tagged Sentences


This is an initial release of a corpus of Welsh CC0 sentences that have been tagged with Universal Dependency part-of-speech tags and saved in jsonl format.

As this is an alpha version of the corpus,  it will increase in size and accuracy as the Iriaith project progresses.

The purpose of this corpus is to enable the creation of statistical Welsh part-of-speech taggers based on machine learning methods.

The corpus currently contains 79,442 tagged training 'sentences', comprising of 3,345 complete unique sentences and 76,097 single word sentences included to boost the trained model's vocabulary (increases accuracy by 1%). The metadata for each sentence is included in the jsonl entry.

The data includes general sentences authored by the Unit's staff as well as online chats, translated CC0 stories and newspaper articles, and tweets, encylopeadic articles provided to us by their authors under a CC0 licence.

In July 2022, an additional 9,109 tagged sentences were added in the file `brawddegau_tagiedig_cc0_covost_ltu.jsonl`. These sentences are translations into Welsh by Facebook of English sentences from Common Voice which form part of of CoVOST2 (https://ai.facebook.com/blog/covost-v2-expanding-the-largest-most-diverse-multilingual -speech-to-text-translation-data-set/). Following a linguistic examination, our linguists judged that they were of a sufficient standard to be included here.

In March 2024 a selection of the most common short sentences in Welsh was added.

Using the early 79k sentence data, we have already succeeded in training a model with over **91%** accuracy on randomly selected texts that were not part of the training data.

That pretrained model is available here:

https://github.com/techiaith/model-tagiwr-spacy-cy

This file of training sentences was intended for use with spaCy, one of the foremost modern NLP libraries.

To use the data to train a spaCy model, first use the `convert` command to convert the file:

https://spacy.io/api/cli#convert

Then use the `train` command to train the model:

https://spacy.io/api/cli#train

Currently, you will need to install a Welsh `lang` folder in spaCy for this to work. We've provided a draft folder and installation instructions here:

https://github.com/techiaith/spacy-cy-lang

We will be contribuiting these files to spaCy in the near future so that this step will no longer be required.

This work was funded by the Welsh Government.
