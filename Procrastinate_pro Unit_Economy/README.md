# Анализ убытков приложения ProcrastinatePRO+

## Описание проекта

Мною было проведено исследование данных приложения Procrastinate Pro+ для определения причин по которой компания терпит убытки последние месяцы, несмотря на большие маркетинговые расходы.    
Цель проекта разобраться в причинах убытков, и выделить стратегии для выхода компании в плюс.    
Для анализа будут использованы данные о пользователях за период с 1 мая по 27 октября 2019 года. После ознакомления и предобработки данных необходимо проанализировать поведения клиентов и определить:

- откуда приходят пользователи и какими устройствами они пользуются
- сколько стоит привлечение пользователей из различных рекламных каналов
- сколько денег приносит каждый клиент
- когда расходы на привлечение клиента окупаются
- какие факторы мешают привлечению клиентов

## Используемые технологии
- Python
- Pandas
- Matplotlib
- Когортный анализ 
- Юнит-экономика 
- Продуктовые метрики

## Выводы

В ходе исследования были проанализированы продуктовые метрики, такие как **retention_rate, churn_rate, conversion_rate, ARPU, cohort_analysis, LTV, ROI, CAC** в разбивке по основным признакам: регион и устройство пользователя, и канал привлечения. 

По результатам исследования было обнаружено, что не окупаются отдельные сегменты пользователей, такие как: **пользователи из США, пользователи привлеченные через дорогие источники AdNonSense, FaceBoom, TipTop а также пользователи девайсов iPhone & Mac.** 

---

1. В региональной разбивке отчетливо видно, что ROI не окупается только в США, и это связано с резким увеличением маркетинговых расходов с июня, при относительно небольшой разнице в LTV клиентов, привлекаемых их США. При этом конверсия пользователей из США ощутимо лучше, чем в остальных странах. A по показателю удержания платящие пользователи из США стабильно плохо удерживаются. Можно повысить удержание для пользователей из США, например с помощью введения персонализированных UX-стратегий, e-mail рассылок, персональных рекомендаций, push-уведомлений. Можно ввести определённые "награды" или привилегии для постоянных пользователей.  
    
2. По анализу LTV, ROI, Conversion, Retention в разбивке по каналам видно что TipTop довольно дорогой канал, LTV его клиентов выше среднего, но при этом он намного ниже CAC по данному каналу. Учитывая что клиенты TipTop конвертируются и удерживаются так же как в других более дешевых каналах, я бы рекомендовала пересмотреть варианты релокации бюджета данного канала на альтернативные более дешевые каналы привлечения.
    
3. Каналы FaceBoom & AdNonSense очень похожи по качеству привлекаемых клиентов. Клиенты данных каналов хорошо конвертируются в платящих, но плохо удерживаются. Если продуктовой команде удастся увеличить повторные продажи клиентам этих каналов, каналы могут выйти в зону окупаемости. Можно ввести определённые "награды" или привилегии для постоянных пользователей.  Также, можно ввести поощрение пользователей за репосты контента и прочий социальный engagement, связанный с приложением, в данных каналах.     