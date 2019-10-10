
## Example Usage

```
- hosts: localhost

  roles:

    - role: mafalb.chrony
      chrony_state: absent

    - role: mafalb.ntp
      ntp_servers:
        - hostname: ntp.example.com
```

```
- hosts: localhost
  roles:
    - role: mafalb.ntp
      ntp_status: absent
```

## Variables

```
ntp_servers:
  - hostname: bla.example.com
    iburst: true		# default false
```

```ntp_status: absent``` # [enabled|disabled|absent]
