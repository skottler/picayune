Picayune
========

A small set of Ansible playbooks and roles targetted toward CentOS 7.

### User management

This project supports managing users via the top-level `users` key, defined as
the following in `vars/user.yml`:

```yml
---
users:
  - username: samkottler
    name: Sam Kottler
    groups: ["wheel", "systemd-journal"]
    uid: 101
    ssh_key:
      - "ssh-rsa
        AAAAB3NzaC1yc2EAAAABIwAAAQEAuZUm6qBJDRKWzrZGx3hiWlVUtmyWvlQGbmI/GyMGqTzzABIb3n8RjpCEBwiBu01wu6ECfyPJ2qGW87G+DVpb1Z5orxQWRPruEg3aw5lXxiHA6dAmd6qWVZKBbQYhXheeepD7QrNwWc/MpVzjqeNitLD0TEI56AJTjL5dIFZHYh5ZHYPYoSVIvH53aub3+vGbzaD/eQamYxuBvecb5A2uHwld//KVA77mKFK68gX92ESd77fpcjwY6cEKQpoobBD4mHpXYfxn8+1OoOkuNo0awkhec9hXQJHRpcIHko+BOGac0d1ZECZIPhAwu7U9KpOCutmJ+YhY1He+++OMXydjxQ==
sam.kottler@mbp"
```
