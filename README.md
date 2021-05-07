﻿
Мета роботи: встановлення Python на ПК, написання свого сайту та алгоритму розпізнання обличчя по фото та відео. 

Основною метою розрахункової роботи було встановлення мови програмування python (через «cmd» або за допомогою «.exe» з офіційного сайту). 

Наступним кроком було встановлення «PyCharm» одна з успішніших середовищ програмування на мові «Python». Далі ми створюємо проект в «PyCharm»:

![](Aspose.Words.0b861129-2c97-44cb-989f-21684d6ffb1b.001.png)

Необхідно встановити компоненти для написання сайту (Django):

![](Aspose.Words.0b861129-2c97-44cb-989f-21684d6ffb1b.002.png)

Код який включає основі компоненти головної сторінки:

![](Aspose.Words.0b861129-2c97-44cb-989f-21684d6ffb1b.003.png)

Та ще багато компонентів, таких як завантаження зображення, інтерфейс переходу та ще багато делікатних налаштувань.

Отриманий сайт:

![](Aspose.Words.0b861129-2c97-44cb-989f-21684d6ffb1b.004.png)

Так ми створили сайт для майбутнього дипломного проекту. В ньому буде відображатись потокове відео з дрону. Він буде керуватись з програми на комп’ютері або мобільному телефоні за допомогою штучного інтелекту, алгоритму розпізнання обличчя. 

Для досягнення мети ми познайомились з основами розпізнавання осіб і очей за допомогою каскадних класифікаторів на основі функцій Хаара.

Можна також використовувати попередньо визначені Каскади Haar, які доступні у відкритому доступі. 

Виявлення об'єктів з використанням каскадних класифікаторів Хаара - це підхід, заснований на машинному навчанні. Каскадна функція будується на великій кількості позитивних і негативних зображень. А потім використовується для виявлення об'єктів на зображеннях.

Для початку алгоритму потрібно багато позитивних зображень (зображень обличь) та негативних зображень (зображень без обличь) для навчання класифікатора. Потім нам потрібно витягнути з нього функції. Для цього використовуються особливості Хаара, показані на зображенні нижче.. Кожна функція представляє собою окреме значення, отримане шляхом віднімання сум  пікселів під білим прямокутником з сум пікселів під чорним прямокутником.

![](Aspose.Words.0b861129-2c97-44cb-989f-21684d6ffb1b.005.png)


Особливості ф.Хаара: 

Як ви можете побачити на малюнку, перші два - це "крайові функції", які використовуються для виявлення країв зображення. 

Третій - це "лінійна функція" (горизонтальна та вертикальна).  Горизонтальна пояснюється тим, що область очей значно темніше, ніж область носа або щоки. А вертикальна - що очі темніше за перенісся.

А четверта - "чотири прямокутника", найчастіше використовується для виявлення похилої лінії.


Для перевірки, ми застосували такий код:

З допомогою ного ми можемо знаходити з ШІ обличчя та очі на фото (рис.1)  та відео (рис.2) 

![](Aspose.Words.0b861129-2c97-44cb-989f-21684d6ffb1b.006.png)

Рис. 1 – Для фото

![](Aspose.Words.0b861129-2c97-44cb-989f-21684d6ffb1b.007.png)

Рис. 2 – Для відео

Результати: 

З відкритим лицем:

![image\_2021-04-21\_19-32-32](Aspose.Words.0b861129-2c97-44cb-989f-21684d6ffb1b.008.png)

Також з перешкодами\завадами для розпізнання лиця

![](Aspose.Words.0b861129-2c97-44cb-989f-21684d6ffb1b.009.png)

# Висновки: 

У ході виконання розрахунково-графічної роботи було встановлено Python та  PyCharm, написано простий сайт на мові програмування Python
для майбутньої його реалізації. Також були розглянуті алгоритми виявлення об'єктів з використанням каскадних класифікаторів Хаара, показані приклади знаходження обличчя та очей. 
