# ansible-rpm

## Examples of use

```
    - role: rpm/pubkey
      dest: /etc/pki/rpm-gpg/RPM-GPG-KEY-EPEL
      fingerprint: 1EEF B876 7D49 24B8 6EAD  08A4 59D7 00E4 D37F 5F19
```

```
    - role: rpm/pubkey
      key_src: neotechnology.gpg.key-1
      dest: /etc/pki/rpm-gpg/RPM-GPG-KEY-NEOTECHNOLOGY-1
      fingerprint: 1EEF B876 7D49 24B8 6EAD  08A4 59D7 00E4 D37F 5F19
```

```
    - role: rpm
      rpm_name: jre1.8
      rpm_src: files/jre-8u181-linux-x64.rpm
      rpm_dest: /tmp/jre-8u181-linux-x64.rpm
```
