# hse_hw2_chip

Для исследования выбрана:
+ Клеточная линия: IMR-90
+ Гистоновая метка: H2AFZ

# Анализ FastQC

Все файлы представлены в папке [reports](./reports)

## Реплика 1 (ENCFF305XOA)
| |  |
|-----------------------|-------------------------|
| ![alt text](./img/xoa/basic_stat.png)   |       ![alt text](./img/xoa/Per%20base%20sequence%20quality.png)  Качество прочтений очень хорошее, все в зеленой зоне и даже не сильно падает к концу рида   |
| ![alt text](./img/xoa/Per%20tile%20sequence%20quality.png) |    ![alt text](./img/xoa/Per%20sequence%20GC%20content.png)      |
| ![alt text](./img/xoa/Adapter%20Content.png)  Лишних адаптеров нет |        ![alt text](./img/xoa/Per%20base%20sequence%20content.png)     |

## Реплика 2 (ENCFF191LBR)
| |  |
|-----------------------|-------------------------|
| ![alt text](./img/lbr/basic_stat.png)   |       ![alt text](./img/lbr/Per%20base%20sequence%20quality.png)   Все в зеленой зоне  |
| ![alt text](./img/lbr/Per%20tile%20sequence%20quality.png)  |    ![alt text](./img/lbr/Per%20sequence%20GC%20content.png)      |
| ![alt text](./img/lbr/Adapter%20Content.png)   Лишних адаптеров нет |        ![alt text](./img/lbr/Per%20base%20sequence%20content.png)     |
## Контроль (ENCFF679UAT)
Потребовалось подрезание чтений
| |  |
|-----------------------|-------------------------|
| ![alt text](./img/uat/basic_stat.png)   |       ![alt text](./img/uat/Per%20base%20sequence%20quality.png)     |
| ![alt text](./img/uat/Per%20tile%20sequence%20quality.png)  |    ![alt text](./img/uat/Per%20sequence%20GC%20content.png)      |
| ![alt text](./img/uat/Adapter%20Content.png)  Лишних адаптеров нет  |        ![alt text](./img/uat/Per%20base%20sequence%20content.png)     |

# Таблица со статистикой по выравниванию на 14 хромосому

| ID | Всего ридов | Уникально выровнилось | Неуникально выравнилось | Не выравнилось |
|----|-------------|-----------------------|-------------------------|----------------|
| ENCFF305XOA   |  55528468   |  2109040 (3.80%)  |   7395246 (13.32%)  |  46024182 (82.88%)  |
| ENCFF191LBR   |  45323153   |  1891932 (4.17%)   |  8252847 (18.21%)   |   35178374 (77.62%)   |
| ENCFF679UAT   |  45762504   |  2087866 (4.56%)   |  6736644 (14.72%)   |   36937994 (80.72%)   |

# Диаграммы Эйлера-Венна
| |  |
|-----------------------|-------------------------|
| ![alt text](./img/v1.png)   |   ![alt text](./img/v2.png)    |
| ![alt text](./img/v3.png) |    ![alt text](./img/v4.png)   |

Перечесений относительно мало, но это скорее всего происходит из-за того, что выравнивание было произведено только на одну хромосому.
# Бонус
![alt text](./img/bonus.png) 

Видим ниже, что располодение гистоновой метки совпадает с тем, что изображено на картинке для H2AFZ. Мы видим рост в начале, а потом затухание на графике.
| |  |
|-----------------------|-------------------------|
| ![alt text](./img/result_1.png)  |  ![alt text](./img/result_2.png)   |
