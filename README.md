# GNU/Linux

Поменять etc/openvpn/login.conf и запустить сервис OpenVPN:
```shell
systemctl enable openvpn@majordomo.service
systemctl start openvpn@majordomo.service
```

# Windows

```
dev tap
auth-nocache

<connection>
remote 81.95.28.29 1194 udp
mssfix 0
float
</connection>

<connection>
remote 78.108.80.230 1194 udp
mssfix 0
float
</connection>

<connection>
remote 78.108.91.250 1194 udp
mssfix 0
float
</connection>

inactive 3600
ping 5
ping-restart 10
remote-random
reneg-sec 36000
server-poll-timeout 10
comp-lzo
verb 2
auth SHA1
auth-user-pass
auth-retry nointeract
client
float
script-security 3
#reneg-ser 36000
<ca>
-----BEGIN CERTIFICATE-----
MIIDyzCCAzSgAwIBAgIJANowWXITcAdHMA0GCSqGSIb3DQEBBQUAMIGgMQswCQYD
VQQGEwJSVTELMAkGA1UECBMCUlUxGTAXBgNVBAcTEFNhaW50LVBldGVyc2J1cmcx
FzAVBgNVBAoTDk1ham9yZG9tbyBMdGQuMQ8wDQYDVQQLEwZvZmZpY2UxGjAYBgNV
BAMTEU1ham9yZG9tbyBMdGQuIENBMSMwIQYJKoZIhvcNAQkBFhRzdXBwb3J0QG1h
am9yZG9tby5ydTAeFw0xMjA3MjUxMjA5MjhaFw0yMjA3MjMxMjA5MjhaMIGgMQsw
CQYDVQQGEwJSVTELMAkGA1UECBMCUlUxGTAXBgNVBAcTEFNhaW50LVBldGVyc2J1
cmcxFzAVBgNVBAoTDk1ham9yZG9tbyBMdGQuMQ8wDQYDVQQLEwZvZmZpY2UxGjAY
BgNVBAMTEU1ham9yZG9tbyBMdGQuIENBMSMwIQYJKoZIhvcNAQkBFhRzdXBwb3J0
QG1ham9yZG9tby5ydTCBnzANBgkqhkiG9w0BAQEFAAOBjQAwgYkCgYEA28CpvcRH
Lav/CTRf88nf1uNWtB/3y4BWhZOpdP+xHqoYfLoMXKOa4f9itjmqpgOwNZB7u3AU
P5uJrU9If8eMy6Uc9AmxM8alv7DL96PkIxbw3MTxC4HqDc7E1GJ5N9pkGO/ZFxHn
vhHuiGR5G5yTZh+lrufhSGjWL2Dr6JX4e2cCAwEAAaOCAQkwggEFMB0GA1UdDgQW
BBSp87/cgdG8+VS72/jdyTxLgq6DtDCB1QYDVR0jBIHNMIHKgBSp87/cgdG8+VS7
2/jdyTxLgq6DtKGBpqSBozCBoDELMAkGA1UEBhMCUlUxCzAJBgNVBAgTAlJVMRkw
FwYDVQQHExBTYWludC1QZXRlcnNidXJnMRcwFQYDVQQKEw5NYWpvcmRvbW8gTHRk
LjEPMA0GA1UECxMGb2ZmaWNlMRowGAYDVQQDExFNYWpvcmRvbW8gTHRkLiBDQTEj
MCEGCSqGSIb3DQEJARYUc3VwcG9ydEBtYWpvcmRvbW8ucnWCCQDaMFlyE3AHRzAM
BgNVHRMEBTADAQH/MA0GCSqGSIb3DQEBBQUAA4GBAIqO8PN8arVYHPs0sBFPeaI5
mdb4zmFGBGENPE4QgnTK9tDfG8s8cLJbsqrLJSXCTOehUV6KqKPOAnBmZCu+lJs6
+VSpnm3ANacWZFKXejr3R92D4SAoEHCWCMUAkZh3MD+qoDR1E3PROfYdKcRf1+eR
zlLP9L/g/sFh438M1RVq
-----END CERTIFICATE-----
</ca>
```
