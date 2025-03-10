<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Поздравление с 8 марта</title>
    <style>
        body {
            background-color: pink;
            font-family: Arial, sans-serif;
            text-align: center;
            padding: 50px;
        }
        .container {
            background-color: white;
            border-radius: 10px;
            padding: 20px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
            display: inline-block;
            width: 80%;
            max-width: 600px;
        }
        h1 {
            color: #ff69b4;
        }
        .name-list {
            margin: 20px 0;
        }
        .name-list button {
            background-color: #ff69b4;
            color: white;
            padding: 10px 20px;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            margin: 5px;
        }
        .name-list button:hover {
            background-color: #ff1493;
        }
        .cute-elements {
            margin-top: 20px;
            font-size: 24px;
        }
    </style>
    <script>
        function showGreeting(name) {
            const container = document.querySelector('.container');
            let greetingText = '';

            switch (name) {
                case 'Татьяна Владимировна':
                    greetingText = 'Здравствуйте Татьяна Владимировна, это поздравление с 8 марта специально для вас, вы лучший классный руководитель<3!';
                    break;
                case 'Полина Асташенко':
                    greetingText = 'Привет Полина Асташенко, поздравляем вас с Международным женским днем! Пусть в твоей жизни всегда будет солнце, цветы и радость!';
                    break;
                case 'Полина Дикоп':
                    greetingText = 'Дорогая Полина Дикоп, поздравляем вас с Международным женским днем!, С праздником! Пусть твои мечты сбываются, а настроение всегда будет весенним!';
                    break;
                case 'Полина Федякина':
                    greetingText = 'Полина Федякина, к вам поздравление от Витали, цитирую "С 8 Марта! Пусть в твоей жизни будет больше радости, любви и тепла. Пусть каждый день приносит что-то хорошее, а рядом всегда будут люди, которые ценят и поддерживают тебя. Будь счастлива!"';
                    break;
                case 'Сати':
                    greetingText = 'Сати, к вам поздровление от Артема Щеголива, цитирую"С 8 Марта тебя Улыбайся смейся звонко, Никогда не унывай И пятерки получай. Пусть исполнятся желания,Все надежды и мечтания. Пусть царит во всём удача, И везение в придачу <br> а еще поздравление от Тимофея, цитирую "С 8 Марта, Пусть каждый день будет радостным, как весеннее солнце, а мечты исполняются легко и быстро!"';
                    break;
                case 'Сумая':
                    greetingText = 'Сумая, к вам поздравление от Севы, цитирую"Сумая  поздравляю тебя с 8 марта желаю тебе всего самого лучшего"';
                    break;
                case 'Женя':
                    greetingText = 'Женя, к вам поздравление от Саши Филиппова, цитирую "ты самая хорошая, желаю тебе счастья"';
                    break;
                case 'Яна Гункель':
                    greetingText = 'Яна Гункель, к вам поздравление от Сергея, цитирую  "Оставайся такой же доброй, весёлой и чудесной! С праздником!"';
                    break;
                case 'Яна Романова':
                    greetingText = 'Яна Романова, к вам поздравление от Димы, цитирую "Мира, счастья, красоты! Чтобы было всё отлично, Чтоб сбывались все мечты!"';
                    break;
                case 'Элина':
                    greetingText = 'Дорогая Элина, поздравляем вас с Международным женским днем! Желаем волшебного настроения, ярких эмоций и весёлых моментов!';
                    break;
                case 'София':
                    greetingText = 'Дорогая София, Пусть эта весна принесёт тебе только радость, тепло и вдохновение!';
                    break;
                case 'Малика':
                    greetingText = 'Дорогая Малика, Будь самой счастливой, самой лучшей и самой любимой! С 8 Марта!';
                    break;
                case 'Рамина':
                    greetingText = 'Рамина, к вам поздравление от Вовы Бутяйкина, цитирую "Поздравляю с женским днем)  пусть везёт тебе во всем. С 8 марта  поздравляю тебя пусть твои мечты забываются"';
                    break;
                case 'Настя':
                    greetingText = 'Дорогая Настя, поздравляем вас с Международным женским днем! Пусть в твоей жизни всегда будет солнце, цветы и радость!';
                    break;
                default:
                    greetingText = 'Дорогая, поздравляем вас с Международным женским днем!';
            }

            container.innerHTML = `
                <h1>Поздравление, ${name}!</h1>
                <p>${greetingText}</p>
                <div class="cute-elements">
                    &#10084; &#127800; &#128149; &#127801; &#128156;
                </div>
                <button onclick="location.reload()">Назад</button>
            `;
        }
    </script>
</head>
<body>
    <div class="container">
        <h1>Поздравление с 8 марта</h1>
        <p>7В класс</p>
        <p>Выберите свое имя, чтобы увидеть поздравление:</p>
        <div class="name-list">
            <button onclick="showGreeting('Татьяна Владимировна')">Татьяна Владимировна</button>
            <button onclick="showGreeting('Элина')">Элина</button>
            <button onclick="showGreeting('Женя')">Женя</button>
            <button onclick="showGreeting('Малика')">Малика</button>
            <button onclick="showGreeting('Настя')">Настя</button>
            <button onclick="showGreeting('Полина Асташенко')">Полина Асташенко</button>
            <button onclick="showGreeting('Полина Дикоп')">Полина Дикоп</button>
            <button onclick="showGreeting('Полина Федякина')">Полина Федякина</button>
            <button onclick="showGreeting('Рамина')">Рамина</button>
            <button onclick="showGreeting('Сати')">Сати</button>
            <button onclick="showGreeting('София')">София</button>
            <button onclick="showGreeting('Сумая')">Сумая</button>
            <button onclick="showGreeting('Яна Гункель')">Яна Гункель</button>
            <button onclick="showGreeting('Яна Романова')">Яна Романова</button>
        </div>
    </div>
</body>
</html>
