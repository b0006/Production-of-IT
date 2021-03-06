# Представление знаний правилами продукций и логический вывод
<h1>Содержание</h1>
  <ul>
    <li><a href="#task">Задача</a></li>
    <li><a href="#about">Описание процесса решения</a></li>
    <li><a href="#solve">Решение</a></li>
    <li><a href="#experience">Полученный мною опыт</a></li>
  </ul>
<h2 id="task">Задача</h2>
<hr>
<p align="justify">
  Построить продукционную модель представления знаний в предметной области «Компьютерные сети» (организация).
</p>
<h2 id="about">Описание процесса решения</h2>
<hr>
<p align="justify">
  Для построения продукционной модели представления знаний необходимо выполнить следующие шаги: 
  <ol>
    <li>Определить целевые действия задачи (являющиеся решениями);</li>
    <li>Определить промежуточные действия или цепочку действий, между начальным состоянием и конечным (между тем, что имеется, и целевым действием);</li>
    <li>Опередить условия для каждого действия, при котором его целесообразно и возможно выполнить. Определить порядок выполнения действий;</li>
    <li>Добавить конкретики при необходимости, исходя из поставленной задачи;</li>
    <li>Преобразовать полученный порядок действий и соответствующие им условия в продукции;</li>
    <li>Для проверки правильности построения продукций записать цепочки продукций, явно проследив связи между ними;</li>
  </ol>
  Этот набор шагов предполагает движение при построении продукционной модели от результата к начальному состоянию, но возможно и движение от начального состояния к результату (шаги 1 и 2).
</p>
<h2 id="solve">Решение</h2>
<hr>
<p align="justify">
1)  Дмитрий имеет несколько компьютеров и хочет их соединить компьютерной сетью. Обязательное действие, выполняемое при организации сети – субъект может проложить сеть и после субъект может передать файл между компьютерами. Значит, есть уже два целевых действия «организовать сеть между компьютерами» и «передать файл», которые взаимосвязаны и следуют друг за другом.
</p>
<p align="justify">
2)  Прежде чем соединить компьютеры локальной сетью, нужны компьютеры и достаточно кабеля. Кроме того, нужно выбрать, на какую именно топологию сети выбрать, чтобы проложить сеть. Значит, цепочка промежуточных действий: «выбор топологии», «передать файл между компьютерами». 
</p>
<p align="justify">
3)  Прежде чем прокладывать сеть между компьютерами, необходимо убедиться, что есть необходимое количество кабеля. Выбор топологии сети может обуславливаться многими причинами, выберем организационный признак – самый дешевый и надежный. Для разных топологий требуются разные дополнительные оборудования, поэтому в зависимости от выбора топологии, оборудования будут различаться. Кроме того, разные топологии отличаются ценой оборудования и надежностью самой сети, поэтому данные топологии будет отличаться. Значит вначале идут действия, позволяющие выбрать топологию, затем характеризующие топологию, а уже потом передача файла.
</p>
<p align="justify">
4)  Пусть в задаче будут рассматриваться три топологии: «Шина», «Звезда» и «Кольцо». Первая – проще в организации и самый дешевый вариант, но не самый надежный. Вторая – надежнее чем первый, но дороже. Третий – «золотая середина» между первым и вторым. Надежнее, чем первый, и дешевле, чем второй. Для «Шина» требуется больше кабеля, для «Звезды» нужен центральный узел, а для «Кольца» потребуются сетевые контроллеры
</p>
<p align="justify">
5)  Выше описанное можно преобразовать в следующие предложения типа «Если, то»:
  <ul>
    <li>Если субъект хочет сделать сеть и у субъекта есть достаточно кабеля, то субъект может организовать сеть;</li>
    <li>Если топология Шина экономичнее и проще в организации, чем Звезда и Кольцо, то субъект выбирает Шина;</li>
    <li>Если топология Звезда надежнее, чем Шина и Кольцо, то субъект выберет Звезду;</li>
    <li>Если топология Кольцо надежнее, чем Шина и чуть дороже, но дешевле, чем Звезда, то субъект выбирает Кольцо;</li>
    <li>Если субъект выбрал Шина, то ему потребуется больше кабеля;</li>
    <li>Если субъект выбрал Звезда, то ему потребуется центр. узел;</li>
    <li>Если субъект выбрал Кольцо, то ему потребуется сетевые контроллеры;</li>
    <li>Если субъект выбрал Шина и имеет достаточно кабеля, то соединение занимает 50 мин;</li>
    <li>Если субъект выбрал Звезда и имеет центр. Узел, то соединение занимает 30 мин;</li>
    <li>Если субъект выбрал Кольцо и имеет сетевые контролеры, то соединении занимает 40 мин.;</li>
    <li>Если сеть проведена будет через 50, или через 30, или через 40 минут, то можно будет соединится между компьютерами;</li>
    <li>Если субъект может соединится, то он может передать файл;</li>
  </ul>
</p>
<p>
  Введем обозначения для фактов (Ф), действий (Д) и продукций (П), тогда:
</p>
<p>
  <b>Субъекты</b> – Дмитрий, Иван, Александр
</p>
<pre>
  Ф1 – субъект хочет проложить сеть
  Ф2 – у субъекта достаточно кабеля
  Ф3 – субъекту экономнее выбрать Шина
  Ф4 – субъекту надежнее Звезда
  Ф5 – субъекту надежнее Шина и дешевле. Чем Звезда
  Ф6 – субъекту требуется много кабеля
  Ф7 – субъекту требуется центр узел
  Ф8 – субъекту требуется сетевые контроллеры
  Ф9 – выбрал топологию сети
</pre>
<pre>
 Множество действий субъектов. 
 Д={Д1,Д2,Д3,Д4,Д5,Д6,Д7,Д8,Д9,Д10,Д11}:
</pre>
<pre>
  Д1 – субъект может проложить сеть
  Д2 – субъект выбрал Шина так как экономия
  Д3 – субъект выбрал Звезда так как надежнее
  Д4 – субъект выбрал Кольцо так как золотая середина
  Д5 – субъект прокладывает сеть с помощью большого кол-ва кабеля
  Д6 – субъект прокладывает сеть с помощью центр узла
  Д7 – субъект прокладывает сеть с помощью сетевого контроллера
  Д8 – сеть будет проложена через 50 мин
  Д9 – сеть будет проложена через 30 мин
  Д10 – сеть будет проложена через 40 мин
  Д11 – после соединения можно будет передать файл
</pre>
<p>
  Продукции:
</p>
<pre>
  П1 (5, Ф1 Ф2) = Д1
  П2 (4, Д1 Ф3) = Д2
  П3 (4, Д1 Ф4) = Д3
  П4 (4, Д1 Ф5) = Д4
  П5 (3 Д2 Ф6) = Д5
  П6 (3 Д3 Ф7) = Д6
  П7 (3 Д4 Ф8) = Д7
  П8 (2 Д5) = Д8
  П9 (2 Д6) = Д9
  П10 (2 Д7) = Д10
  П11(1 Д8 или Д9 или Д10) = Д116) 
</pre>
<p>
  <img src="1222.png" alt="production">
</p>
<h2 id="experience">Полученный мною опыт</h2>
  <ul>
    <li>Опыт работы с языком логики Prolog в среде Visual Prolog</li>
  </ul>
