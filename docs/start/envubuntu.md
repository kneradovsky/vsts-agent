

# ![Ubuntu](../res/ubuntu_med.png) Ubuntu System Pre-requisites

## Versions

Tested on 16.04 LTS (Yosemite) and 14.04 LTS (El Capitan).  Not domain joined.  

16.04 is recommended since latest and supports SystemD for runnings as a service.

## Git

If you use git, git >= 2.9.0 is a pre-requisite for Ubuntu agents.

[Install Latest Git on Ubuntu](http://askubuntu.com/questions/568591/how-do-i-install-the-latest-version-of-git-with-apt/568596)

```bash
$ sudo apt-add-repository ppa:git-core/ppa
$ sudo apt-get update
$ sudo apt-get install git
```

## Optionally Java if TfsVc

The agent distributes team explorer everywhere.

But, if you are using TfsVc, install Oracle Java 1.6+ as TEE uses Java.

## Etc

There was an assertion that on Ubuntu 16 this was needed.  We didn't need.  Adding in case it helps someone.  We will verify on clean build and dev boxes.

```bash
apt-get install libcurl4-openssl-dev
```

