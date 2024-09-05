# OS dependencies

## Ubuntu / Debian
```
sudo apt-get install curl exiftool libcurl4-openssl-dev jq libssl-dev sshpass libsqlite3-dev sqlite3 libpq-dev libxml2-utils ncftp p7zip-full
```

## Red Hat / CentOS
```
sudo dnf groupinstall "Development Tools"
sudo dnf install sqlite
yum install perl-IPC-Cmd curl curl-devel sqlite-devel libxml2 openssl-devel
```

# minARC

## Build

```
rake -f build_minarc.rake minarc:build
```


## Install

```
build_minarc.rake minarc:install[borja,localhost,s2_test_pg]
```

## Unit tests

```
export MINARC_PLUGIN=S2PDGS
minArcUnitTests
```






