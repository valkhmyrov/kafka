Inventory file must content two groups: [zookeeper] and [kafka]. In case of single node installation server must be member of two groups simultaneously.


How to start:
  ansible-playbook -i inventory/hosts install_kafka.yml --extra-vars '{"kafka_version": "2.13-2.4.1"}'

