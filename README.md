# passhport-client
OpenBSD's SSH client compatible with PaSSHport tunneling

## Setup, build and install
```
apk add alpine-sdk
abuild checksum
abuild -r
apk add passhport-client-1.0-r0.apk
```

## Usage
```
passhport-client -l target [-p port] host [command]
```

## With lftp
```
set sftp:connect-program /usr/bin/passhport-client
```
