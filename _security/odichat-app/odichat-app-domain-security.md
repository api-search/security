---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: odichat.app
  spf: true
hosts:
- cert_expires: Jan 10 05:16:30 2027 GMT
  host: odichat.app
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Odichat Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Odichat, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Odichat
provider_slug: odichat-app
slug: odichat-app-domain-security
source_filename: odichat-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: odichat.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 05:16:30 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: odichat.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/odichat-app/security/odichat-app-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Messaging
- CRM
- WhatsApp
- Business
- Artificial Intelligence
---
