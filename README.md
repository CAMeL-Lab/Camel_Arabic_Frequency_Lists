# CAMeL_Arabic_Frequency_Lists

## Summary
The CAMeL Arabic Frequency Lists dataset is derived from the pretraining datasets used to pretrain the family of [CAMeLBERT models](https://huggingface.co/collections/CAMeL-Lab/camelbert-653f42bfcbc8ae32a51a692d) (16.1M unique word types / 17.3B word tokens). Three main varieties of Arabic were used: Classical Arabic (CA), Dialectal Arabic (DA), and Modern Standard Arabic (MSA).

**To download, please click on the link below**:
- [CA_freq_lists.tsv.zip](https://github.com/CAMeL-Lab/Camel_Arabic_Frequency_Lists/releases/download/v1.0/CA_freq_lists.tsv.zip): Classical Arabic frequency list.
- [DA_freq_lists.tsv.zip](https://github.com/CAMeL-Lab/Camel_Arabic_Frequency_Lists/releases/download/v1.0/DA_freq_lists.tsv.zip): Dialectal Arabic (mixed dialects) frequency list.
- [MSA_freq_lists.tsv.zip](https://github.com/CAMeL-Lab/Camel_Arabic_Frequency_Lists/releases/download/v1.0/MSA_freq_lists.tsv.zip): Modern Standard Arabic frequency list.
- [MIX_freq_lists.tsv.zip](https://github.com/CAMeL-Lab/Camel_Arabic_Frequency_Lists/releases/download/v1.0/MIX_freq_lists.tsv.zip): All CA+DA+MSA frequency list (a union of all three sets with frequencies aggregated)

For details about the different genres and sources of the data, please refer to the CAMeLBERT paper [here](https://aclanthology.org/2021.wanlp-1.10/).

Each of the frequency list files contains unique types of Arabic only words along with their frequencies as they appeared in the pretraining data. We excluded digits, punctuation, and non-Arabic script tokens.

All files are tab-separated with the first column being the word in Arabic script and the second column being the frequency (note that due to the mixed text direction the the order may be *displayed* in reverse). See the following example:

- Examples from CA: out of 2.4M unique word types from a corpus of 847M word tokens.
```
في	16664531
من	15695517
بن	13571947
الله	11433931
عن	9140820
...
المستعان	6285
الورقة	6284
الروياني	6284
الثريا	6283
يسافر	6283

....
فكعمرة	4
فكعرض	4
فكضامن	4
فكرؤيته	4
فكتفريق	4
```

- Examples from DA: out of 6.7M unique word types from a corpus of 5.8B word tokens.
```
من	127245884
في	101567242
الله	72525262
علي	65410197
لا	52420507
...
قضيته	70256
دره	70235
تعطيك	70226
تهديد	70216
الاوراق	70213
...
هالمكااان	35
هالشوز	35
هالرغد	35
هالثبات	35
نننس	35

```

- Examples from MSA: out of 11.4M unique word types from a corpus of 12.6B word tokens.
```
في	255725161
من	205864175
على	122591931
و	68783652
أن	64519408
...
السائل	128423
ثانوى	128420
الحيوانية	128417
نزيف	128393
عصابة	128386
...
سهرن	52
ستنسيه	52
ستمتلكه	52
ستكفينا	52
ستضره	52

```

- Examples from MIX: out of 16.1M unique word types from a corpus of 17.3B word tokens.
```
في	373956934
من	348805576
على	132084198
و	121102569
الله	111745498
...
وفدا	213505
المنافقين	213483
البيلاروسي	213461
الطيبين	213441
اساسي	213409
...
كهلون	91
كفعال	91
كعروة	91
كالوفرة	91
كالمستهزىء	91

```

## Citation
```
@software{Khalifa:2021:Camel_Frequency,
author = {Khalifa, Salam and Inoue, Go and Alhafni, Bashar and Baimukan, Nurpeiis and Bouamor, Houda and Habash, Nizar},
title = {{Camel Arabic Frequency Lists }},
year = 2021,
url = {https://github.com/CAMeL-Lab/Camel_Arabic_Frequency_Lists}
}
```

## Contributors
- Salam Khalifa
- CAMeLBERT paper authors
