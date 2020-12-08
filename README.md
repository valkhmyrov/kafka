Try:
  ansible-playbook -i inventory/hosts install_kafka.yml --extra-vars '{"kafka_version": "2.13-2.4.1"}'