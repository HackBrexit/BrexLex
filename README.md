# BrexLex

---

## Contains

* MySQL
* Apache
* Python

## Dependencies

* Vagrant

---

## Usage

1. Clone repo `git clone git@github.com:HackBrexit/BrexLex.git`
2. Vagrant up (use `--debug` for more verbose output from **vagrant**)
3. Access **web** on `http://192.168.50.99/` (dont forget to add a host entry)
4. Access **mysql** on `192.168.50.99:3306`

Files **mounted** on `/vagrant` & **apache** serves `/vagrant`

### Vagrant commands

* create or turn on VM `vagrant up`
* ssh on to VM `vagrant ssh`
* turn off VM `vagrant halt`
* status of VM `vagrant status`
* destroy VM `vagrant destroy`

---

## Customisation


### System wide **apt** packages

Edit `ansible/vars/all.yml` and add to collect on line 4, looks like `packages: [vim, htop, iotop]`

*Or variables, mysql passwords etc*

### What **ansible** installs (eg. apache)

Edit `ansible/playbook.yml` *comment/uncomment* **roles** collection.
