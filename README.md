# Часть 1. Google Ngram Viewer

## 10 самых частотных продолжений фразы "due to the"

 - fact
 - presence
 - lack
 - high
 - influence
 - absence
 - same
 - use
 - action
 - formation

![](https://github.com/ElizabethDolgikh/hw6/blob/master/NgramViewer_1.png "wildcard search")

## Part-of-speech Tags

Слово "only" в английском языке может относиться к 3-4 частям речи: быть наречием, прилагательным, союзом или существительным. В словарях зафиксированы только первые три варианта:

![](https://github.com/ElizabethDolgikh/hw6/blob/master/additional_pic_1.png "macmillan dictionary")
![](https://github.com/ElizabethDolgikh/hw6/blob/master/additional_pic_2.png "cambridge dictionary")
![](https://github.com/ElizabethDolgikh/hw6/blob/master/additional_pic_3.png "cambridge dictionary")
![](https://github.com/ElizabethDolgikh/hw6/blob/master/additional_pic_4.png "cambridge dictionary")

При этом "only" в функции существительного в некоторых контекстах все-таки можно встретить:

![](https://github.com/ElizabethDolgikh/hw6/blob/master/additional_pic_5.png)

Судя по получившемуся в Ngram Viewer графику, чаще всего "only" встречается в качестве наречия, реже всего — в качестве существительного и союза. Линии "ONLY_NOUN" и ONLY_CONJ" на графике сливаются.

![](https://github.com/ElizabethDolgikh/hw6/blob/master/NgramViewer_2.png "part-of-speech tags")

P.S. "case-insensitive search" был применен, т.к. в качестве наречия "only" может располагаться в начале предложения. В остальных случаях — только в середине или в конце предложения, что и показал Ngram Viewer:

![](https://github.com/ElizabethDolgikh/hw6/blob/master/NgramViewer2_comment.png)

## British English vs American English: Takeaway & Takeout

Для сравнения были выбраны слова takeaway и takeout. Оба являются существительными, производными от фразовых глаголов, take away и take out, означают еду «на вынос» или рестораны, готовящие такую еду. В словарях обычно указывается, что takeaway характерно для британского варианта английского языка, а takeout — для американского. Разница в написании существительных и фразовых глаголов важна, с ней впоследствии оказались связаны ошибки на графике (см. ниже).

Графики частотности этих слов в корпусах британского и американского английского это подтверждают. При этом разница в частотности слова takout для американского варианта языка и takeaway для британского на графике кажется незначительной.

![](https://github.com/ElizabethDolgikh/hw6/blob/master/NgramViewer_3(1).png)
![](https://github.com/ElizabethDolgikh/hw6/blob/master/NgramViewer_3(2).png)
![](https://github.com/ElizabethDolgikh/hw6/blob/master/NgramViewer_3(3).png)

Полный запрос в Ngram Viewer был таким:

`takeout_NOUN:eng_us_2012,takeout_NOUN:eng_gb_2012,takeaway_NOUN:eng_gb_2012,takeaway_NOUN:eng_us_2012`

![](https://github.com/ElizabethDolgikh/hw6/blob/master/NgramViewer_3(4).png)

_Зачем в запросе использовались частеречные теги_

Если их не указывать, искажается левая часть графика: складывается впечатление, что в 1800 году сравниваемые слова были более частотными, чем в 1900, а слово takeaway было более характерным для американского английского, чем для британского. 

![](https://github.com/ElizabethDolgikh/hw6/blob/master/NgramViewer_3(5).png)

Так получается из-за того, что в старых текстах больше ошибок распознавания. Это видно, если обратиться к ссылкам на тексты в разделе "Search in Google Books" под графиком: take out (или даже иногда _take our_ leave) в отсканированных книгах было распознано как takeout. 

![](https://github.com/ElizabethDolgikh/hw6/blob/master/takeaway_1.png)
![](https://github.com/ElizabethDolgikh/hw6/blob/master/takeaway_2.png)
![](https://github.com/ElizabethDolgikh/hw6/blob/master/takeaway_3.png)

Если построить график по запросу `takeout_NOUN,takeout_VERB`, искажение также будет видно. С takeaway ситуация аналогичная.

![](https://github.com/ElizabethDolgikh/hw6/blob/master/takeout%20verb%20or%20noun.png)

Если ограничить поиск частеречным тегом `_NOUN_`, график становится более точным.

# Часть 2. Sketch Engine




