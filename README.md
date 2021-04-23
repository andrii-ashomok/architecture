# Нефункциональные требования (NFR)

Основные тезисы: критерии качества / риски / constrains copy

[ISO-25010|https://iso25000.com/index.php/en/iso-25000-standards/iso-25010] (replace ISO/IEC 9126)



- Functional suitability
	- completness
	- correctness
	- appropriate - подходящий
- Performance efficiency - Operational costs
	- resource usage
	- capacity
		- Scalability
			- current & future loads
			- predict load
	- cloud
	- Performance
		- responce time
		- CPU/mem efficient
		- on device
- Compatibility - Interoperability
	- другие медицинские системы
	- наше API
	- мы юзаем API
- Usability
	- понятный = буду пользоваться / не понятный - не буду
	- ошибка человека в использовании
	- не меняется со временем
	- accessibility
	- learn
- Reliability
	- открывается всегда
	- относительно - пока летел, лечение изменили
	- auditing, jourmals - proof
	- Availability
		- critical
		- бизнес не может без софта свои процессы вести (юзеры не видят софт или опционально)
		- бизнес продает софтз
			- юзер не может без софта
		- SLA compliance
		- нет соединения с сервером - offline mode
- Security
	- подмена данных - выпить не то
	- потеря медицинских данных - работа, страховка
	- что пьют
	- просто увели пароли
	- intergity - fk
- Maintainability
	- modular
	- reusable
	- Modifiability
		- by user
		- by developer
			- в рамках SA
			- выход на рамки
		- by admin
	- Testability
		- как проверить расписание unit tests
		- acceptance tests
		- is it working now? operational
	- licenses
	- team
	- rare specialists
- Portability
	- mobile (зачем vs PWA как - круто)
	- сервер - переезд между облаками
	- пережить обновление 3 версий linux
	- внешне либы (такие же тнебования)
	- reinstall on new system
	- ci/cd + инструкция по развертыванию ci/cd
	- docker
	- java vs c++
	- p not code - dart, js
