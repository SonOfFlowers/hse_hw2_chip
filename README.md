# hse_hw2_chip

Ссылка на колаб с основным заданием: https://colab.research.google.com/drive/1CLhbxoFdjsw0KW_4TqwHP73_yVhZQB_I?hl=ru#scrollTo=E83RAR9vNLut
Чтобы выполнить задание я взял клеточную линию - DND-41, гистоновую метку - H3K27ac , реплики - ENCFF000AQI, ENCFF000AQH, контроль - ENCFF000AOG. (Кратко AQI, AQH, AOG)

## FastQC reports

### AQI

![image](https://user-images.githubusercontent.com/93160309/157734342-4145ca93-9191-4bb7-9944-565d1a203376.png)

![image](https://user-images.githubusercontent.com/93160309/157734415-eb008e87-c189-4d47-ad1c-5464b807548c.png)

![image](https://user-images.githubusercontent.com/93160309/157734767-fb973a0e-bbb8-4470-a369-2a2340535318.png)

### AQH

![image](https://user-images.githubusercontent.com/93160309/157734838-0f911962-936b-4b93-9ac5-ee74220286e0.png)

![image](https://user-images.githubusercontent.com/93160309/157734878-1cbdbb24-1d74-4786-bf4c-7360108fdc7d.png)

![image](https://user-images.githubusercontent.com/93160309/157734948-78fefdb1-8eb4-45f9-b03c-13b8fb24833d.png)

### AOG

![image](https://user-images.githubusercontent.com/93160309/157734998-85d97628-515c-4801-9b44-1db664b6d6ec.png)

![image](https://user-images.githubusercontent.com/93160309/157735031-e8b64d59-e881-4f6b-ac55-e8bacead90c2.png)

![image](https://user-images.githubusercontent.com/93160309/157735070-4798e938-11d2-476b-ad10-1d1b970b8731.png)

Т.к. с fastq файлами все шикарно я пропустил стадию подрезания или фильтрования.

## Что дало нам выравнивание? (или пробежимся по результатам)

![image](https://user-images.githubusercontent.com/93160309/157735863-13aabfa9-a152-4fb2-85f8-2bcbe1baf159.png)

В клетках DND-41 с гистоном H3K27aс связалась не вся ДНК и не все её фрагменты , связанные с нужным гистоном, находятся на 14-ой хромосоме. Следовательно, уникальных выравниваний будет примерно столько, сколько занимает 14-ая хромосома во всей ДНК. 

## Сравнение результатов

![image](https://user-images.githubusercontent.com/93160309/157738829-7e0668a0-fee1-4724-aa63-777544f3528a.png)

![image](https://user-images.githubusercontent.com/93160309/157738903-d13e424b-b1c4-4b0c-a810-499b606a7842.png)

Поскольку мы выравниваем на одну хромосому, в результате мы имеем, что с большей частью пиков из файла ENCODE перечесений нет. 
