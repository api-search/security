---
api_specs:
- filename: ssh-key-management-openapi.yml
  format: yaml
  label: OpenSSH Key Management API
  slug: openssh-management
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ssh/refs/heads/main/openapi/ssh-key-management-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: openssh.com
  spf: false
- caa:
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:caa-reports@goteleport.com"
  - 0 issue "amazonaws.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: goteleport.com
  spf: true
hosts:
- cert_expires: Sep 24 15:55:53 2026 GMT
  host: www.openssh.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 10 06:20:38 2026 GMT
  host: goteleport.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ssh Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SSH, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: SSH
provider_slug: ssh
slug: ssh-domain-security
source_filename: ssh-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.openssh.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 15:55:53 2026 GMT\n  hsts: false\n- host: goteleport.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 06:20:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: openssh.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: goteleport.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:caa-reports@goteleport.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ssh/refs/heads/main/security/ssh-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- SSH
- Secure Shell
- Remote Access
- Cryptography
- Network Security
- System Administration
---
