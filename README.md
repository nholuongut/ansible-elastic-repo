# A role for deploying softare repository from [elastic.co](http://www.elastic.co). It provide Elastic Search, Logstash and Kibana software suite.

![](https://i.imgur.com/waxVImv.png)
### [View all Roadmaps](https://github.com/nholuongut/all-roadmaps) &nbsp;&middot;&nbsp; [Best Practices](https://github.com/nholuongut/all-roadmaps/blob/main/public/best-practices/) &nbsp;&middot;&nbsp; [Questions](https://www.linkedin.com/in/nholuong/)
<br/>

Supports
--------

Supported targets:

- Debian 8 "Jessie"
- Debian 9 "Stretch"
- Debian 10 "Buster"
- Ubuntu 16.04 "Xenial"
- Ubuntu 18.04 "Bionic"
- RedHat EL / CentOS 6
- RedHat EL / CentOS 7

Role Variables
--------------

This roles comes preloaded with almost every available default. You can override each one in your hosts/group vars, in your inventory, or in your play. See the annotated defaults in `defaults/main.yml` for help in configuration. All provided variables start with `elastic_repo__`.

- `elastic_repo__branch: 7.x` - Branch of repository to setup on the host. curently supported: 5.x, 6.x, 7.x.
- `elastic_repo__local_gpgkey: false` - Use local copy of elastic.co repository GPG key, shipped with the role. Can be usefull for hosts that don't have direct access to internet (using apt-proxy).

Usage
-----

Clone this repo into your roles directory:

    $ git clone https://github.com/nholuongut/ansible-elastic-repo.git

Or use Ansible galaxy requirements.yml

    # nholuong.elastic_repo galaxy role

And add it to your play's roles:

    - hosts: ...
      roles:
        - nholuong.elastic_repo

You can also use the role as a playbook. You will be asked which hosts to provision, and you can further configure the play by using `--extra-vars`.

    $ ansible-playbook -i inventory --extra-vars='{...}' main.yml


Still to do
-----------

# 🚀 I'm are always open to your feedback.  Please contact as bellow information:
### [Contact ]
* [Name: nho Luong]
* [Skype](luongutnho_skype)
* [Github](https://github.com/nholuongut/)
* [Linkedin](https://www.linkedin.com/in/nholuong/)
* [Email Address](luongutnho@hotmail.com)

![](https://i.imgur.com/waxVImv.png)
![](Donate.png)
[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/nholuong)

# License
* Nho Luong (c). All Rights Reserved.🌟


