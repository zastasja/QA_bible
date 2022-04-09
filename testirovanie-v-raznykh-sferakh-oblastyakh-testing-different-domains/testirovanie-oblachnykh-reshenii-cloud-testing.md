# Тестирование облачных решений (Cloud testing)

**Облачные вычисления** - это предоставление по требованию вычислительных услуг, таких как серверы, хранилища данных, базы данных, сети, программное обеспечение и т. д., как правило, через Интернет и с оплатой по мере использования.

Облако построено на одном или нескольких серверах, объединенных между собой системами виртуализации. Также технологии виртуализации позволяют разделить аппаратные мощности на части, которые соответствуют текущим потребностям пользователей, обращающихся к аппаратному обеспечению, как к услуге. В результате пользователь переходит от приобретения, управления и амортизации аппаратных ресурсов к покупке серверного времени, дискового пространства, сетевой пропускной способности, необходимой для выполнения своих задач.

![https://www.softwaretestingmaterial.com/wp-content/uploads/2020/09/Cloud-Computing.png?ezimgfmt=ng:webp/ngcb5](https://www.softwaretestingmaterial.com/wp-content/uploads/2020/09/Cloud-Computing.png?ezimgfmt=ng:webp/ngcb5)

В облачных вычислениях различают несколько видов сервисов, для удобства в их обозначении используют аббревиатуру «as a service», то есть «как сервис», или «в виде услуги»:

* **SaaS** (Software as a service; программное обеспечение как услуга) - модель предоставления программного обеспечения, при которой поставщик разрабатывает веб-приложение и самостоятельно управляет им, предоставляя пользователям доступ к нему через интернет;
* **PaaS** (Platform as a service; платформа как услуга) - это предоставление интегрированной платформы для разработки, тестирования, развертывания и поддержки приложений как услуги. В облаке функционирует некоторый набор программ, основных сервисов и библиотек, на основе которых предлагается разрабатывать свои приложения. Помимо этого, под PaaS понимают также и отдельные части сложных систем, например системы базы данных или коммуникаций;
* **IaaS** (Infrastructure as a service; инфраструктура как услуга) - это предоставление аппаратных ресурсов, как правило, объединенных на основе виртуализации, как услуги. IaaS состоит из трех основных компонентов - аппаратное обеспечение (серверы, системы хранения данных, клиентские системы, сетевое оборудование), операционные системы и системное ПО (средства виртуализации, автоматизации, основные средства управления ресурсами), и связующее ПО для управления аппаратным и программным обеспечением.

![https://www.mindk.com/blog/wp-content/uploads/2018/11/paas-saas-iaas.png](https://www.mindk.com/blog/wp-content/uploads/2018/11/paas-saas-iaas.png)

**Тестирование SaaS**

Это процесс тестирования программного обеспечения, в котором программное приложение, созданное в рамках модели «Программное обеспечение как услуга», тестируется на соответствие как функциональным, так и нефункциональным требованиям. Целью тестирования SaaS является обеспечение качества путем тестирования безопасности данных, целостности, производительности, совместимости и масштабируемости программного приложения.

Облачное тестирование фокусируется на основных компонентах, таких как:

* Приложение: охватывает тестирование функций, сквозные бизнес-процессы, безопасность данных, совместимость с браузерами и т. д.;
* Сеть : включает в себя тестирование различных пропускных способностей сети, протоколов и успешной передачи данных по сетям;
* Инфраструктура : охватывает тестирование аварийного восстановления, резервное копирование, безопасное соединение и политики хранения. Инфраструктура должна быть проверена на соответствие нормативным требованиям.

Другие типы тестирования в облаке включают:

* Performance;
* Availability;
* Compliance;
* Security;
* Scalability;
* Multi-tenancy;
* Live upgrade testing.

**Примеры тест-кейсов**:

* **Performance Testing**:
  * Сбой из-за одного действия пользователя в облаке не должен влиять на производительность других пользователей;
  * Ручное или автоматическое масштабирование не должно вызывать сбоев;
  * На всех типах устройств производительность приложения должна оставаться одинаковой;
  * Избыточное резервирование на стороне поставщика не должно снижать производительность приложения.
* **Security Testing**:
  * Только авторизованный клиент может получить доступ к данным;
  * Данные должны быть хорошо зашифрованы;
  * Данные должны быть полностью удалены, если они не используются клиентом;
  * Администрация со стороны поставщиков не должна получать доступ к данным клиентов;
  * Проверьте различные настройки безопасности, такие как брандмауэр, VPN, антивирус и т. д.
* **Functional testing**:
  * Допустимый ввод должен давать ожидаемые результаты;
  * Сервис должен правильно интегрироваться с другими приложениями;
  * Система должна отображать тип учетной записи клиента при успешном входе в облако;
  * Когда клиент решил переключиться на другие службы, работающая служба должна автоматически закрыться.
* **Interoperability & Compatibility Testing**:
  * Проверка требований совместимости тестируемой системы;
  * Проверьте совместимость браузера в облачной среде;
  * Определите Дефект , который может возникнуть при подключении к облаку;
  * Любые неполные данные в облаке не должны переноситься;
  * Убедитесь, что приложение работает на другой облачной платформе;
  * Протестируйте приложение во внутренней среде, а затем разверните его в облачной среде.
* **Network Testing**:
  * Тест протокола, отвечающий за подключение к облаку;
  * Целостность данных при передаче;
  * Правильность подключения к сети;
  * Проверьте, не отбрасываются ли пакеты брандмауэром с обеих сторон.
* **Load and Stress Testing**:
  * Проверка служб при доступе нескольких пользователей к облачным службам;
  * Определите дефект, ответственный за сбой оборудования или среды;
  * Проверьте, не выходит ли система из строя при увеличении удельной нагрузки;
  * Проверить, как система меняется со временем под определенной нагрузкой.

Источники:

* [Облачные вычисления (обзор)](https://habr.com/ru/post/69038/)
* [What is Cloud Testing? SaaS Testing Tutorial](https://www.guru99.com/cloud-testing-tutorial-with-saas-testing-primer.html)

Доп. материал:

* [Введение в Облачные Вычисления для Всех от Инженера Microsoft, Ex-Amazon](https://habr.com/ru/post/585064/)
* [Хаб “Облачные вычисления” на хабре](https://habr.com/ru/hub/cloud\_computing/)
* [SaaS Testing Guide: What You Should Know](https://www.softwaretestingmaterial.com/saas-testing/)