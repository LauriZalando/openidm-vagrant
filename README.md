# openidm-vagrant
OpenIDM Vagrant box including Oracle/Java 7

    git clone https://github.com/zalando/openidm-vagrant.git
    vagrant up

Your are now done. Visit the UI here:
https://192.168.33.12:8443/openidmui/index.html#login/

Full docu of OpenIDM here: http://docs.forgerock.org/en/openidm/3.1.0/install-guide/index.html

## Troubleshooting

*OpenIDM Start*
Sometimes the bootstrap script does not like to recognize the inserted crontab. Should this be the case just do a `sudo /opt/openidm/startup.sh` to start OpenIDM from within vagrant.
Or you uncomment the cron insertion in the bootstrap file and do a `vagrant destroy` and `vagrant up`.

*The box 'chef/ubuntu-14.04' could not be found.*
`vagrant box add chef/ubuntu-14.04`
