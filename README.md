# llm-ravijuhendi-hindamine
See repositoorium on loodud magistreitöö jaoks, mille eesmärk on hinnata suurte keelemudelite (LLM-ide) võimekust ravijuhendite vastavuse hindamisel.

Repositooriumile ja selle sisule rakendub CC BY 4.0 litsents.

## Programmi töötamiseks kasutati

Python: versioon 3.11.14

ja järgnevaid teeke:

- torch (versioon 2.6.0+cu124)
- vllm (versioon 0.8.3)
- transformers (versioon 4.50.0)
- pypdf (versioon 6.7.0)
- pandas (versioon 3.0.0)
- openpyxl (versioon 3.1.5)
- accelerate (versioon 1.2.0)

Kõik vajalikud paketid saab paigaldada käsuga:

```bash
pip install -r requirements.txt
```

## Kirjeldus

See repositoorium sisaldab magistritöö **"Suurte keelemudelite kasutamine ravijuhendite vastavuse hindamiseks päriselu terviseandmete põhjal"** koodi, ravijuhendite kuut versiooni (kolm formaati × kaks keelt) koos võltsitud juhendiga ning näidisandmete faili.

Töös uuriti, kuidas avatud lähtekoodiga meditsiiniline keelemudel MedGemma 27B suudab hinnata Eesti emakakaelavähi sõeluuringu juhendi täitmist 103 patsiendi vaatlusandmete põhjal.

## Juhised

Programmi käivitamiseks tuleb kasutada repositooriumis olevat koodifaili.

Enne käivitamist tuleb muuta faili alguses olevaid parameetreid vastavalt andmetele ja vajadusele:
kasutatav mudel,
Hugging Face'i token
sisendandmete fail,
ravijuhendite asukoht,
väljundseaded ja
kasutatavad viibad.

## Programmi käivitamine:

```bash
python kood.py
```

## Märkused
Enamus piisavalt suured keelemudelid vajavad GPU ja CUDA tuge.
