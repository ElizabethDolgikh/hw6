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

1. Три самых частотных модификатора существительного question:

   - difficult
   - important
   - fundamental

![](https://github.com/ElizabethDolgikh/hw6/blob/master/SketchEngine_1.png)
![](https://github.com/ElizabethDolgikh/hw6/blob/master/SketchEngine_2.png)

2. Как синонимичные глаголы были выбраны __own__ и __possess__. 

![](https://github.com/ElizabethDolgikh/hw6/blob/master/SketchEngine_3.png)

Они могут употребляться со следующими дополнениями:

![](https://github.com/ElizabethDolgikh/hw6/blob/master/SketchEngine_4.png)

Интересно, что с __possess__ употребляются такие слова как _capacity, ability, qualification, knowledge, quality, characteristic, skill, attribute_, в то время как с __own__ чаще сочетаются слова, связанные с экономикой или физическими объектами.

Судя по выдаче в Sketch Engine, глаголов, которые употреблялись бы вместе с обоими словами, нет. 

![](https://github.com/ElizabethDolgikh/hw6/blob/master/SketchEngine_5.png)

Только с __possess__ употребляются 2 глагола:

- exercise

![](https://github.com/ElizabethDolgikh/hw6/blob/master/SketchEngine_6.png)

- expose

![](https://github.com/ElizabethDolgikh/hw6/blob/master/SketchEngine_7.png)

Только с __own__ употребляется 15 глаголов. Самые частотные сочетания:

- operate

![](https://github.com/ElizabethDolgikh/hw6/blob/master/SketchEngine_8.png)

- manage

![](https://github.com/ElizabethDolgikh/hw6/blob/master/SketchEngine_9.png)

- control

![](https://github.com/ElizabethDolgikh/hw6/blob/master/SketchEngine_10.png)

3. В разделе Trends корпуса BNC есть слово __predecessor__.

![](https://github.com/ElizabethDolgikh/hw6/blob/master/SketchEngine_11.png)

Данные в BNC (и график) показывают рост частотности слова. Посмотрим на частотность этого же слова в Ngram Viewer. Т.к. в BNC представлен британский английский на материале текстов второй половины XX века, а по слову predecessor данные по частотности даются с 1969 по 1994 гг., в настройках запроса был указан тот же временной промежуток и выбран корпус British English.

![](https://github.com/ElizabethDolgikh/hw6/blob/master/NgramViewer_predecessor(1).png)

Полученные два графика выглядят по-разному: Ngram Viewer не показывает резкий рост частотности слова predecessor. _С чем это может быть связано?_

1) BNC и Ngram Viewer измеряют частотность в разных единицах. В BNC для каждого года приводится IPM, в Ngram Viewer частотность дана в процентах.

![](https://github.com/ElizabethDolgikh/hw6/blob/master/comparison_1.png)
![](https://github.com/ElizabethDolgikh/hw6/blob/master/comparison_2.png)
![](https://github.com/ElizabethDolgikh/hw6/blob/master/comparison_3.png)

2) Число текстов в BNC и число книг, датируемых 1969-1994 гг., в корпусе британского английского в Ngram Viewer, скорее всего, тоже различны.

3) Корпус BNC более сбалансирован по жанрам, чем корпус Google Ngrams.

Похожие несоответствия получаются, если исследовать одно и то же слово в Ngram Viewer и в НКРЯ. 

