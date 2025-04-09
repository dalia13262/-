<!DOCTYPE html>
<!-- saved from url=(0241)file:///E:/%D0%B0%D1%80%D1%85%D0%B8%D1%82%D0%B5%D0%BA%D1%82%D1%83%D1%80%D0%BD%D1%8B%D0%B5%20%D1%81%D0%BE%D0%BE%D1%80%D1%83%D0%B6%D0%B5%D0%BD%D0%B8%D1%8F%20%D0%B3%D0%BE%D1%80%D0%BE%D0%B4%D0%B0%20%D0%98%D1%80%D0%BA%D1%83%D1%82%D1%81%D0%BA.html -->
<html lang="ru"><head><meta http-equiv="Content-Type" content="text/html; charset=UTF-8">
    
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Архитектурные сокровища Иркутска</title>
    <style>
        body {
            font-family: 'Roboto', sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f5f5f5;
            color: #333;
        }
        
        header {
            background: linear-gradient(135deg, #1e3c72 0%, #2a5298 100%);
            color: white;
            padding: 2rem;
            text-align: center;
            box-shadow: 0 4px 12px rgba(0,0,0,0.1);
        }
        
        h1 {
            margin: 0;
            font-size: 2.5rem;
        }
        
        .subtitle {
            font-size: 1.2rem;
            opacity: 0.9;
        }
        
        .container {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            padding: 2rem;
            gap: 2rem;
            max-width: 1400px;
            margin: 0 auto;
        }
        
        .building-card {
            background: white;
            border-radius: 8px;
            box-shadow: 0 4px 8px rgba(0,0,0,0.1);
            width: 350px;
            overflow: hidden;
            transition: transform 0.3s ease;
        }
        
        .building-card:hover {
            transform: translateY(-5px);
        }
        
        .model-container {
            height: 250px;
            background: #eee;
            position: relative;
        }
        
        .model-placeholder {
            width: 100%;
            height: 100%;
            display: flex;
            align-items: center;
            justify-content: center;
            background: linear-gradient(135deg, #e0e0e0 0%, #bdbdbd 100%);
            color: #555;
            font-weight: bold;
        }
        
        .building-info {
            padding: 1.5rem;
        }
        
        .building-name {
            font-size: 1.5rem;
            margin: 0 0 0.5rem 0;
            color: #1e3c72;
        }
        
        .building-description {
            margin: 0;
            color: #666;
            line-height: 1.5;
        }
        
        .info-button {
            display: inline-block;
            margin-top: 1rem;
            padding: 0.5rem 1rem;
            background: #1e3c72;
            color: white;
            border: none;
            border-radius: 4px;
            cursor: pointer;
            transition: background 0.3s ease;
        }
        
        .info-button:hover {
            background: #2a5298;
        }
        
        .modal {
            display: none;
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: rgba(0,0,0,0.7);
            z-index: 100;
            align-items: center;
            justify-content: center;
        }
        
        .modal-content {
            background: white;
            border-radius: 8px;
            width: 80%;
            max-width: 800px;
            max-height: 80vh;
            overflow-y: auto;
            padding: 2rem;
            position: relative;
        }
        
        .close-button {
            position: absolute;
            top: 1rem;
            right: 1rem;
            font-size: 1.5rem;
            background: none;
            border: none;
            cursor: pointer;
            color: #666;
        }
        
        .modal-title {
            font-size: 2rem;
            color: #1e3c72;
            margin-top: 0;
        }
        
        .modal-image {
            width: 100%;
            height: 300px;
            object-fit: cover;
            border-radius: 4px;
            margin: 1rem 0;
        }
        
        footer {
            background: #333;
            color: white;
            text-align: center;
            padding: 1.5rem;
            margin-top: 2rem;
        }
        
        @media (max-width: 768px) {
            .container {
                padding: 1rem;
            }
            
            .building-card {
                width: 100%;
            }
            
            .modal-content {
                width: 95%;
                padding: 1rem;
            }
        }
    </style>
</head>
<body>
    <header>
        <h1>Архитектурные сокровища Иркутска</h1>
        <p class="subtitle">Интерактивная 3D коллекция исторических зданий</p>
    </header>
    
    <div class="container">
        <!-- Московские ворота -->
        <div class="building-card">
            <div class="model-container">
                <div class="model-placeholder">3D модель Московских ворот</div>
            </div>
            <div class="building-info">
                <h2 class="building-name">Московские ворота</h2>
                <p class="building-description">Триумфальная арка, построенная в 1813 году в честь 10-летия восшествия на престол Александра I.</p>
                <button class="info-button" onclick="openModal(&#39;moskovskie-vorota&#39;)">Подробнее</button>
            </div>
        </div>
        
        <!-- Драматический театр -->
        <div class="building-card">
            <div class="model-container">
                <div class="model-placeholder">3D модель Драматического театра</div>
            </div>
            <div class="building-info">
                <h2 class="building-name">Драматический театр им. Охлопкова</h2>
                <p class="building-description">Один из старейших театров Сибири, основанный в 1850 году с уникальной архитектурой.</p>
                <button class="info-button" onclick="openModal(&#39;teatr-ohlopkova&#39;)">Подробнее</button>
            </div>
        </div>
        
        <!-- Собор Богоявления -->
        <div class="building-card">
            <div class="model-container">
                <div class="model-placeholder">3D модель Собора Богоявления</div>
            </div>
            <div class="building-info">
                <h2 class="building-name">Собор Богоявления</h2>
                <p class="building-description">Православный храм, памятник сибирского барокко, построенный в 1718-1746 годах.</p>
                <button class="info-button" onclick="openModal(&#39;sobor-bogoyavleniya&#39;)">Подробнее</button>
            </div>
        </div>
        
        <!-- Музей декабристов -->
        <div class="building-card">
            <div class="model-container">
                <div class="model-placeholder">3D модель Музея декабристов</div>
            </div>
            <div class="building-info">
                <h2 class="building-name">Музей декабристов</h2>
                <p class="building-description">Историко-мемориальный музей, посвященный жизни декабристов в сибирской ссылке.</p>
                <button class="info-button" onclick="openModal(&#39;muzey-dekabristov&#39;)">Подробнее</button>
            </div>
        </div>
        
        <!-- Дом-музей Вампилова -->
        <div class="building-card">
            <div class="model-container">
                <div class="model-placeholder">3D модель Дома-музея Вампилова</div>
            </div>
            <div class="building-info">
                <h2 class="building-name">Дом-музей Вампилова</h2>
                <p class="building-description">Мемориальный музей драматурга Александра Вампилова, расположенный в доме его детства.</p>
                <button class="info-button" onclick="openModal(&#39;dom-vampilova&#39;)">Подробнее</button>
            </div>
        </div>
        
        <!-- Усадьба Сукачёва -->
        <div class="building-card">
            <div class="model-container">
                <div class="model-placeholder">3D модель Усадьбы Сукачёва</div>
            </div>
            <div class="building-info">
                <h2 class="building-name">Усадьба Сукачёва</h2>
                <p class="building-description">Городская усадьба XIX века, принадлежавшая городскому голове В.П. Сукачёву.</p>
                <button class="info-button" onclick="openModal(&#39;usadba-sukacheva&#39;)">Подробнее</button>
            </div>
        </div>
        
        <!-- Сибирский дворец -->
        <div class="building-card">
            <div class="model-container">
                <div class="model-placeholder">3D модель Сибирский дворец</div>
            </div>
            <div class="building-info">
                <h2 class="building-name">Сибирский дворец</h2>
                <p class="building-description">Сибирский дворец или, как называют его горожане, Белый дом.</p>
                <button class="info-button" onclick="openModal(&#39;sibirskiy-dvorec&#39;)">Подробнее</button>
            </div>
        </div>
        
        <!-- Усадьба Шастиных -->
        <div class="building-card">
            <div class="model-container">
                <div class="model-placeholder">3D модель Усадьбы Шастиных</div>
            </div>
            <div class="building-info">
                <h2 class="building-name">Усадьба Шастиных</h2>
                <p class="building-description">Деревянная усадьба в стиле модерн, построенная в начале XX века для купеческой семьи Шастиных.</p>
                <button class="info-button" onclick="openModal(&#39;usadba-shastinyh&#39;)">Подробнее</button>
            </div>
        </div>
    </div>
    
    <!-- Модальные окна с подробной информацией -->
    <div id="moskovskie-vorota" class="modal">
        <div class="modal-content">
            <button class="close-button" onclick="closeModal()">×</button>
            <h2 class="modal-title">Московские ворота</h2>
            <img src="./Архитектурные сокровища Иркутска_files/4fdbe1eb7b02bf5224d0956c9d4061ca.jpg" alt="Московские ворота" class="modal-image">
            <p>Московские ворота — триумфальная арка в Иркутске, построенная в 1813 году в честь 10-летия восшествия на престол императора Александра I. </p>
            <p></p>📍 Местоположение: ул. Нижняя Набережная, рядом с площадью Декабристов.
			<p>Архитектурный стиль: ампир. Высота сооружения составляет 19 метров, ширина — 16,5 метров. Ворота украшены колоннами и скульптурными композициями.</p>
            <p>Первые деревянные ворота возвели в 1811 году к столетию дома Романовых. В 1891 году их заменили каменными, которые, к сожалению, были снесены в советское время.Полностью восстановлены по сохранившимся чертежам и фотографиям в 2011 году. Ворота расположены на въезде в историческую часть города со стороны Московского тракта и символизируют связь Иркутска с европейской частью России. На них изображены гербы Сибири и Иркутска, а также памятные надписи.</p>
        </div>
    </div>
    
    <div id="teatr-ohlopkova" class="modal">
        <div class="modal-content">
            <button class="close-button" onclick="closeModal()">×</button>
            <h2 class="modal-title">Драматический театр им. Н.П. Охлопкова</h2>
            <img src="./Архитектурные сокровища Иркутска_files/XXXL" alt="Драматический театр" class="modal-image">
            <p>Иркутский академический драматический театр имени Н.П. Охлопкова — один из старейших театров Сибири, основанный в 1850 году. Современное здание театра построено в 1897 году по проекту архитектора В.А. Шретера.</p>
            <p>📍ул. Карла Маркса, 14.</p>
			<p>Архитектурный стиль: эклектика с элементами барокко. Здание отличается богатым декором фасадов и прекрасной акустикой зала.</p>
            <p>Один из старейших театров Сибири, основан в 1850 году. Современное здание построено в 1897 году в стиле необарокко.В 1949 году театру было присвоено имя народного артиста СССР Николая Павловича Охлопкова, который начинал здесь свою карьеру. В театре выступали Фёдор Шаляпин и Вера Комиссаржевская. Во время Гражданской войны здесь проходили революционные митинги.</p>
        </div>
    </div>
	
	<div id="sobor-bogoyavleniya" class="modal">
        <div class="modal-content">
            <button class="close-button" onclick="closeModal()">×</button>
            <h2 class="modal-title">Собор Богоявления</h2>
            <img src="./Архитектурные сокровища Иркутска_files/scale_1200" alt="Собор Богоявления" class="modal-image">
			<p>Православный храм, памятник сибирского барокко, построенный в 1718-1746 годах.</p>
            <p>📍ул. Нижняя Набережная, 2.</p>
			<p>Первый деревянный собор построили еще в 1693-1695, но пожар 3 августа 1716 года уничтожил это строение вместе с частью острожной стены и множеством посадских домов. Фундамент нового, каменного собора заложили в июле 1718 года, в мае 1719 года приступили к кладке стен.</p>
            <p>В храме сохранились уникальные фрески XVIII века. Колокольня собора — одно из самых высоких сооружений исторического центра. В советское время был закрыт, в здании размещался хлебозавод.</p>
        </div>
    </div>
	
	<div id="muzey-dekabristov" class="modal">
        <div class="modal-content">
            <button class="close-button" onclick="closeModal()">×</button>
            <h2 class="modal-title">Музей декабристов</h2>
            <img src="./Архитектурные сокровища Иркутска_files/XXXL(1)" alt="Музей декабристов" class="modal-image">
            <p>Историко-мемориальный музей, посвященный жизни декабристов в сибирской ссылке.</p>
            <p>📍ул. Декабрьских Событий, 77 (усадьба Волконских), пер. Волконского, 10 (усадьба Трубецких).</p>
            <p>Коллекция будущего Иркутского музея декабристов начала формироваться в 1925 г., когда к столетию со дня восстания на Сенатской площади в Иркутском музее Революции была создана экспозиция, посвященная декабристам.Состоит из двух усадеб: князей Волконских и Трубецких. Сохранились подлинные вещи, письма и мебель XIX века.</p>
			<p>В доме Волконских бывали Пушкин и другие известные личности. Здесь проходят балы в исторических костюмах.</p>
        </div>
    </div>
	
	<div id="dom-vampilova" class="modal">
        <div class="modal-content">
            <button class="close-button" onclick="closeModal()">×</button>
            <h2 class="modal-title">Дом-музей Вампилова</h2>
            <img src="./Архитектурные сокровища Иркутска_files/18_mart.jpg" alt="Дом-музей Вампилова" class="modal-image">
            <p>Мемориальный музей драматурга Александра Вампилова, расположенный в доме его детства.</p>
            <p>📍ул. Богдана Хмельницкого, 3.</p>
            <p>Культурный центр Александра Вампилова открыт в&nbsp;день 75-летия драматурга 19&nbsp;августа 2012&nbsp;года. Работает по&nbsp;четырём направлениям: Картинная галерея с&nbsp;работами, посвящёнными Иркутску, Байкалу, Александру Вампилову и его окружению. Воссоздана обстановка 1960-х годов, представлены личные вещи писателя. </p>
			<p>Вампилов погиб трагически — утонул в Байкале за два дня до своего 35-летия. Его пьесы («Старший сын», «Утиная охота») до сих пор ставят в театрах.</p>
        </div>
    </div>
	
	<div id="usadba-sukacheva" class="modal">
        <div class="modal-content">
            <button class="close-button" onclick="closeModal()">×</button>
            <h2 class="modal-title">Усадьба Сукачёва</h2>
            <img src="./Архитектурные сокровища Иркутска_files/mtOsEhbbYP4.jpg" alt="Усадьба Сукачёва" class="modal-image">
            <p>Городская усадьба XIX века, принадлежавшая городскому голове В.П. Сукачёву.</p>
            <p>📍ул. Декабрьских Событий, 112.</p>
            <p>В 1920–1930-х годах здесь располагалась школа-коммуна "Новая жизнь". Когда страна покончила с беспризорностью, в усадьбе разместился Дом ребенка, в 1950-х годах —&nbsp;детский сад. В 1986 году усадьба была передана Иркутскому художественному музею. С этого времени ведутся проектные и реставрационные работы по её воссозданию: мемориально-художественная экспозиция, посвященная жизни и деятельности Сукачева с историческим зимним садом. Так же устраиваются временные выставки, проводятся культурные мероприятия.</p>
			<p>В усадьбе бывали Чехов и другие известные гости. В парке сохранились редкие для Сибири деревья.</p>
        </div>
    </div>
	
	<div id="sibirskiy-dvorec" class="modal">
        <div class="modal-content">
            <button class="close-button" onclick="closeModal()">×</button>
            <h2 class="modal-title">Сибирский дворец</h2>
            <img src="./Архитектурные сокровища Иркутска_files/diploma" alt="Сибирский дворец" class="modal-image">
            <p>Сибирский дворец или, как называют его горожане, Белый дом.</p>
            <p>📍бульвар Гагарина, 24.</p>
            <p>Этот особняк был выстроен купцом, первым городским головой Михаилом Васильевичем Сибиряковым в 1792—1799 годах и уже тогда составил яркое украшение города, однако сам купец пожить в нем не успел и оставил его в наследство сыну Ксенофонту. Дом Сибирякова сгорел и обрушился: целые стены вывалились. Для нового строительства руины сгоревшего здания были частично разобраны, частично укреплены; и первый, и второй дом были практически одинаковы. Построен в стиле классицизма, напоминает петербургские дворцы. Сейчас здесь Научная библиотека ИГУ.</p>
			<p>В 1918 году здесь располагалось правительство Колчака. Во дворце хранится уникальная коллекция старинных книг.</p>
        </div>
    </div>
	
	<div id="usadba-shastinyh" class="modal">
        <div class="modal-content">
            <button class="close-button" onclick="closeModal()">×</button>
            <h2 class="modal-title">Усадьба Шастиных</h2>
            <img src="./Архитектурные сокровища Иркутска_files/original.jpg" alt="Усадьба Шастиных" class="modal-image">
            <p>Деревянная усадьба в стиле модерн, построенная в начале XX века для купеческой семьи Шастиных.</p>
            <p>📍ул. Седова, 40.</p>
            <p>Дом купцов Шастиных строился в середине XIX века. &nbsp;Он был выполнен в стиле русского барокко. Первое упоминание о нем относится к 1843 году. Постепенно внешний вид усадьбы менялся, но орнамент при этом становился все красивее и ярче. Нынешний вид усадьба приобрела в 1907 году, когда в домовладение вступил почетный гражданин города Аполос Иванович Шастин. Именно тогда появилась основная часть украшений.</p>
			<p>По инициативе французской ассоциации сохранения мировых памятников, дом купцов Шастиных был внесен в список мирового охраняемого наследия и при поддержке мэрии Иркутска спасен от сноса. 28 августа 1998 года постановлением мэра города на базе усадьбы создается муниципальное учреждение «Дом Европы». Был создан с целью развития и укрепления международных связей Иркутска и стран Европы.В здании сохранились оригинальные интерьеры. Сейчас здесь размещается культурный центр.</p>
        </div>
    </div>
    
    <!-- Остальные модальные окна аналогично -->
    
    <footer>
        <p>© 2025 Архитектурные сокровища Иркутска</p>
        <p>СПАСИБО, ЧТО ПОСЕТИЛИ МОЙ САЙТ</p>
    </footer>
    
    <script>
        function openModal(id) {
            document.getElementById(id).style.display = 'flex';
            document.body.style.overflow = 'hidden';
        }
        
        function closeModal() {
            const modals = document.querySelectorAll('.modal');
            modals.forEach(modal => {
                modal.style.display = 'none';
            });
            document.body.style.overflow = 'auto';
        }
        
        // Закрытие модального окна при клике вне его
        window.onclick = function(event) {
            if (event.target.className === 'modal') {
                closeModal();
            }
        }
        
        // Здесь будет код для загрузки 3D моделей с использованием Three.js или аналогичной библиотеки
        // Например:
        /*
        function load3DModel(containerId, modelPath) {
            // Инициализация сцены, камеры, рендерера
            // Загрузка модели из modelPath
            // Добавление модели в контейнер с id=containerId
        }
        
        // Загрузка моделей для каждого здания
        document.addEventListener('DOMContentLoaded', function() {
            load3DModel('model-moskovskie-vorota', 'models/moskovskie-vorota.glb');
            // и так для всех зданий
        });
        */
    </script>

</body></html>
