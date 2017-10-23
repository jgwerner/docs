## Install and Run 3Blades

Now that your local and remote environments have been configured you are ready to run the **ansible playbook** to install dependencies and launch 3Blades.

You should run the ansible playbook from the `onpremise` folder root cloned from [https://github.com/3blades/onpremise](https://github.com/3blades/onpremise). Some arguments are required, others are optional. Refer to [Configuration](../docs/onpremise-configuration) section for additional configuration options.

```
$ ./install.sh
```
The install script will prompt you to confirm `license` agreement, `server IP address` and `private key` for SSH access. Once these values are confirmed, the script kicks off an ansible script to set up 3Blades. You may also manually run the ansible script like so:

```
ansible-playbook -s hosts full-stack-deployment.yml \
--e "force_pull_images=yes \
app_secret_key=your_secret_key_here \
tbs_host=your_server_ip_or_domain"
```

!!! tip "Additional global environment options"
    To view a full list of possible environment options, you may want to take a look at [the yaml file where all default values](https://github.com/3Blades/onpremise/blob/master/group_vars/all.yml) are defined.
