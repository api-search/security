---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: nuevometodo.com
  spf: true
hosts:
- cert_expires: Nov  5 23:59:59 2026 GMT
  host: nuevometodo.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nuevo M Todo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nuevo Método, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Nuevo Método
provider_slug: nuevo-m-todo
slug: nuevo-m-todo-domain-security
source_filename: nuevo-m-todo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nuevometodo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  5 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: nuevometodo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nuevo-m-todo/refs/heads/main/security/nuevo-m-todo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Digital Health
- Corporate Wellness
- Employee Benefits
- Mental Health
- Telemedicine
- Insurance
- Latin America
---
