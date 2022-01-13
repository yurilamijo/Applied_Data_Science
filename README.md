# Portfolio Applied Data Science
Name: Yuri Lamijo<br/>
Studentnumber: 18050697<br/>
Course: Minor Applied Data Science

# Project Emo
_Project Emo is in staat gesteld door de heer Hani Al-Ers die werkzaam is bij een Lectoraat van De Haagse Hogeschool._

Project Teddy is in deze minor opgesplits in drie verschillende projecten. Deze projecten zijn project Nurish, Dialog en Emo. Beide project hebben te maken met het classificeren van kenmerken in audio.
<br/><br/>

## Task Definition
Het doel van project Emo is het herkennen van emoties uit spraak audio van ouderen met dementie. Zorgverleners kunnen hiermee de quality of Life van een ouder in kaart brengen. Verder kunnen ze sneller actie ondernemen wanneer de quality of life van een ouder verslechterd.

Gebaseerd op het probleemstelling, project domein, feedback van de docenten en de product owner is de volgende hoofdvraag opgestelt.
> Which machine learning models achieve the highest precision classifying emotions, using (four) datasets containing audio with labeled vocal emotional expressions recorded in a professional recording studio, in order to recognize emotions within household environments?

Vanuit deze hoofdvraag zijn de volgende sub onderzoekvragen opgesteld.
> Which machine learning algorithms are available in literature to classify emotions from audio? 

> How can precision in machine learning algorithms be improved for the TESS, SAVEE, RAVDESS and CREMA-D datasets?

> Can the known methods of classifying be reproduced with the same precision/recall on the available dataset?

<br/>

## Planning
Het project team was bij de kick off van de minor geadviseerd om de werkzaamheden uit te voeren en te planning in de Agile techniek. Hierom hebben wij unaniem gekozen om SCRUM toe te passen. Vier van de project leden waaronder ik waren al bekend SCUM. Waardoor wij de andere 2 project leden konden ondersteunen met het SCRUM process. Verder had het team besloten om een vaste SCRUM master rol toe tewijzen. Deze rol had ik vervuld.

Sprints tot sprint 3 duurde een week. Dit liep echter niet zoals verwacht. De user stories die uitgevoerd werden, moesten vaak mee genomen worden omdat deze nog niet af was of omdat deze net te groot was. Hierom hadden wij er voor gekozen om sprints te houden van 2 weken. Aan het eind van iedere sprint werd er met het team een retrospective gehouden die daarna gevolgd werd door een sprint planning voor de volgende sprint.
<br/>

<details>
<summary>Project plan - Miro</summary>
In sprint 3, hadden wij een Miro timeline board gemaakt. Daarin werd de werkzaamheden (user stories) en potentiele werkzaamheden zichtbaar gemaakt. Hierdoor konden wij een globale planning maken voor de gehele minor en het project. Dit timeline board heeft naar mijn mening veel geholden bij het beslissen en prioriseren van welke user stories bepaalde sprints uitgevoerd moeten worden.

zichtbaar gemaakt welke werkzaamheden in bepaalde sprint uitgevoerd werden.

