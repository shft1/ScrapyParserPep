# Scrapy Parser PEP

---

### Парсер, который собирет информацию о всех существующих документах PEP и сохраняет ее в соответствующие файлы:
- `pep_время_.csv` - файл, в котором лежит вся информации про PEP (номер, имя, статус)
- `status_summary_время_.csv` - файл, в котором лежит результат сбора информации PEP,   
а именно количество PEP в разных статусах и их общее количество.

---

### Стек Технологий:
- Python 3.9
- Scrapy
- requests

---

**Пререквизиты:**
- OC - Кроссплатформенная
- Версия python - 3.9 и выше

---

### Инструкция по развертыванию:
**Клонируйте репозиторий:**

```
git clone git@github.com:shft1/ScrapyParserPep.git
```

**Cоздайте и активируйте виртуальное окружение:**

```
python3 -m venv venv
```

* _Если у вас Linux/macOS_

    ```
    source venv/bin/activate
    ```
* _Если у вас Windows_

    ```
    source venv/scripts/activate
    ```

**Установите зависимости из файла requirements.txt:**

```
pip install -r requirements.txt
```

---

**Запустите тесты, для проверки корректности работы приложения**  
Находясь в дирректории `scrapy_parser_pep` выполните следующую команду:
```
(venv) .../scrapy_parser_pep $ pytest
```
_Если все 14 тестов успешно пройдены, то Парсер полностью функционирует_

<img width="1143" alt="image" src="https://github.com/user-attachments/assets/84cd1052-f68d-41a4-b5a8-54903c93df67" />

---

Запустить проект нужно командой `scrapy crawl pep` из дирректории `scrapy_parser_pep`
```
(venv) .../scrapy_parser_pep $ scrapy crawl pep
```

---

Исполнитель - [Алексей Малков](https://github.com/shft1)
