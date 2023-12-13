# test-<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Магазин - Xiaomi Watch S1 Pro</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f4f4f4;
        }

        header {
            background-color: #333;
            color: #fff;
            padding: 1em;
            text-align: center;
        }

        section {
            display: flex;
            flex-wrap: wrap;
            justify-content: space-around;
            padding: 2em;
        }

        .product {
            background-color: #fff;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
            margin: 1em;
            padding: 1em;
            text-align: center;
            width: 300px;
        }

        button {
            background-color: #4CAF50;
            color: white;
            padding: 10px 15px;
            border: none;
            border-radius: 5px;
            cursor: pointer;
        }

        button:hover {
            background-color: #45a049;
        }
    </style>
</head>
<body>

<header>
    <h1>Онлайн-магазин - Xiaomi Watch S1 Pro</h1>
</header>

<section>
    <div class="product">
        <h2>Xiaomi Watch S1 Pro, Silver</h2>
        <p>Тип разъема для зарядки: Магнитное крепление</p>
        <p>Тип элемента питания: Несъемные</p>
        <p>Активное время работы, ч: 336</p>
        <p>Емкость аккумулятора, mAh: 500</p>
        <p>Технология аккумулятора: Li-Polymer</p>
        <p>Связь: Bluetooth - Да, Поддержка Wi-Fi - Да</p>
        <p>Основные характеристики: Вибрация - Да, Поддержка платформ - Android, iOS</p>
        <p>Комплектация: Часы, Кабель для зарядки, Руководство пользователя</p>
        <p>Серия: Xiaomi Watch S1 Pro</p>
        <p>Экран: Сенсорный экран - Да, Диагональ, дюйм: 1.47, Разрешение: 480 x 480</p>
        <p>Влагозащита: 5ATM</p>
        <p>Габариты: Высота, мм: 46, Ширина, мм: 46, Толщина, мм: 11.3</p>
        <p>Вес, гр: 120</p>
        <p>Цена: $120</p>
        <p>Количество товара для покупки: <input type="number" id="quantity" value="1" min="1"></p>
        <button onclick="addToCart('Xiaomi Watch S1 Pro', 120)">Добавить в корзину</button>
    </div>
</section>

<script>
    let cart = [];
    let total = 0;

    function addToCart(product, price) {
        const quantity = parseInt(document.getElementById('quantity').value);
        cart.push({ product, price, quantity });
        total += price * quantity;
        alert(`Товар "${product}" (${quantity} шт.) добавлен в корзину. Общая стоимость: $${total}`);
    }
</script>

</body>
</html>
