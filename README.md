# passhport-client
OpenBSD's SSH client compatible with PaSSHport tunneling

## Setup and build
```
apk add alpine-sdk
abuild checksum
abuild -r
```

## Install
```
apk add --allow-untrusted passhport-client-1.X-rX.apk
```

## Usage
```
passhport-client -l target [-p port] host [command]
```

## With lftp
```
set sftp:connect-program /usr/bin/passhport-client
```
