
## Example Usage

```
- hosts: localhost

  roles:

    - role: mafalb.chrony/absent

    - role: mafalb.ntp
      ntp_servers:
        - hostname: ntp.example.com
```

```
- hosts: localhost
  roles:
    - role: mafalb.ntp/disabled
```

```
- hosts: localhost
  roles:
    - role: mafalb.ntp/absent
```

## Variables

```
ntp_servers:
  - hostname: bla.example.com
    iburst: true		# default false
```

```ntp_status: absent``` # [enabled|disabled|absent]
