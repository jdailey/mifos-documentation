# Installing docker & docker-compose

### Installing docker-compose

```text
> sudo apt-get install docker-compose
Hit:1 http://azure.archive.ubuntu.com/ubuntu bionic InRelease
Get:2 http://azure.archive.ubuntu.com/ubuntu bionic-updates InRelease [88.7 kB]
Get:3 http://azure.archive.ubuntu.com/ubuntu bionic-backports InRelease [74.6 kB                                    ]
Hit:4 http://security.ubuntu.com/ubuntu bionic-security InRelease
Fetched 163 kB in 0s (403 kB/s)
Reading package lists... Done
notadmin@large-dfsp-channels:~$ sudo apt-get install docker-compose
Reading package lists... Done
Building dependency tree
Reading state information... Done
The following package was automatically installed and is no longer required:
  grub-pc-bin
Use 'sudo apt autoremove' to remove it.
The following additional packages will be installed:
  bridge-utils cgroupfs-mount containerd docker.io
  golang-docker-credential-helpers libsecret-1-0 libsecret-common pigz
  python-asn1crypto python-backports.ssl-match-hostname python-cached-property
  python-certifi python-cffi-backend python-chardet python-cryptography
  python-docker python-dockerpty python-dockerpycreds python-docopt
  python-enum34 python-funcsigs python-functools32 python-idna
  python-ipaddress python-jsonschema python-mock python-openssl python-pbr
  python-pkg-resources python-requests python-six python-texttable
  python-urllib3 python-websocket python-yaml runc ubuntu-fan
Suggested packages:
  ifupdown aufs-tools debootstrap docker-doc rinse zfs-fuse | zfsutils
  python-cryptography-doc python-cryptography-vectors python-enum34-doc
  python-funcsigs-doc python-mock-doc python-openssl-doc python-openssl-dbg
  python-setuptools python-socks python-ntlm
The following NEW packages will be installed:
  bridge-utils cgroupfs-mount containerd docker-compose docker.io
  golang-docker-credential-helpers libsecret-1-0 libsecret-common pigz
  python-asn1crypto python-backports.ssl-match-hostname python-cached-property
  python-certifi python-cffi-backend python-chardet python-cryptography
  python-docker python-dockerpty python-dockerpycreds python-docopt
  python-enum34 python-funcsigs python-functools32 python-idna
  python-ipaddress python-jsonschema python-mock python-openssl python-pbr
  python-pkg-resources python-requests python-six python-texttable
  python-urllib3 python-websocket python-yaml runc ubuntu-fan
0 upgraded, 38 newly installed, 0 to remove and 16 not upgraded.
Need to get 65.8 MB of archives.
After this operation, 329 MB of additional disk space will be used.
Do you want to continue? [Y/n]
Get:1 http://azure.archive.ubuntu.com/ubuntu bionic/universe amd64 pigz amd64 2.                                    4-1 [57.4 kB]
Get:2 http://azure.archive.ubuntu.com/ubuntu bionic/main amd64 bridge-utils amd6                                    4 1.5-15ubuntu1 [30.1 kB]
Get:3 http://azure.archive.ubuntu.com/ubuntu bionic/universe amd64 cgroupfs-moun                                    t all 1.4 [6320 B]
Get:4 http://azure.archive.ubuntu.com/ubuntu bionic-updates/universe amd64 runc                                     amd64 1.0.0~rc10-0ubuntu1~18.04.2 [2000 kB]
Get:5 http://azure.archive.ubuntu.com/ubuntu bionic-updates/universe amd64 conta                                    inerd amd64 1.3.3-0ubuntu1~18.04.2 [21.7 MB]
Get:6 http://azure.archive.ubuntu.com/ubuntu bionic/universe amd64 python-backpo                                    rts.ssl-match-hostname all 3.5.0.1-1 [7024 B]
Get:7 http://azure.archive.ubuntu.com/ubuntu bionic/main amd64 python-pkg-resour                                    ces all 39.0.1-2 [128 kB]
Get:8 http://azure.archive.ubuntu.com/ubuntu bionic/universe amd64 python-cached                                    -property all 1.3.1-1 [7568 B]
Get:9 http://azure.archive.ubuntu.com/ubuntu bionic/main amd64 python-six all 1.                                    11.0-2 [11.3 kB]
Get:10 http://azure.archive.ubuntu.com/ubuntu bionic/main amd64 libsecret-common                                     all 0.18.6-1 [4452 B]
Get:11 http://azure.archive.ubuntu.com/ubuntu bionic/main amd64 libsecret-1-0 am                                    d64 0.18.6-1 [94.6 kB]
Get:12 http://azure.archive.ubuntu.com/ubuntu bionic/universe amd64 golang-docke                                    r-credential-helpers amd64 0.5.0-2 [444 kB]
Get:13 http://azure.archive.ubuntu.com/ubuntu bionic/universe amd64 python-docke                                    rpycreds all 0.2.1-1 [4138 B]
Get:14 http://azure.archive.ubuntu.com/ubuntu bionic/main amd64 python-certifi a                                    ll 2018.1.18-2 [144 kB]
Get:15 http://azure.archive.ubuntu.com/ubuntu bionic/main amd64 python-chardet a                                    ll 3.0.4-1 [80.3 kB]
Get:16 http://azure.archive.ubuntu.com/ubuntu bionic/main amd64 python-idna all                                     2.6-1 [32.4 kB]
Get:17 http://azure.archive.ubuntu.com/ubuntu bionic-updates/main amd64 python-u                                    rllib3 all 1.22-1ubuntu0.18.04.1 [85.9 kB]
Get:18 http://azure.archive.ubuntu.com/ubuntu bionic-updates/main amd64 python-r                                    equests all 2.18.4-2ubuntu0.1 [58.5 kB]
Get:19 http://azure.archive.ubuntu.com/ubuntu bionic/universe amd64 python-webso                                    cket all 0.44.0-0ubuntu2 [30.7 kB]
Get:20 http://azure.archive.ubuntu.com/ubuntu bionic/main amd64 python-ipaddress                                     all 1.0.17-1 [18.2 kB]
Get:21 http://azure.archive.ubuntu.com/ubuntu bionic/universe amd64 python-docke                                    r all 2.5.1-1 [69.0 kB]
Get:22 http://azure.archive.ubuntu.com/ubuntu bionic/universe amd64 python-docke                                    rpty all 0.4.1-1 [10.8 kB]
Get:23 http://azure.archive.ubuntu.com/ubuntu bionic/universe amd64 python-docop                                    t all 0.6.2-1build1 [25.6 kB]
Get:24 http://azure.archive.ubuntu.com/ubuntu bionic/main amd64 python-enum34 al                                    l 1.1.6-2 [34.8 kB]
Get:25 http://azure.archive.ubuntu.com/ubuntu bionic/main amd64 python-functools                                    32 all 3.2.3.2-3 [10.8 kB]
Get:26 http://azure.archive.ubuntu.com/ubuntu bionic/main amd64 python-funcsigs                                     all 1.0.2-4 [13.5 kB]
Get:27 http://azure.archive.ubuntu.com/ubuntu bionic/main amd64 python-pbr all 3                                    .1.1-3ubuntu3 [53.7 kB]
Get:28 http://azure.archive.ubuntu.com/ubuntu bionic/main amd64 python-mock all                                     2.0.0-3 [47.4 kB]
Get:29 http://azure.archive.ubuntu.com/ubuntu bionic/main amd64 python-jsonschem                                    a all 2.6.0-2 [31.5 kB]
Get:30 http://azure.archive.ubuntu.com/ubuntu bionic/universe amd64 python-textt                                    able all 0.9.1-1 [8160 B]
Get:31 http://azure.archive.ubuntu.com/ubuntu bionic/main amd64 python-yaml amd6                                    4 3.12-1build2 [115 kB]
Get:32 http://azure.archive.ubuntu.com/ubuntu bionic/universe amd64 docker-compo                                    se all 1.17.1-2 [76.3 kB]
Get:33 http://azure.archive.ubuntu.com/ubuntu bionic-updates/universe amd64 dock                                    er.io amd64 19.03.6-0ubuntu1~18.04.1 [39.9 MB]
Get:34 http://azure.archive.ubuntu.com/ubuntu bionic/main amd64 python-asn1crypt                                    o all 0.24.0-1 [72.7 kB]
Get:35 http://azure.archive.ubuntu.com/ubuntu bionic/main amd64 python-cffi-back                                    end amd64 1.11.5-1 [63.4 kB]
Get:36 http://azure.archive.ubuntu.com/ubuntu bionic-updates/main amd64 python-c                                    ryptography amd64 2.1.4-1ubuntu1.3 [221 kB]
Get:37 http://azure.archive.ubuntu.com/ubuntu bionic/main amd64 python-openssl a                                    ll 17.5.0-1ubuntu1 [41.3 kB]
Get:38 http://azure.archive.ubuntu.com/ubuntu bionic/main amd64 ubuntu-fan all 0                                    .12.10 [34.7 kB]
Fetched 65.8 MB in 8s (7919 kB/s)
Extracting templates from packages: 100%
Preconfiguring packages ...
Selecting previously unselected package pigz.
(Reading database ... 106500 files and directories currently installed.)
Preparing to unpack .../00-pigz_2.4-1_amd64.deb ...
Unpacking pigz (2.4-1) ...
Selecting previously unselected package bridge-utils.
Preparing to unpack .../01-bridge-utils_1.5-15ubuntu1_amd64.deb ...
Unpacking bridge-utils (1.5-15ubuntu1) ...
Selecting previously unselected package cgroupfs-mount.
Preparing to unpack .../02-cgroupfs-mount_1.4_all.deb ...
Unpacking cgroupfs-mount (1.4) ...
Selecting previously unselected package runc.
Preparing to unpack .../03-runc_1.0.0~rc10-0ubuntu1~18.04.2_amd64.deb ...
Unpacking runc (1.0.0~rc10-0ubuntu1~18.04.2) ...
Selecting previously unselected package containerd.
Preparing to unpack .../04-containerd_1.3.3-0ubuntu1~18.04.2_amd64.deb ...
Unpacking containerd (1.3.3-0ubuntu1~18.04.2) ...
Selecting previously unselected package python-backports.ssl-match-hostname.
Preparing to unpack .../05-python-backports.ssl-match-hostname_3.5.0.1-1_all.deb                                     ...
Unpacking python-backports.ssl-match-hostname (3.5.0.1-1) ...
Selecting previously unselected package python-pkg-resources.
Preparing to unpack .../06-python-pkg-resources_39.0.1-2_all.deb ...
Unpacking python-pkg-resources (39.0.1-2) ...
Selecting previously unselected package python-cached-property.
Preparing to unpack .../07-python-cached-property_1.3.1-1_all.deb ...
Unpacking python-cached-property (1.3.1-1) ...
Selecting previously unselected package python-six.
Preparing to unpack .../08-python-six_1.11.0-2_all.deb ...
Unpacking python-six (1.11.0-2) ...
Selecting previously unselected package libsecret-common.
Preparing to unpack .../09-libsecret-common_0.18.6-1_all.deb ...
Unpacking libsecret-common (0.18.6-1) ...
Selecting previously unselected package libsecret-1-0:amd64.
Preparing to unpack .../10-libsecret-1-0_0.18.6-1_amd64.deb ...
Unpacking libsecret-1-0:amd64 (0.18.6-1) ...
Selecting previously unselected package golang-docker-credential-helpers.
Preparing to unpack .../11-golang-docker-credential-helpers_0.5.0-2_amd64.deb ..                                    .
Unpacking golang-docker-credential-helpers (0.5.0-2) ...
Selecting previously unselected package python-dockerpycreds.
Preparing to unpack .../12-python-dockerpycreds_0.2.1-1_all.deb ...
Unpacking python-dockerpycreds (0.2.1-1) ...
Selecting previously unselected package python-certifi.
Preparing to unpack .../13-python-certifi_2018.1.18-2_all.deb ...
Unpacking python-certifi (2018.1.18-2) ...
Selecting previously unselected package python-chardet.
Preparing to unpack .../14-python-chardet_3.0.4-1_all.deb ...
Unpacking python-chardet (3.0.4-1) ...
Selecting previously unselected package python-idna.
Preparing to unpack .../15-python-idna_2.6-1_all.deb ...
Unpacking python-idna (2.6-1) ...
Selecting previously unselected package python-urllib3.
Preparing to unpack .../16-python-urllib3_1.22-1ubuntu0.18.04.1_all.deb ...
Unpacking python-urllib3 (1.22-1ubuntu0.18.04.1) ...
Selecting previously unselected package python-requests.
Preparing to unpack .../17-python-requests_2.18.4-2ubuntu0.1_all.deb ...
Unpacking python-requests (2.18.4-2ubuntu0.1) ...
Selecting previously unselected package python-websocket.
Preparing to unpack .../18-python-websocket_0.44.0-0ubuntu2_all.deb ...
Unpacking python-websocket (0.44.0-0ubuntu2) ...
Selecting previously unselected package python-ipaddress.
Preparing to unpack .../19-python-ipaddress_1.0.17-1_all.deb ...
Unpacking python-ipaddress (1.0.17-1) ...
Selecting previously unselected package python-docker.
Preparing to unpack .../20-python-docker_2.5.1-1_all.deb ...
Unpacking python-docker (2.5.1-1) ...
Selecting previously unselected package python-dockerpty.
Preparing to unpack .../21-python-dockerpty_0.4.1-1_all.deb ...
Unpacking python-dockerpty (0.4.1-1) ...
Selecting previously unselected package python-docopt.
Preparing to unpack .../22-python-docopt_0.6.2-1build1_all.deb ...
Unpacking python-docopt (0.6.2-1build1) ...
Selecting previously unselected package python-enum34.
Preparing to unpack .../23-python-enum34_1.1.6-2_all.deb ...
Unpacking python-enum34 (1.1.6-2) ...
Selecting previously unselected package python-functools32.
Preparing to unpack .../24-python-functools32_3.2.3.2-3_all.deb ...
Unpacking python-functools32 (3.2.3.2-3) ...
Selecting previously unselected package python-funcsigs.
Preparing to unpack .../25-python-funcsigs_1.0.2-4_all.deb ...
Unpacking python-funcsigs (1.0.2-4) ...
Selecting previously unselected package python-pbr.
Preparing to unpack .../26-python-pbr_3.1.1-3ubuntu3_all.deb ...
Unpacking python-pbr (3.1.1-3ubuntu3) ...
Selecting previously unselected package python-mock.
Preparing to unpack .../27-python-mock_2.0.0-3_all.deb ...
Unpacking python-mock (2.0.0-3) ...
Selecting previously unselected package python-jsonschema.
Preparing to unpack .../28-python-jsonschema_2.6.0-2_all.deb ...
Unpacking python-jsonschema (2.6.0-2) ...
Selecting previously unselected package python-texttable.
Preparing to unpack .../29-python-texttable_0.9.1-1_all.deb ...
Unpacking python-texttable (0.9.1-1) ...
Selecting previously unselected package python-yaml.
Preparing to unpack .../30-python-yaml_3.12-1build2_amd64.deb ...
Unpacking python-yaml (3.12-1build2) ...
Selecting previously unselected package docker-compose.
Preparing to unpack .../31-docker-compose_1.17.1-2_all.deb ...
Unpacking docker-compose (1.17.1-2) ...
Selecting previously unselected package docker.io.
Preparing to unpack .../32-docker.io_19.03.6-0ubuntu1~18.04.1_amd64.deb ...
Unpacking docker.io (19.03.6-0ubuntu1~18.04.1) ...
Selecting previously unselected package python-asn1crypto.
Preparing to unpack .../33-python-asn1crypto_0.24.0-1_all.deb ...
Unpacking python-asn1crypto (0.24.0-1) ...
Selecting previously unselected package python-cffi-backend.
Preparing to unpack .../34-python-cffi-backend_1.11.5-1_amd64.deb ...
Unpacking python-cffi-backend (1.11.5-1) ...
Selecting previously unselected package python-cryptography.
Preparing to unpack .../35-python-cryptography_2.1.4-1ubuntu1.3_amd64.deb ...
Unpacking python-cryptography (2.1.4-1ubuntu1.3) ...
Selecting previously unselected package python-openssl.
Preparing to unpack .../36-python-openssl_17.5.0-1ubuntu1_all.deb ...
Unpacking python-openssl (17.5.0-1ubuntu1) ...
Selecting previously unselected package ubuntu-fan.
Preparing to unpack .../37-ubuntu-fan_0.12.10_all.deb ...
Unpacking ubuntu-fan (0.12.10) ...
Setting up python-idna (2.6-1) ...
Setting up python-texttable (0.9.1-1) ...
Setting up libsecret-common (0.18.6-1) ...
Setting up python-functools32 (3.2.3.2-3) ...
Setting up python-yaml (3.12-1build2) ...
Setting up python-asn1crypto (0.24.0-1) ...
Setting up runc (1.0.0~rc10-0ubuntu1~18.04.2) ...
Setting up python-certifi (2018.1.18-2) ...
Setting up cgroupfs-mount (1.4) ...
Setting up python-pkg-resources (39.0.1-2) ...
Setting up containerd (1.3.3-0ubuntu1~18.04.2) ...
Created symlink /etc/systemd/system/multi-user.target.wants/containerd.service →                                     /lib/systemd/system/containerd.service.
Setting up python-backports.ssl-match-hostname (3.5.0.1-1) ...
Setting up bridge-utils (1.5-15ubuntu1) ...
Setting up python-cffi-backend (1.11.5-1) ...
Setting up python-six (1.11.0-2) ...
Setting up python-dockerpty (0.4.1-1) ...
Setting up ubuntu-fan (0.12.10) ...
Created symlink /etc/systemd/system/multi-user.target.wants/ubuntu-fan.service →                                     /lib/systemd/system/ubuntu-fan.service.
Setting up python-pbr (3.1.1-3ubuntu3) ...
update-alternatives: using /usr/bin/python2-pbr to provide /usr/bin/pbr (pbr) in                                     auto mode
Setting up python-enum34 (1.1.6-2) ...
Setting up python-funcsigs (1.0.2-4) ...
Setting up python-docopt (0.6.2-1build1) ...
Setting up python-ipaddress (1.0.17-1) ...
Setting up libsecret-1-0:amd64 (0.18.6-1) ...
Setting up pigz (2.4-1) ...
Setting up python-cached-property (1.3.1-1) ...
Setting up python-urllib3 (1.22-1ubuntu0.18.04.1) ...
Setting up python-chardet (3.0.4-1) ...
Setting up docker.io (19.03.6-0ubuntu1~18.04.1) ...
Adding group `docker' (GID 116) ...
Done.
Created symlink /etc/systemd/system/sockets.target.wants/docker.socket → /lib/sy                                    stemd/system/docker.socket.
docker.service is a disabled or a static unit, not starting it.
Setting up python-mock (2.0.0-3) ...
Setting up python-websocket (0.44.0-0ubuntu2) ...
update-alternatives: using /usr/bin/python2-wsdump to provide /usr/bin/wsdump (w                                    sdump) in auto mode
Setting up golang-docker-credential-helpers (0.5.0-2) ...
Setting up python-cryptography (2.1.4-1ubuntu1.3) ...
Setting up python-requests (2.18.4-2ubuntu0.1) ...
Setting up python-jsonschema (2.6.0-2) ...
update-alternatives: using /usr/bin/python2-jsonschema to provide /usr/bin/jsons                                    chema (jsonschema) in auto mode
Setting up python-dockerpycreds (0.2.1-1) ...
Setting up python-openssl (17.5.0-1ubuntu1) ...
Setting up python-docker (2.5.1-1) ...
Setting up docker-compose (1.17.1-2) ...
Processing triggers for systemd (237-3ubuntu10.39) ...
Processing triggers for man-db (2.8.3-2ubuntu0.1) ...
Processing triggers for ureadahead (0.100.0-21) ...
Processing triggers for libc-bin (2.27-3ubuntu1) ...
```

### Checking docker installation

```text
> sudo docker --version
Docker version 19.03.6, build 369ce74a3c

> sudo docker images
REPOSITORY          TAG                 IMAGE ID            CREATED             SIZE

> sudo docker ps
CONTAINER ID        IMAGE               COMMAND             CREATED             STATUS              PORTS               NAMES

> sudo docker-compose version
docker-compose version 1.17.1, build unknown
docker-py version: 2.5.1
CPython version: 2.7.17
OpenSSL version: OpenSSL 1.1.1  11 Sep 2018
```

