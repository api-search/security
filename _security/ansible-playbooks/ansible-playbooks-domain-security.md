---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: ansible.com
  spf: true
- caa:
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue " amazontrust.com"
  dmarc: false
  dnssec: false
  domain: readthedocs.io
  spf: false
hosts:
- cert_expires: Oct  2 12:36:59 2026 GMT
  host: docs.ansible.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 27 13:13:23 2026 GMT
  host: ansible-runner.readthedocs.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 29 04:33:07 2027 GMT
  host: pypi.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ansible Playbooks Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ansible Playbooks, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Ansible Playbooks
provider_slug: ansible-playbooks
slug: ansible-playbooks-domain-security
source_filename: ansible-playbooks-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.ansible.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 12:36:59 2026 GMT\n  hsts: false\n- host: ansible-runner.readthedocs.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 13:13:23 2026 GMT\n  hsts: false\n- host: pypi.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 29 04:33:07 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ansible.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: readthedocs.io\n  dnssec: false\n  caa:\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \" amazontrust.com\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ansible-playbooks/refs/heads/main/security/ansible-playbooks-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Ansible
- Automation
- Configuration Management
- DevOps
- Infrastructure As Code
- Orchestration
- Playbooks
---
