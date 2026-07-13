---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: todogroup.org
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: linuxfoundation.org
  spf: true
hosts:
- cert_expires: Aug 14 02:49:37 2026 GMT
  host: todogroup.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 14 02:49:37 2026 GMT
  host: landscape.todogroup.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 18:30:18 2026 GMT
  host: community.linuxfoundation.org
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Todo Group Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TODO Group, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: TODO Group
provider_slug: todo-group
slug: todo-group-domain-security
source_filename: todo-group-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: todogroup.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 02:49:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: landscape.todogroup.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 02:49:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: community.linuxfoundation.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 18:30:18 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: todogroup.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: linuxfoundation.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/todo-group/refs/heads/main/security/todo-group-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Community
- Linux Foundation
- Open Source
- OSPO
---
