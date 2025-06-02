[![Typing SVG](https://readme-typing-svg.herokuapp.com?font=Roboto&weight=500&size=26&pause=1000&color=F7F7F7&width=500&lines=YandexMaps+Graber;%D0%90%D1%81%D0%B8%D0%BD%D1%85%D1%80%D0%BE%D0%BD%D0%BD%D1%8B%D0%B9+%D0%BF%D0%B0%D1%80%D1%81%D0%B5%D1%80+%D0%B4%D0%BB%D1%8F+%D0%AF%D0%BD%D0%B4%D0%B5%D0%BA%D1%81.%D0%9A%D0%B0%D1%80%D1%82+)](https://git.io/typing-svg)

![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54) ![Playwright](https://img.shields.io/badge/-playwright-%232EAD33?style=for-the-badge&logo=playwright&logoColor=white) 
## Используемый стек
- Python 3.13
- Playwright + Asyncio
- Json

## Установка и запуск
~~~
git clone https://github.com/tak3e/yandexmapsgraber.git
cd YandexMapsGraber
pip3 install -r requirements.txt
python3 main.py
~~~

После запуска откроется окно браузера. Сначала необходимо выбрать масштаб поиска, который отображается справа внизу. Чтобы увеличить или уменьшить масштаб, прокрутите колесиком мыши. Затем нажмите левую кнопку мыши и выберите точку на карте, после чего нажмите «Искать рядом». После этого начинается загрузка компаний и автоматический парсинг. По окончанию работы скрипта, появляется файл result.json с полученой информацией с сайтов.

## Конфигурация 
- **scroll_units = 500**
Данный параметр отвечает за прогрузку компаний. Чем больше значение, тем больше компаний будет найдено. На каждые 500 ед. приходится +-150 компаний, зависит от мощности ПК. Стоит также отметить, чем больше значение, тем дольше будет прогрузка.

- **time_to_search = 120000**
Указывается в милисекундах. Отвечает за время выбора точки и маштаба на карте, по истечению 120 секунд, программа закроется. 
- **time_limit_for_parsing = 5000**