![Miro timeline planning](https://gcdn.pbrd.co/images/id0k4ReDnCfR.jpg?o=1)
_Figuur 1 - Miro timeline planning_

---
</details>
<details>
<summary>Github - SCRUM</summary>
Als groep besloten we om het project board van Github te gebruiken als ons SCRUM board. De User Stories en Epics werden toegepast door middel van het aanmaken van issues. Het SCRUM board werd verdeeld in 4 secties: <b>To do</b>, <b>In progress</b>, <b>Waiting for feedback</b> and <b>Done</b>

Ik was verantwoordelijk voor het opstellen van de user stories. Aan het einde van elke sprint hielden we een sprint planning. In deze planning keken we naar ons Miro bord en bepaalden we welke taak uitgevoerd moest worden. 
![Sprint 8 backlog](https://gcdn.pbrd.co/images/zaFEIkf5La2M.png?o=1)
_Figuur 2 - Sprint 8 backlog_

![Uitgevoerde user stories 1](https://github.com/yurilamijo/Applied_Data_Science/blob/main/afbeeldingen/user_stories-1.png)

![Uitgevoerde user stories 2](https://github.com/yurilamijo/Applied_Data_Science/blob/main/afbeeldingen/user_stories-2.png)

![Uitgevoerde user stories 3](https://github.com/yurilamijo/Applied_Data_Science/blob/main/afbeeldingen/user_stories-3.png)

---
</details>
<details><summary>Daily stand-up/ Retrospective</summary>
<b>Daily standup</b><br />
In de daily standup, vertelde we wat voor werkzaamheden uitvoerd waren, knelpunten die voorkwamen en welke werkzaamheden we van plan zijn uit te voeren. Hierdoor wist het team exact wie welke werkzaamheden uitvoerde of mogelijk hulp nodig heeft.
<br /><br />

<b>Retrospective </b><br />

Voor iedere retrospective is er een afbeelding geexpoteerd, zodat alle geschreven tickets en actiepunten terug gevonden kon worden. De afbeeldingen kunnen terug gevonden worden in de wiki pagina [Retrospective](https://github.com/koendebruijn/Emotions/wiki/Retrospective) in de [Emotions GitHub repositorie](https://github.com/koendebruijn/Emotions).  

---
</details>
<br />

## Evaluation
We hebben een CNN kunnen opleveren die angry, sad, happy en neural emoties kunnen herkennen. Maar voor dit model is er zeker nog ruimte voor verbetering. Een van de eerste verbetering die toegepast kan worden is het optimaliseren van de hyperparameters. Dit hebben wij voor de CNN helaas niet kunnen uitvoeren wegen het gebrek van tijd. De tweede verbetering die toegepast kan worden is door over-sampling toe te passen op de neutrale audio fragmenten hier door verhogen we de precision voor neutral samples. Als gevolg hiervan is dat de model nu alleen met meer zekerheid kan zeggen dat het een bepaalde emotie is. Verder kan er gekeken worden om meerdere datasets toe te voegen aan de huidige dataset. De datasets die toegevoegd kunnen worden zijn: eNTERFACE, EMO-DB, DES en SUSAS.

Naast deze verbeteringen kan er ook gekeken worden naar een mogelijke andere methodes voor het classificeren van emoties. Een van deze methodes is het groeperen van emoties in groepen van positive, negative en neutral. Dit kan handig zijn in situaties waarbij de eindgebruiker alleen wilt weten dat er een emotie aanwezig was en welke dit mogelijk kan zijn. Maar om deze methode te kunnen uitvoeren adviseren we wel om de groeperingen te bespreken met professionnels binnen het vakgebied van emoties.

Een van de belangrijkste toekomstige aanpasingen die toegepast moet worden is het evalueren van het model met audio fragmenten van ouderen met dementie en het trainen van het model met deze data. Pas nadat deze stap is uitgevoerd weet de opdrachtgever zeker of het mogelijk is om accuraat emoties te kunnen herkennen bij ouderen met dementie.

<br />

## Conclusion
Om onze hoofdvraag te kunnen beantwoorden is er gebriuik gemaakt van een gecombineerde dataset dat bestaat uit vier datasets. Deze datasets zijn: RAVDESS, CREMA-D, SAVEE en TESS. Voor de machine learning modellen is er gebruik gemaakt van KNN, SVM en Logistic Regression. Deze resultaten zijn in dit [excel](https://github.com/yurilamijo/Applied_Data_Science/blob/main/excel/Evaluation%20precision%2024-11-2021.xlsx) te vinden. Bij deze resultaten is ook het MLP model opgenomen. Omdat de resultaten van deze models matig waren, hadden wij besloten om onze focus te leggen op oplossing die gebruik maakt van een CNN. Dit was omdat wij tijdens de literatuur onderzoek een goeie paper hadden gevonden die gebruikt maakte van een CNN die veelbelovende resultaten aantoonde. Omdat wij in het midden van de minor overgestapt waren van ML models naar een CNN hadden we niet alle optimalisaties kunnen toepassen op de CNN die we wel op de ML models hadden toegepast en dat is jammer. Er is daarom voor de CNN zeker nog ruimte voor verbetering. De CNN die opgezet is kan de emoties angry, sad, neutral en happy met huisomgevingsgeluiden herkenen met een precisie van 80% en zonder huisomgevingsgeluiden 84%. Dit zijn geen slechte precentages, maar zoals ik eerder had benoemd kan de CNN nog verbeterd worden dat kan leiden to betere resultaten

<br />

# Communication
<details>
<summary>Discord</summary>
Het team had aan het begin van het project afgesproken om all communicatie over het project via Discord te doen. In Discord hadden we hiervoor een aparte discord server gemaakt voor alle project emo leden. Hierin werden relevanten documenten, websites en video tutorials met elkaar gedeeld. Verder werden hier ook de daily stand-ups, retrospectives, sprint planningen en andere meetings gehouden.
<br /><br />
Omdat het Smart Teddy Bear project uit drie verschillende projecten bestaat en ook te maken had met het clasificeren van audio. Hadden wij het initiatief genomen om een discord server op te zetten met daarin alle project groepen gerelateerd op het Smart Teddy Bear project. Hierin kon iedereen relevante research papers en resulten met elkaar delen.

---
</details>
<details>
<summary>Google Drive</summary>
Om tegelijk met het team te werken aan documenten werd er gebruik gemaakt van Google Drive. Hierin maakten wij de presentaties voor de interne, externe en product owner meetings. 

---
</details>
<br />

## Presentations
Tijdens het project werden er presentaties gegeven in de interne, externe en product owner meetings. Deze presentaties werden samen met het team ingedeeld en opgezet. De Interne presentaties werden begeleid door Jaap en ondersteund door de rest van het team.
Voor de externe presentaties hadden we besloten om deze te houden met maximaal 4 verschillende team leden. De taak verdeling voor deze presentaties werd tijdens het opzet van een presentatie uitgevoerd.
De product owner presentaties werd door Berno begeleid met ondersteuning van het team om vragen te kunnen beantwoorden.

Mijn bijdragen bij het maken presentatie was het vullen van de presentatie met resultaten en de machine learning modellen en CNN.
Verder controleerde ik de presentaties of feedback punten van vorig presentaties verbeterd waren in het nieuwe presentatie.
<br />
Presentaties heb ik zelf niet individuele uitgevoerd. Deze werden altijd in team verband uitgevoerd. Ik heb echter zelf alleen specifieke delen van presentaties gepresenteerd. De presentaties waarin ik onderdelen heb gepresenteerd heb ik onderin in een lijst benoemd.

The presentations with the product owner were held by Breno
* Internal presentations were I take part of
    * [Internal Presentation 4](https://github.com/yurilamijo/Applied_Data_Science/blob/main/presentaties/Interne%20presentatie%20week%204.pdf)
    * [Internal Presentation 8](https://github.com/yurilamijo/Applied_Data_Science/blob/main/presentaties/Interne%20presentatie%20week%208.pdf)
    * [Internal Presentation 10](https://github.com/yurilamijo/Applied_Data_Science/blob/main/presentaties/Interne%20presentatie%20week%2010.pdf)
* External presentations were I take part of
    * [External Presentation 1](https://github.com/yurilamijo/Applied_Data_Science/blob/main/presentaties/External%20Presentation%201%20-%20team%20emo.pptx.pdf)
    * [External Presentation 3](https://github.com/yurilamijo/Applied_Data_Science/blob/main/presentaties/External%20Presentation%203.pdf)

<br /><br />

# Research Paper
Als team hadden we besloten dat iedereen aan de research paper kon gaan werken.
Het initieel opzet van de research paper werdt gedaan door Breno, Zahir en ik. Wij begonnen eerst met het opzetten van het structuur van de paper. Daarna begonnen we eerst met de Introduction en Background hoofstukken. Nadat alle expirimenten van de CNN uitgevoerd waren en er definitieve resultaten waren sloten Jaap, Koen en Julian aan bij het schrijven van de paper.
<br />
Nadat alle hoodstukken gevuld en af waren, liepen we met ze alle gezamelijk alinea voor alinea na om de inhoud, spelling, grammatica en samenhang te controleren. Hierdoor kon iedereen zijn mening en feedback geven. Waardoor we naar mijn mening een redelijke research paper hebben kunnen opzetten.


Voor de research paper heb ik de volgende delen met feedback en samenwerking van het team geschreven:
* Introductie
* Methodology
    * Architecture
* Results
<br /><br />

# Domain knowledge
Voordat er machine learning models en neural networks ontwikkeld konden worden moest er eerst kennis opgedaan worden over het domein. Hiervoor heb ik literatuur onderzoek naar relevante onderzoeken en projecten die emoties classificeren uit audio. Verder kregen we ook documenten van onze product owner, zodat we ons konden inlezen op het domein en het Smart Teddy Bear project.
<br /><br />

## Introduction of the subject field
De Smart Teddy is een therapeutisch partner die ouderen observeert doormiddel van sensoren in de Smart Teddy. De teddy bezit op het moment een aantal basis functionaliteiten zoals het observeren op het hoeveelheid aan plezier op een dag heeft en of ouderen genoeg laang genoeg slapen. Deze infromatie wordt dan in beeld gebracht in een dashboard voor verzorgers. Hiermee wordt er een schatting gemaakt over de Quality of Life van de ouder. Verzorgers kunnen met deze informatie sneller handelen en mogelijk de Quality of Life van een ouder verbeteren.

![Smart Teddy dashboard](https://bigdata-thuas.eu/wp-content/uploads/2017/10/Screenshot-2021-04-10-at-23.32.41-300x161@2x.png)<br />
_Figuur 2 - Smart Teddy dashboard_

<br />
De product owner wilt voor de volgende prototype een aantal functionaliteiten toevoegen aan de teddy. Een van die functionaliteiten is het herkennen van emoties via spraak audio. Met behulp van deze functionaliteiten kan er in het dashboard aangegeven worden hoe vaak bepaalde emoties zijn geuit op een dag. Verzorgers die niet ter plekken zijn kunnen hierdoor een beeld de situatie krijgen zonder er fysiek bij te zijn. 
<br /><br />

## Literature Research
In dit hoofdstuk wordt er in kaart gebracht wat de resultaten waren van literatuur onderzoek.

<details>
<summary>Speech Emotion Detection using IoT based Deep Learning for Health Care
</summary>

Links: [IEEE](https://ieeexplore.ieee.org/abstract/document/9005638/authors#authors), [PDF](https://www.researchgate.net/profile/Sayed-Shah-6/publication/337992475_Speech_Emotion_Detection_using_IoT_based_Deep_Learning_for_Health_Care/links/5df968d392851c8364854a33/Speech-Emotion-Detection-using-IoT-based-Deep-Learning-for-Health-Care.pdf)

Deze research paper stelde een CNN als oplossing voor het classificeren van emoties. Voor het trainen van hun model maakten ze gebruik van de RAVDESS dataset. Verder beschreef deze paper duidelijk welke stappen er waren ondernomen en hoe iedere stap invloed had op de resultaten. Daarom adviseerde ik het team om ook deze paper door te nemen en het te gebruiken als baseline voor onze model en paper.

<b>Data Augmentation</b><br />
Deze paper maakte gebruik van 3 vormen van data augmentatie. Deze waren: Time Stretching, Pitch Shifiting en Dynamic Range Compression. Na het uitvoeren van data augemntatie verbeterde zij de resultaten van de CNN

<b>Results</b><br />
Hun uiteindelijke model resulteerde in 95% voor mannen en 97% voor vrouwen. Zij hebben kunnen aantonen dat het mogelijk is om emoties te kunnen herkennen uit spraak audio met hoge accuractie.

<b>Conclusion</b><br />
De researcher van de paper hebben hoge resultaten behaald, maar er kan echter niet gesproken worden van een model dat zulke resulatten zal krijgen bij realistisch auido.

Het RAVDESS dataset wordt namelijk door profesionele acteuren en actresses in gesproken in een profesionele studio. Verder bestaat de ingesproken audio uit 2 verschillende zinnen. 

---

</details>
<br />

## Explanation of Terminology, jargon and definitions
In dit hoofdstuk worden de gevonden en gebruikten terminologies, jargon en definities van het project uitgelegd.

* Ambient noise -
* Chromagram -
* Convolutional Neural Network -
* Mel-Frequency Cepstral Coefficients (MFCC's) -
* Multilayer perceptron -
* Spectrogram -
* Threshold -
* Transfer Learning -
* Waveform -
* Quality of Life - 
* Zero-crossing rate - 


<br />

# Created models
Voor het project heb ik een Multi Layer Perceptron (MLP) model van start tot eind gemaakt. Daarnaast heb ik ook gewerkt aan de Convolutional Neural Network (CNN) die wij als team hebben opgeleverd.
<br /><br />

## Multi Layer Perceptron (MLP)
source: [towardsdatascience](https://towardsdatascience.com/building-a-speech-emotion-recognizer-using-python-4c1c7c89d713)



[MLP model notebook]()

### Data Preprocessing
De data preprocessing pipeline werdt door de SVM, MLP, KNN en Logistic Regression modellen gebruikt. 

<details>
<summary>Data exploration</summary>
Ik heb voor het model geen taken uitgevoerd dat betrekking had op data exploration. Deze taken waren uitgevoerd door Jaap. Hij had voor de data exploration visualisaties gemaakt van de audio samples die vertaald werden naar waveforms, de balance van de verschillende emoties, de duratie van audio samples en de balance tussen man en vrouw audio samples.

---
</details>

<details>
<summary>Data cleaning</summary>
Data cleaning taken heb ik niet uitgevoerd. Deze werdt gezamelijk uitgevoerd door Jaap en Breno. Deze taak hield om stiltes in audio fragmenten te verwijderen.

---
</details>

<details>
<summary>Data preparation</summary>
De data preparation is voor het grooten deels door mij opgezet. De werkzaamheden die andere teamleden bij de data preparation hebben uitgevoerd werd vaak ook ondersteund door mij.<br />
Voor de SVM, MLP, KNN en Logistic Regression modellen werden de RAVDESS en CREMA-D datasets gebruikt. De RAVDESS dataset bevatte 8 emoties: neutral, happy, sad, angry, calm, fearful, disgust en surprised. De CREMA-D dataste bevatte 6 emoties: neutral, happy, sad, angry, fearful en disgust. Om de resultaten te kunnen vergelijken is ervoor gekozen om de 2 extra emoties (surprised en calm) van de RAVDESS dataset niet te gebruiken.

<br />

Verschillende data preparation processen.
* Originele data met 6 emoties 
* Getrimde data met 6 emoties 
* Geaugmenteerde data
* Gegroupeerde data
* Geslacht gesplite data

<br />
<b>Feature extraction</b><br />
Voor feature extraction is er gebruik gemaakt van de Mel-Frequency Cepstral Coefficients (MFCC's), Zero-crossing rate (ZCR) en chromagram. 


Om deze data bruikbaar te maken voor de MLP model maar ook voor de andere ML models. 

Volgend de tutorial die ik heb gevolgd word de _mean_ berekend van de MFCC's, ZCR en chromagram. Deze data wordt dan in een numpy hstack gezet zodat deze data dan gebruikt kan worden om de model te trainen

```python
def extract_feature(audio, sr, emotion, mfcc=True, chroma=True, mel=True):
    result = np.array([])
    
    if mfcc:
        # Gets the mean of the MFCC
        # Change to 21 bins instead of 40
        mfccs = np.mean(lb.feature.mfcc(y=audio, sr=sr, n_mfcc=40).T, axis=0)
        result = np.hstack((result, mfccs))
    if chroma:
        # Gets the mean of the chromagram
        stft = np.abs(lb.stft(audio))
        chroma = np.mean(lb.feature.chroma_stft(S=stft, sr=sr).T, axis=0)
        result = np.hstack((result, chroma))
    if mel:
        # Gets the mean of the Mel-frequency spectrogram
        mel = np.mean(lb.feature.melspectrogram(audio, sr=sr).T, axis=0)
        result = np.hstack((result, mel))
    
    return (result.tolist(), emotion)
```


<b>Audio augmentatie</b><br />
Voor data verijking is er data augmentatie uitgevoerd. Deze taak heb ik gezamelijk uitgevoerd met Koen en Zahir. De verschillende data augmentaties zijn in individueel en in iedere combinatie gebruikt en getest. De resultaten hiervan zitten in dit [excel bestand](""). Uit de resultaten is gebleken dat het augmenteren van een klein tot middelmatig negatief effect had op de accuracy van het model. 

De volgende data augmentaties zijn toegepast: 
* Change pitch (up and down)
* Change speed (slow and fast)
* Change speed (slow and fast) and pitch (up and down)
* HPSS
* Value augmentation*
* Added distribution noise*

*Deze data augmentaties heb ik uitgewerkt en getest

```python
def augment_audio(row, is_augmented: bool = False):
    audio, sr = lb.load(row["file"], sr=22050)

    extracted_features = []
    augmented_audios = [audio]
    
    if is_augmented:
        # Change pitch down
        augmented_audios.append(Augmenter.change_pitch(audio=audio, sr=sr))

        # Change pitch up
        augmented_audios.append(Augmenter.change_pitch(audio=audio, sr=sr, pitch_type="up"))

        # Change speed slow
        augmented_audios.append(Augmenter.change_speed(audio=audio))
        
        # Change speed fast
        augmented_audios.append(Augmenter.change_speed(audio=audio, speed_change="high"))

        # Change speed & pitch down
        augmented_audios.append(Augmenter.change_speed_and_pitch(audio=audio, sr=sr))  

        # Change speed & pitch up
        augmented_audios.append(Augmenter.change_speed_and_pitch(audio=audio, sr=sr, pitch_type="up"))  

        # Add distribution noise
        augmented_audios.append(Augmenter.add_distribution_noise(audio=audio))
        

    for a in augmented_audios:
        extracted_features.append(extract_feature(a, sr, row["emotion"]))
        
    return extracted_features
```

<br />

<b>Positive, Negative en Neutral groepering</b> <br />
Naast het classificeren van specifieke emoties, zijn er ook modelen getrained op basis van positive negatieve en neutrale emoties. Hierbij wouden we vergelijken of het groeperen van emoties vergelijkbare of zelfs betere resultaten zou behalen inplaats van het individueel classificeren van emoties. Deze taak werdt aan het begin door Zahir uitgevoerd. Nadat Zahir om ondersteuning vroeg sloot ik aan om hem te helpen bij het coderen. De code voor de die in de onderstaande code blok staat is geschreven door Zahir met ondersteuning van mij.

```python
def load_data_in_pos_neg(path, dataset_name:str):
    data = []
    # https://www.paulekman.com/universal-emotions/what-is-surprise/
    positive = ["neutral", "happy", "calm", "suprised"]
    negative = ["sad", "angry", "fearful", "disgust", "suprised"]
    
    for i, file in enumerate(glob.glob(path)):
        file_path = os.path.basename(file)

        emotion = ''
        if dataset_name == "ravdess":
            emotion = RAVDESS_emotion_labels[file_path.split("-")[2]]
            #emotion = RAVDESS_emotion_labels[file_path.split("-")[3]] #turn on for trimmed data
        else:
            emotion = CREMA_D_emotion_labels[file_path.split("_")[2]]
            
        if emotion not in focused_emotion_labels:
            continue
            
        if emotion in positive:
            label = "positive"
        else:
            label = "negative"

        data.append([file, label])
           
    end_time = time.perf_counter()
   
    return pd.DataFrame(data, columns=["file", "emotion"])
```

<br />

<b>Audio splitted by male en female</b><br />
Deze taak van preprocessing is gezamelijk uitgevoerd door Koen en Breno. Bij werdt er gekeken of de resultaten tussen audio van mannen en vrouwen werkelijk van elkaar verschillen zoals de paper *Speech Emotion Detection using IoT based Deep Learning for Health Care* verklaarde. De dataset werd op originele dataset (per emotie) en met de groepeerde (positive negatieve en neutrale) dataset gesplits op geslacht

```python
def load_sex_splitted_files(path:str, dataset_name:str):
    """
        Splits the male and female data into seperat datasets
    """
    female_data = []    
    male_data = []

    for i, file in enumerate(glob.glob(path)):
        file_path = os.path.basename(file)
        
        if dataset_name == "ravdess":
            # Splits RAVDESS sex samples
            parts = file_path.replace('.','-').split("-")
            emotion = RAVDESS_emotion_labels[parts[2]]
            #emotion = RAVDESS_emotion_labels[parts[3]] #turn on for trimmed data
            
            if emotion not in focused_emotion_labels:
                continue
            
            #if int(parts[7])%2 == 0: #turn on for trimmed data
            if int(parts[6])%2 == 0:  #turn on for normal data
                # Female sample
                female_data.append([file, emotion])
            else:
                # Male sample
                male_data.append([file, emotion])
        else:
            # Splits CREMA-D sex samples
            parts = file_path.replace('.','_').split("_")
            emotion = CREMA_D_emotion_labels[parts[2]]
            
            if emotion not in focused_emotion_labels:
                continue
            
            #f int(parts[0].split('-')[1]) in CREMA_D_female_samples: # turn on for trimmed data
            if int(parts[0]) in CREMA_D_female_samples:
                # Female sample
                female_data.append([file, emotion])
            else:
                # Male sample
                male_data.append([file, emotion])
            
            
    female_df = pd.DataFrame(female_data, columns=["file", "emotion"])
    male_df = pd.DataFrame(male_data, columns=["file", "emotion"])
        
    return female_df, male_df
```

[Notebook audio preprocessing]()

---
</details>

<details>
<summary>Data explanation</summary>

<b>CREMA-D</b><br />
De Crowd-sourced Emotional Multimodal Actors Dataset ([CREMA-D](https://github.com/CheyneyComputerScience/CREMA-D)) dataset bestaat uit 7442 audio fragmenten die ingesproken zijn door 91 acteurs. Hiervan zijn er 48 man en 43 vrouw tussen 20 en 74 jaar oud die van verschillende etniciteiten (Afro-Amerikaans, Aziatisch, Kaukasisch, Spaans, en Niet Gespecificeerd) komen. De dataset bevat 12 zinnen die gesproken zijn in 6 verschillende emoties. Deze emoties zijn: Anger, Disgust, Fear, Happy Neutral en Sad.


<b>RAVDESS</b><br />
De Ryerson Audio-Visual Database of Emotional Speech and Song ([RAVDESS](https://zenodo.org/record/1188976)) bestaat uit 7356 spraak en video fragmenten. Wij maken voor dit priject alleen gebruik van de 1440 spraak fragmenten. De samples zijn gesproken door 12 mannelijke stemacteuren en 12 vrouwelijke stemactrices. De dataset bevat 2 zinnen die gesproken zijn in 8 verschillende emoties. De emoties zijn: Anger, Disgust, Fear, Happy, Neutral, Sad, Calm en Suprise.


<b>SAVEE</b><br />
Surrey Audio-Visual Expressed Emotion ([SAVEE](https://www.kaggle.com/barelydedicated/savee-database)) is een dataset van 480 audio samples. De samples zijn gesproken door 4 mannelijke stemacteuren. De dataset bevat 15 zinnen die gesproken zijn in 7 emoties. De emoties zijn: Anger, Disgust, Fear, Happy , Sad, Calm en Suprise.


<b>TESS</b><br />
Toronto emotional speech set ([TESS](https://www.kaggle.com/ejlok1/toronto-emotional-speech-set-tess)) is een dataset van 2800 audio samples. De samples zijn gesproken door 2 vrouwelijke stemactrices. De dataset bevat 200 zinnen die gesproken zijn in 7 emoties. De emoties zijn: Anger, Disgust, Fear, Happy ,Neutral Sad, en Suprise.

---

</details>

<details>
<summary>Data visualization (exploratory)</summary>
Gedurende project ben ik niet bezig geweest met het visualiseren van de datasets.

---

</details>

<br />

### Predictive Analysis

<details>
<summary>Selecting a Model</summary>

Ik heb voor het project een MLP model gemaakt met behulp van de sklearn bibliotheek. Ik heb ervoor gekozen om een MLP model op te zetten omdat ik een tutorial op towardsdatascience had gevonden die gebruik maakte van een MLP classifier voor het herkennen van emoties. Verder kwam ik ook een andere [paper](http://www.gjstx-e.cn/gallery/40-may2021.pdf) tegen die ook MLP model gebruikte voor emotie herkenning.

---

</details>

<details>
<summary>Configuring a Model</summary>
Ik had voor de models die opgezet werden in sklearn een [basemodel]() model gemaakt die iedereen kon gebruiken als ze een model zouden maken. De basemodel bevatte de functionaliteit om verschillende dataset types te kunnen inladen. Zo hoefde we alleen de bestands locatie van de JSON bestand door te geven en deze werden dan ingeladen. Verder had ik ook een evaluatie methode geschreven die de recall, precision, accuracy, classification report en confusion matrix toonde. Hiermee probeerde ik te voorkomen dat andere projectleden geen code zouden schrijven voor dezelfde functionaliteiten. De MLP model maakte eerst gebruikt van deze basemodel. Later in het project was er een notebook gemaakt waarin alle models in een keer uitgevoerd konden worden. Deze werd door Jaap opgezet.

---

</details>

<details>
<summary>Training a Model</summary>
Om de beste model te vinden kunnen met de met de juiste hyperparameters is er gebruikt gemaakt van GridSearchCV om de hyperparameters te optimaliseren.

```python    
    @classmethod
    def grid_search(cls, dataset_name, is_augmented=False):
        # train dataset
        train_dataset = super().read_dataset(dataset_type='train', dataset_name=dataset_name)

        X_train, y_train = [], []
        
        if is_augmented:
            X_train = train_dataset['Augmented']['X']
            y_train = train_dataset['Augmented']['y']
        else:
            X_train = train_dataset['OriginalData']['X']
            y_train = train_dataset['OriginalData']['y']
        
        # GridSearchCV Train accuracy
        param_grid = [
            {
                'activation' : ['logistic', 'tanh', 'relu'],
                'solver' : ['sgd', 'adam'],
                'hidden_layer_sizes': [
                     (100,), (200,), (300,)
                 ],
                'alpha': [0.0001, 0.05],
                'learning_rate': ['constant', 'adaptive'],
#                 'max_iter': [10],
            }
        ]
        
        clf = GridSearchCV(model, param_grid, cv=5, scoring=scoring, n_jobs=5) 
        
        start_time = time.perf_counter()
        clf.fit(X_train, y_train)
        end_time = time.perf_counter()
        
        print(f"Duration fitting: {end_time - start_time:04f}")
        
        print("Best parameters set found on development set:")
        print(clf.best_params_)
        print(clf.best_estimator_)
        print(clf.best_score_)
        
        return clf
```

In de onderstaande code block staan de resultaten die de model heeft kunnen bereiken bij het classificeren van positieve en negatieve emoties bij de CREMA-D dataset.
```
Best parameters set found on development set:
{'activation': 'tanh', 'alpha': 0.0001, 'hidden_layer_sizes': (200,), 'learning_rate': 'adaptive', 'max_iter': 10, 'solver': 'adam'}
MLPClassifier(activation='tanh', hidden_layer_sizes=(200,),
              learning_rate='adaptive', max_iter=10)

Train accuracy is: 0.7275784753363229
Test accuracy is: 0.6888440860215054

Recall: [0.86712598 0.30508475]
Precision: [0.72870141 0.51612903]

Classification Report:
              precision    recall  f1-score   support

    negative       0.73      0.87      0.79      1016
    positive       0.52      0.31      0.38       472

    accuracy                           0.69      1488
   macro avg       0.62      0.59      0.59      1488
weighted avg       0.66      0.69      0.66      1488
```

</details>

<details>
<summary>Evaluating a Model</summary>

De MLP model was geëvalueerd met behulp van Kfold cross validation. Deze code was helaas later in de minor niet meer gebruikt. Dit kwam omdat de modellen niet met hun geoptimaliseerde hyperparameters individueel weer werd geëvalueerd met Cross validation. De code Kfold cross validation is te vinden in deze [notebook](). 
De MLP model is geëvalueerd met de andere modellen die de projectleden hadden gemaakt. Bij deze evaluatie is er gekeken naar de resultaten bij het gebruikt van de RAVDESS en CREMA-D datasets. De TESS en SAVEE datasets zijn hier afwezig omdat deze oas later waren toegevoegd. Helaas was er geen tijd meer met de extra datasets nog een evaluatie uit te voeren voor deze modellen. De evaluatie resultaten is in deze excel bestand terug te vinden.

</details>

<details>
<summary>Visualizing the outcome of a model</summary>
De resultaten van de MLP model werden gevisualiseerd met behulp van de `model_accuracy` functie in de basemodel. Een van de visualisaties die de functie alleen miste is de de learning curve van de model. Dit zou het voor ons makkelijker kunnen maken om te kunnen zien of de model aan het underfitten of overfitten was.
</details>

<br />

# Reflection and Evaluation
<details>
<summary>Persoonlijke leerdoelen evaluatie</summary>

<b>Situatie</b><br />
Als Software Engineering student was ik erg enthousiast over de minor. Ik had voor de minor al veel gelezen de resultaten en potentie van data science. Alleen wist ik niet waar ik zou moeten beginnen met het leren van het vakgebied. Hierom had ik ervoor gekozen om de minor Apllied Data Science te volgen. Zodat ik opzet en het proces van data science zou kunnen begrijpen en om deze in de praktijk te beoefenen. 

<b>Taak</b><br />
Voor de minor had ik een aantal leerdoelen voor mezelf opgesteld die ik aan het eind van de minor wilde beheersen. De leerdoelen die ik voor mezelf opgesteld had zijn de volgende:

* Ik wilde leren welke vormen van machine learning models en neural networks er zijn.
* Ik wilde leren hoe ik een machine learning model en/of een neural network train.
* Ik wilde leren hoe ik data van een getrainde machine learning model kan visualiseren.
* Ik wilde leren hoe het proces van data science van begin tot eind inelkaar zit.

<b>Actie</b><br />
Om de opgestelde leerdoelen te behalen heb ik de volgende acties ondernomen:

Om te leren welke vormen van ML models en neural networks er zijn heb wou ik de Datacamp cursussen voltooien en de lectures van de minor volgen. Verder wilde ik met de opgenomen kennis meer onderzoek doen over de modelen en mogelijke nieuwe modellen die niet in de lectures voor komen.

Om te leren hoe ik een machine learning model en/of een neural network kan trainen. Wilde ik de Datacamp cursussen voltooien en de lectures van de minor bij wonen. Hierna wilde ik zelf proberen om de resultaten van de cursussen en lectures na te bootsen.

Om te leren hoe ik data van getrainde models kan visualiseren wilde ik de lecture van Tony Andioli over data visualizatie bijwonen. De kennis die ik bij deze lecture dan heb opgenomen wilde ik kan toepassen op het project.

<b>Resultaat</b><br />
Tijdens de minor heb ik me best gedaan om mijn opgestelde leerdoel te behalen. Zo heb ik tijdens de minor kennis opgedaan over welke vormen van ML models en neural networks er zijn. Deze kennis heb ik opgedaan door het volgen van de Datacamp cursussen en de lectures van de minor. Verder heb ik meerder ML models kunnen trainen in Datacamp en eigen test project. Zo heb ik een SVM  model gemaakt in Datacamp en een MLP model voor het project. De resultaten die daaruit kwamen heb ik daarna kunnen visualiseren.

Door het bijwonen van de lectures en het voltooien van de Datacamp cursussen heb ik kunnen zien het proces van data science in elkaar zit en waarom het proces zo is.

<b>Reflectie</b><br />
Ik ben tevreden met resultaten die ik heb kunnen behalen. Ik heb de leerdoelen die ik voor mezelf had opgestelt kunnen behalen en dat geeft mij voldoening dat. Voordat ik aan de minor begon wist ik alleen wat data science was en wat je er mee kan. Nu kan ik door de minor zelf machine learning models of neural networks opgezetten en evalueren. Maar ik heb zeker tijdens de minor ook fouten gemaakt die ik wil verbeteren bij mijn eigen projecten. Na de minor zal ik zeker nog verder gaan met het verbeteren van mijn eigen proces bij het toepassen van data science. Ik weet nu op welke punten ik kritisch moet kijken om betrouwbare resultaten te kunnen bereiken.

</details>
<details>
<summary>Persoonlijke project bijdragen evaluatie</summary>
<b>Situatie</b><br />
De Smart Teddy Project was het eerste project dat betrekking had op data science. Het project bestond uit 6 project leden. Hiervan kwam er een project lid kwam van bestuurskunden, een van bedrijfskunden en 4 software engineering. Omdat ik als software engineering student al ervaring had met programmeren zou het programmeren van een ML model of een neural network niet all te moeilijk zijn kwa opzet. Ik kan hierdoor meer focus leggen op andere process van data science. Omdat er ook 2 team leden waren die nog geen ervaring hadden met programmeren, gaf ik aan dat ik graag hun wil helpen als er hulp nodig zou zijn. 

<b>Taak</b><br />
Ik na binnen het team de taak op als scum master. Als scrum master zorgde ik ervoor dat het scum proces soepel verloopt. Zo begeleide ik de daily standup's, sprint refinments, sprint planning en sprint retrospectives. Verder probeerde ik ervoor te zorgen dat iedereen in het team wist welke user stories hij moest uitvoeren en iedereen gemotiveerd te houden. Naast het de taak als scrum master was ik ook een data scientist. Deze rol nam met zich mee dat ik ML modellen of neural networks kan opzetten en verbeteren zodat we verschillende emoties kunnen classificeren. Verder moet dan de resultaten die uit de modellen komen geevalueerd worden. 

<b>Actie</b><br />
Door user stories te prioriseren kan er een overzicht van het project gemaakt worden. Hiermee weet het hele team wat hun te wachten staat. Verder stelde ik bij iedere meeting of er vragen waren of als iemand nog iets wou bespreken. <br />
Als data scientist moet ik de datacamp cursussen en lectures volgen. Die pas ik dan toe op mijn eigen modelen. Verder heb ik gebruik gemaakt van websites zoals StackOverflow en TowardsDatascience om verder te kunnen komen bij problemen.

<b>Resultaat</b><br />
Aan het begin van het project had iedereen behoefte aan een abstracte project overzicht. Hierom had ik samen met het team de huidige, afgesloten en toekomstige userstories er bij gehaald en deze in timeline overzicht gezet in Miro die hiervoor al is besproken. Door het maken van dit project overzicht had iedereen een goed beeld van onze huidige voortgang en welke werkzaamheden hierna uitgevoerd kunnen worden. Dit overzicht werdt bij iedere sprint planning erbij gehaald om deze bij te werken.<br />
Verder heb ik ML modellen kunnen opzetten en een neural network kunnen configueren. Hiervan heb ik de resultaten in kaart kunnen brengen doormidelen van Tensorboard of een confusion matrix.

<b>Reflectie</b><br />
Ik ben tevreden op de manier dat ik de scrum master rol heb kunnen voldoen voor dit project. Het team was transparant en de communicatie tussen elkaar was altijd op orde. Hierdoor kon het hele team efficient te werk gaan. Verder was het mij gelukt om een MLP model voor het project op te zetten. Nadat het team zag dat er een model was dat goede resultaten kon behalen werd iedereen meer gemotiveerd. Ook ben ik blij dat ik team leden heb kunnen ondersteunen bij het opzetten van ML modellen en het evalueren van onze CNN.

</details>
<details>
<summary>Groeps evaluatie</summary>
<b>Situatie</b><br />
Het projectgroep bestond in totaal uit 6 project leden. Vier projectleden studeren software engineering, één projectlid studeert bestuurskunden en één projectlid studeert bedrijfskunde. Iedereen binnen de groep had geen ervaring op het gebied van data science. De projectliden van bedrijfskunde en bestuurskunden hadden ook geen ervaring op het gebied van SCRUM en programmeren. Verder was iedereen in het project groep gemotiveerd om de minor te kunnen voltooien en daarbij over data science te kunnen leren.

<b>Taak</b><br />
Als projectgroep hadden wij de Emotions project van Hani Al-Ers onder ons genomen. Het eind goal van dit project was het kunnen opleveren van een ML model of een neural network die verschillende emoties kan herkennen. De resultaten die we daarvan hebben behaald wordt dan in een research paper opgenomen. 
<br />

Verder had iedereen in de groep ook zijn eigen taken. Zo had ik hiervoor al verteld dat ik de scrum master was en dat ik verantwoordelijk was voor het organiseren van de daily stand-ups, wekelijkse refinements, sprint planning en retrospectives. Een andere student was toevallig een docent op De Haagse Hogeschool. Hij nam opzich de taak op om de afspraken te beheren tussen de verschillende docenten. Verder had iedereen ook hun eigen taken die in de user stories zijn beschreven.

<b>Actie</b><br />
Als team besproken we altijd met elkaar wie welke taken opzich nam. Op bepaalde momenten kwam het wel eens voor dat meerdere projectleden of zelf iedereen bezig was met dezelfde userstories. Een voorbeeld hiervan is, dat iedereen aan het begin van het project bezig was met literatuur onderzoek of dat iedereen bezig was met de research paper. Maar bij de momenten waarvan dit niet zo was, was iedereen zelfstanding aan het werk met hun eigen user storie. Verder deden we ook aan pair programming. Zo konden we elkaar ondersteunen als iemand er niet uitkwam. 

Tijdens het project kwamen we ook tegen problemen aan. Op het moment dat we tegen problemen aankwamen waardoor bepaalde werkzaamheden stop gezet moest worden bespraken we altijd gelijk met elkaar. Als wij er dan niet uitkwamen vroegen we hulp en advies van de docenten.

<b>Resultaat</b><br />
Doordat iedereen gemotiveerd en vastberaden was om de minor en het project te voltooien hebben wij als project team veel kunnen bereiken. Aan het begin van de minor wisten we niet hoe we een ML model of een neural network moesten opzetten en of het project doel van de product owner haalbaar was. Maar door alle harde werk en communicatie met elkaar hebben we een CNN kunnen opleveren die emoties kan herkennen.

<b>Reflectie</b><br />
Ik kan met plezier en een goed gevoel deze minor afsluiten. We hebben als team en als individu veel kunnen bereiken met elkaar en op eigen kracht. Iedereen was positief ingesteld, transparant en behulpzaam. Verder hebben we ook een CNN kunnen opleveren met aardig goeie resulaten. Maar dit model kan zeker nog verbeterd worden. We hebben als team niet de hyperparameters kunnen tunnen en verder kunnen bouwen op onze CNN die nu alleen gebruik maakt van de DensNet model als baseline.

</details>

<br />

# Datacamp
Tijdens de minor heb ik de DataCamp cursussen die aangeboden werden gevolgd. Persoonlijk vond ik deze cursussen zeer leerzaam op het gebied van Data Science. Ik had hiervoor geen idee hoe Data Science praktisch inelkaar zat en deze cursussen gaven hier een aardig goed beeld van. Onderin in dit hoofdstuk heb ik een afbeelding toegevoegd met daarin de DataCamp cursussen die ik heb afgerond.

![Uitgevoerde DataCamp cursussen](https://gcdn.pbrd.co/images/E7pkfRINI68j.png?o=1)

_Figuur 4 - Uitgevoerde DataCamp cursussen_