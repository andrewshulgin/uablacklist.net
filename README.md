# UABlacklist

Список запрещённых в Украине сайтов.

## Основания
| Дата       | Основание                                                                                 |
| ---------- | ----------------------------------------------------------------------------------------- |
| 19.10.2022 | [УКАЗ ПРЕЗИДЕНТА УКРАЇНИ №726/2022](https://www.president.gov.ua/documents/7262022-44481) |
| 26.02.2022 | [НКРЗІ](https://nkrzi.gov.ua/index.php?r=site/index&pg=99&id=2249)                        |
| 16.02.2022 | [УКАЗ ПРЕЗИДЕНТА УКРАЇНИ №57/2022](https://www.president.gov.ua/documents/572022-41373)   |
| 11.02.2022 | [УКАЗ ПРЕЗИДЕНТА УКРАЇНИ №51/2022](https://www.president.gov.ua/documents/512022-41349)   |
| 30.10.2021 | [УКАЗ ПРЕЗИДЕНТА УКРАЇНИ №556/2021](https://www.president.gov.ua/documents/5562021-40497) |
| 21.08.2021 | [УКАЗ ПРЕЗИДЕНТА УКРАЇНИ №379/2021](https://www.president.gov.ua/documents/3792021-39757) |
| 21.08.2021 | [УКАЗ ПРЕЗИДЕНТА УКРАЇНИ №378/2021](https://www.president.gov.ua/documents/3782021-39753) |
| 20.08.2021 | [УКАЗ ПРЕЗИДЕНТА УКРАЇНИ №376/2021](https://www.president.gov.ua/documents/3762021-39745) |
| 20.08.2021 | [УКАЗ ПРЕЗИДЕНТА УКРАЇНИ №375/2021](https://www.president.gov.ua/documents/3752021-39741) |
| 24.06.2021 | [УКАЗ ПРЕЗИДЕНТА УКРАЇНИ №266/2021](https://www.president.gov.ua/documents/2662021-39265) |
| 24.06.2021 | [УКАЗ ПРЕЗИДЕНТА УКРАЇНИ №265/2021](https://www.president.gov.ua/documents/2652021-39261) |
| 21.05.2021 | [УКАЗ ПРЕЗИДЕНТА УКРАЇНИ №203/2021](https://www.president.gov.ua/documents/2032021-38949) |
| 23.03.2021 | [УКАЗ ПРЕЗИДЕНТА УКРАЇНИ №109/2021](https://www.president.gov.ua/documents/1092021-37481) |
| 14.05.2020 | [УКАЗ ПРЕЗИДЕНТА УКРАЇНИ №184/2020](https://www.president.gov.ua/documents/1842020-33629) |
| 13.02.2020 | [Cправа № 761/4683/20](https://nkrzi.gov.ua/index.php?r=site/index&pg=99&id=1876)         |
| 27.01.2020 | [Cправа № 757/3623/20-к](https://nkrzi.gov.ua/index.php?r=site/index&pg=99&id=1870)       |
| 19.03.2019 | [УКАЗ ПРЕЗИДЕНТА УКРАЇНИ №82/2019](https://www.president.gov.ua/documents/822019-26290)   |
| 21.06.2018 | [УКАЗ ПРЕЗИДЕНТА УКРАЇНИ №176/2018](https://www.president.gov.ua/documents/1762018-24362) |
| 14.05.2018 | [УКАЗ ПРЕЗИДЕНТА УКРАЇНИ №126/2018](https://www.president.gov.ua/documents/1262018-24150) |
| 15.05.2017 | [УКАЗ ПРЕЗИДЕНТА УКРАЇНИ №133/2017](https://www.president.gov.ua/documents/1332017-21850) |

## Формат domains.json

Массив объектов, где ключ - домен. Значение - объект со свойствами:

- `urls` (масссив, опционально). Список ссылок, которые были перечислены в документе, на том же домене. Отсутствует, 
  если в документе не было ссылок.
- `company` (строка, опционально). Название компании на украинском языке, которой принадлежит домен, как она указана в 
  документе. Изначально отсутствовало, поэтому некоторые домены без этого свойства.
- `alias` (строка, опционально). Алиас латиницей для группировки нескольких доменов разных компаний для удобства. 
  Допустим, у webmoney несколько названий компаний и для группировки используется alias.   
- `reason` (строка, опционально). Ссылка или текстовое описание причины блокировки.
- `term` (строка или null). Дата конца блокировки формата "дд.мм.гггг". `null` в случае безсрочной блокировки.
