<h1>Программа "ход животных"</h1>

<p>Необходимо добавить на хост систему запись в sudo crontab -e:
<pre>* * * * * docker exec zoo-app bash -c "php artisan schedule:run"</pre>
Это нужно, чтобы работал Laravel Scheduler.

Далее каждую минуту будет запускаться ход животных, а в базу будут писаться изменения свойств животных.

Как поднять на linux:
Клонировать репозиторий, в папке прописать <pre>make install</pre>
</p>
<img src="screenshots/screen1.png">
<img src="screenshots/screen2.png">