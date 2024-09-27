# ПСБ хакатон
<p align="center">
<img src="https://github.com/AndrewsCollider/PSB_hackathon/blob/main/Team_logo.png" width="250" height="250" class="center">

  # Команда: HackHunters
</p>

# Задание 

[Ссылка на условие](https://ai.hse.ru/hacks/psb24)

Задача классификации.

В рамках данного хакатона нам надо было создать модель для банка, которая помогала бы отелям-партнерам **определить отменит ли клиент бронирование номера**. Результаты технической части надо было внедрить в **новый банковский продукт**, помогающий студентам с организацией отдыха, а отелям с пониманием, как не понести убытки из-за отмененных броней.

**Метрика:** AUC ROC

# Навигация в файлах и папках:
- `data` - initial data provided by the organizers
  - `train.xlsx` - начальный обучающий датасет
  - `test.xlsx` - начальный тестовый датасет
  - `Train.csv` - обработанный обучающий датасет
  - `Test.csv` - обработанный тестовый датасет
  - `Preprocessing.ipynb` - код обработки данных
- `models` - модели, реализованные в рамках данного хакатона
  - `Ensembles.ipynb`
  - `Tabnet.ipynb`
  - `AutoML.ipynb`

# Решение
Для решения задачи классификации мы попробовали множество моделей, а также методов обработки данных и добавления признаков для большего удобства и высшей точности. Немного подробностей о каждой стадии:

## Обработка данных

## Добавление новых признаков

## Построение моделей

## Итоговый банковский продукт
Схематичный вид продукта и выгода для каждого участника (банка, отелей, студентов) можно найти в презентации. 

Исходя из анализа рынка, сделанного по открытым источникам, собственным опросам и custdev-интервью, мы выявили основные боли студентов. Чтобы удовлетворить основные потребности поколения Z и создать удобный продукт, мы решили предложить ПСБ **приложение и карту**.

Приложение включает в себя:
- **`Трикаунт`**, чтобы забыть о раздельном счете во время поездок с друзьями.
  - **`Пример:`** Компания друзей из 4 человек поехали в Питер на 5 дней. Там они платят за еду, экскурсии, развлечения и отель. Причем платит не каждый сам за себя, а преимущественно один оплачивает за всех, чтобы сэкономить время.
  - **Вместе с Трикаунт** они `смогут забыть о проблеме` разделения счетов: сервис позволяет учесть расходы каждого, неттингует платежи и предлагает **наилучший** способ рассчитаться с другом.
- **`GPT Travel`** - генеративный ИИ, который по запросу, заданному в вольной форме, выдает варианты наиболее подходящих мест отдыха. <br>
  - **`Пример запроса:`** Привет, подбери подходящий город: мой бюджет 50.000 рублей на 10 дней на двоих, поеду летом. Хочу, чтобы путь от Москвы до города занял не больше суток. Хочу, чтобы мой отдых был активным, c разными видами спорта на воде, а, плавая, я должен видеть горы!!
  - **`Ответ GPT:`** вот 4 варианта, которые могут подходить под большинство вашим запросов... (`*Выдает:* место, цену, отель, путь до места отдыха и тд`)
- **`Карта с аутентичными районами от местных жителей`**
  - Представители поколения Z, прошедшие *custdev-интервью*, отмечали, что зачастую едут в новые города, чтобы узнать местную культуру, быт людей и другие особенности. `Они не хотят` ходить по всем известным достопримечательностям, ведь лучше "прожить жизнь" местных жителей и увидеть аутентичные места, значимые для тех, кто родился и вырос в этих местах.
  - В приложении будет размещена **карта с развернутыми модерируемыми комментариями о своей малой родине** от каждого пользователя приложения. В качестве системы стимулов размещения комментариев будет добавлена **геймификация**, а также разработаны поощрительные бонусы. Да что там бонусы: многим людям поколения Z просто хочется делиться со сверстниками особенностями своего любимого города.
- **`Отслеживание добросовестности клиента`** - данная составляющая приложения создана по большей части для отелей и стимулирования пользователей лучше планировать поездки, чтобы `не отказываться от брони`. Уровни, которые будут копиться у пользователя и, возможно, давать бонусы в виде кэшбэков, могут сбрасываться, если пользователь отменил бронь в последний момент.
- **`Скидки, кэшбэки, займы с отложенным возвратом`**

