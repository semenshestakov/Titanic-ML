# Titanic ML
Это мои первые соревнования Kaggle 
https://www.kaggle.com/competitions/titanic 

Пройдемся по файлам в этом репозитории \
gender_submission.csv - это пример записи результата, индекс не нужно сохранять. \
train.csv - это файл с тренировочной выборкой и лэйблом \
test.csv - файл с тестовой выборкой, которую надо предсказать и записать в gender_submission.csv 
result - это какой у меня получился результат на тестовой выборке
Network.ipynb - это пример моего кода, как я работал с данными.

# Краткая статистика по тренировочной выборке
![Screenshot 2023-06-22 at 18.51.52.png](..%2F..%2F..%2F..%2F..%2Fvar%2Ffolders%2Fp8%2Fhs842n8x29x1xnhy3skzz61h0000gn%2FT%2FTemporaryItems%2FNSIRD_screencaptureui_99xjKN%2FScreenshot%202023-06-22%20at%2018.51.52.png)
![Screenshot 2023-06-22 at 18.53.11.png](..%2F..%2F..%2F..%2F..%2Fvar%2Ffolders%2Fp8%2Fhs842n8x29x1xnhy3skzz61h0000gn%2FT%2FTemporaryItems%2FNSIRD_screencaptureui_RQvDqS%2FScreenshot%202023-06-22%20at%2018.53.11.png)
Больше статистики есть на странице соревнований

# Выбор модели
Решил выбрать для первых соревнования нейронную сеть.

 (Dense)          (None, 64)                768        
 (Dropout)        (None, 64)                0\
 (Dense)          (None, 32)                2080      
 (Dropout)        (None, 32)                0         
 (Dense)          (None, 8)                 264       
 (Dense)          (None, 1)                 9         
                                                                 
Total params: 3,121
Trainable params: 3,121 \
Для модели выбрал оптимизатор - адам, ошибку -бинарная кросс-энтропия, метрику - accuracy


# Результаты
У меня получилось занять 2606 место из 15914 - это примерно топ 16%, я думаю если поиграться с данными, заполнить пропуски, то можно залететь в топ 10-12%,+ надо учитывать, что люди которые набрали точность выше 85% точно играли не честно, если даже не 82% - а таких примерно 500. Мне, кажется, что максимальная точность честным путём около 81%
![Screenshot 2023-06-22 at 19.05.11.png](..%2F..%2F..%2F..%2F..%2Fvar%2Ffolders%2Fp8%2Fhs842n8x29x1xnhy3skzz61h0000gn%2FT%2FTemporaryItems%2FNSIRD_screencaptureui_q0t2iB%2FScreenshot%202023-06-22%20at%2019.05.11.png)

