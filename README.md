# logging_stuff

Роли для установки и конфигурирования сервисов Prometheus, Node Exporter, FluentBit, а также Elasticsearch и Kibana.
На управляющей машине необходимо наличие ansible, а также ролей geerlingguy.kibana, geerlingguy.elasticsearch и geerlingguy.java.
Основной плейбук - setup_monitoring.yml. Устанавливает все сервисы: ansible-playbook -i hosts setup_monitoring.yml
Перечитывание конфигурации: ansible-playbook -i hosts setup_monitoring.yml --tags configure
