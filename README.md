# Ansible role Bareos storage

Ansible role for installing and configuring Bareos remote/local storage on a target host.

## Getting Started

Check out my [Bareos director role](https://github.com/vdzhorov/ansible-role-bareos-director) for more complete documentation.

### Configuring the storage

In order to add a new storage, you will need to:

* Have the storage present in your inventoy file
* Properly configure your *bareos_storage.yml* group_vars.

### Example bareos_storage.yml group_vars

```

bareos_max_concurrent_jobs: 5
bareos_max_bandwidth_per_job: "50 m/s"

bareos_archive_type: "File"
bareos_archive_device: "/var/lib/bareos/storage"
```

## Built With

 [Ansible 2.8](https://docs.ansible.com/ansible/2.8/index.html) - Ansible 2.8

## Built With

* [Ansible 2.8](https://docs.ansible.com/ansible/latest/roadmap/ROADMAP_2_8.html) - Ansible 2.8

## Authors

* **Valentin Dzhorov** - *Initial work* - [vdzhorov](https://github.com/vdzhorov)

## Company
* **Delta.BG**

## License

This project is licensed under the MIT License.
