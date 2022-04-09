# Тестирование методом серого ящика (Grey Box Testing)

Тестирования методом серого ящика вообще нет в ISTQB, тем не менее много где можно встретить упоминания этого типа тестирования. В целом оно определяется как метод тестирования ПО, который предполагает комбинацию White Box и Black Box подходов или как дополненный черный ящик. Т.е., внутреннее устройство/код известны/используется лишь частично, и, например, имея доступ к внутренней структуре и алгоритмам работы ПО, можно написать более эффективные тест-кейсы, но само тестирование проводится с помощью техники черного ящика, то есть, с позиции пользователя.

Примеры: тестирование с проверкой корректности записей в БД; работа с логами и метриками для поиска root cause проблем.

**Техники**:

* **Матричное тестирование (Matrix Testing)**: разработчики предоставляют все переменные в программе, а также связанные с ними технические и бизнес-риски. Методика матричного тестирования проверяет риски, определенные разработчиками. Матричный метод устанавливает все используемые переменные в программе. Этот метод помогает идентифицировать и удалять переменные, которые не используются в программе, и, в свою очередь, помогает увеличить скорость работы программного обеспечения;
* **Регрессионное тестирование (Regression Testing)**: регрессионное тестирование выполняется, когда в программное обеспечение вносятся какие-либо изменения или исправляется какой-либо дефект. Это делается для того, чтобы новое изменение или исправление не повлияло на существующие функциональные возможности программного обеспечения;
* **Тестирование ортогональных массивов или OAT (Orthogonal Array Testing or OAT)**: этот метод тестирования больше используется для сложных функций или приложений, когда требуется максимальное покрытие кода с минимальным количеством test cases и имеет большие тестовые данные с n числом комбинаций;
* **Pattern testing**: тестирование по образцу выполняется на основе предыдущих дефектов, обнаруженных в ПО. Записи о дефектах анализируются на предмет причин дефектов, и создаются test cases на основе этих дефектов и их причин;

Источник: [Grey Box Testing Tutorial With Examples, Tools And Techniques](https://www.softwaretestinghelp.com/grey-box-testing-tutorial/)