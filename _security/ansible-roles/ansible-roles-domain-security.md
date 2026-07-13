---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: ansible.com
  spf: true
- caa:
  - 0 iodef "mailto:it-cert-admin@redhat.com"
  - 0 issue "amazontrust.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: redhat.com
  spf: true
hosts:
- cert_expires: Sep 17 12:14:32 2026 GMT
  host: galaxy.ansible.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 13 23:59:59 2027 GMT
  host: console.redhat.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ansible Roles Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ansible Roles, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Ansible Roles
provider_slug: ansible-roles
slug: ansible-roles-domain-security
source_filename: ansible-roles-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: galaxy.ansible.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 12:14:32 2026 GMT\n  hsts: false\n- host: console.redhat.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 13 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ansible.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: redhat.com\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:it-cert-admin@redhat.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ansible-roles/refs/heads/main/security/ansible-roles-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Ansible
- Automation
- Collections
- Configuration Management
- DevOps
- Infrastructure As Code
- Roles
---
