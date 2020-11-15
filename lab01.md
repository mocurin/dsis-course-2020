### К лекции №2

**Упражнение №5.0.1**  

Освойтесь с NumPy с помощью этого туториала:  

https://jakevdp.github.io/PythonDataScienceHandbook/02.00-introduction-to-numpy.html
  
Перед следующим упражнением, убедитесь что вы понимаете разницу между nparray и стандартным list!  
  
**Упражнение №5.0.2**  
Изучите Pandas - дефакто стандарт для работы с табличными (не bigdata) данными.  

https://jakevdp.github.io/PythonDataScienceHandbook/03.01-introducing-pandas-objects.html

https://jakevdp.github.io/PythonDataScienceHandbook/03.02-data-indexing-and-selection.html

https://jakevdp.github.io/PythonDataScienceHandbook/03.01-introducing-pandas-objects.html 
 
**Упражнение №5.1**  

Сделайте свой датафрейм на основе 2D-nparray  
Он должен поддерживать:  
* построчный индекс  
* хранить названия и порядок колонок  
* функции индексирования:  
 * iloc[i,j] - получить элемент по i-й строке j-й колонке. (i/j также могут быть slice-объектами)  
 * loc[k,z] - получить элемент по k-му значению построчного индекса z-й колонке (k может быть iterable/slice, z - iterable)  
 * [] - переопределить getitem, сделать его алиасом вашей loc-функции  
Также нужно сделать статический метод, читающий CSV:   
`your_package.read_csv(file_path, **csv_opts)`   
и возвращающий инстанс вашего датафрейма с прочитанными данными.    
Метод должен принимать параметры, настраивающие поведение чтения CSV-файла.  

**Упражнение №6.1**

Почитайте про случайный лес в [мануалах scikit](https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.RandomForestClassifier)

Научитесь обучать лес и запускать его.  
Для хранения и передачи данных для sklearn вы должны использовать собственный датафрейм!  

**Упражнение №6.2**

Научитесь визуализировать деревья. Почитайте:

  * [sklearn.tree.export_graphviz](https://scikit-learn.org/stable/modules/generated/sklearn.tree.export_graphviz.html#sklearn.tree.export_graphviz)
  * [How to Visualize a Decision Tree from a Random Forest in Python using Scikit-Learn](https://towardsdatascience.com/how-to-visualize-a-decision-tree-from-a-random-forest-in-python-using-scikit-learn-38ad2d75f21c)

**Задача №7**

Посмотрите на данные из выборки ещё раз. Обучите RF на этих данных.
Сравните RF c алгоритмами **p1_fraud**, **p2_fraud** и **p3_fraud**.

**Задача №8**

Подумайте, как с помощью RF оценивать информативность признаков?
Найдите информативные признаки. 

Сравните результаты с результатами **упражнения №1**.
