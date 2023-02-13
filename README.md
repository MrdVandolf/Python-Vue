<h1>Как запустить этот проект</h1>

<h3>

<ol>
<li>
<p>Скачайте проект при помощи команды</p>
<p>git clone</p>

</li>
<li>
<p>Создайте файл .env и заполните его данными из файла .env.example</p>
</li>

<li>
<p>В качестве POSTGRES_PORT и POSTGRES_USER укажите произвольные значения на ваше усмотрение (без спец. символов)</p>
</li>


<li>
<p>Запустите проект командой docker-compose up</p>
</li>

<li>
<p>После запуска проект будет доступен двумя частями: в качестве бэкенда и фронтэнда</p>
</li>
<li>
<p>Фронтэнд будет доступен по порту VUE_PORT из файла .env</p>
<p>Через него можно создавать и изменять сотрудников в компании</p>
<p>Изначально база данных компании пуста, поэтому на странцие будет находиться только кнопка "Создать"</p>
</li>
<li>
<p>Бэкенд будет доступен по порту API_PORT из файла .env</p>
<p>На него можно делать три типа запросов</p>
<ul>
    <li>GET /employees/all - возвращает полную иерархию сотрудников в компании</li>
    <li>POST /employees/new - создает нового сотрудника</li>
    <li>POST /employees/change - изменяет существующего сотрудника (или говорит об ошибке и не вносит изменений)</li>
</ul>

</li>

</ol>

</h3>