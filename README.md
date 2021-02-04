Inventory file must contain two groups: [zookeeper] and [kafka]. In case of single node installation server must be member of two groups simultaneously.
Inventory example:

    [kafka]
    kafka_1.domain.com
    kafka_2.domain.com
    kafka_3.domain.com

    [zookeeper]
    zookeeper_1.domain.com
    zookeeper_2.domain.com
    zookeeper_3.domain.com




How to start:

    ansible-playbook -i inventory/hosts install_kafka.yml --extra-vars '{"kafka_version": "2.13-2.4.1", "endpoint_url": "http://dev01-obj.corp.dev"}'

