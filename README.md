Создание gutenberg блока Summary. 
Одна из классных задач в котором я использовал InnerBlock ( Block Api https://developer.wordpress.org/block-editor/reference-guides/block-api/ ). 
Как я делал эту задачу: Я создал и подключил плагин, после в этом плагине я создал среду разработки с помощью wp-env (https://developer.wordpress.org/block-editor/getting-started/devenv/get-started-with-wp-env/).
В плагине в главном файле php я подключил я создал функцию и в функции я подключил все файлы которые находятся в папке build (register_block_type( __DIR__ . '/build' );).
Созданную функцию я подключил через хук init.

Перешёл на написание JS. В папке src есть три файла js(edit.js - для написание функции которая возвращает блок, save.js - которая как я понял выполняет сохранение блока в БД, index.js - для import js и scss.

Ну и конечно же стили которые пишу на scss.

Использовал: wp-env, JS, SCSS
