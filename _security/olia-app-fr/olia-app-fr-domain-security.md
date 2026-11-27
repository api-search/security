---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: olia-app.fr
  spf: true
hosts:
- cert_expires: Jan 24 22:19:05 2027 GMT
  host: olia-app.fr
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Olia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Olia, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Olia
provider_slug: olia-app-fr
slug: olia-app-fr-domain-security
source_filename: olia-app-fr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: olia-app.fr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 24 22:19:05 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: olia-app.fr\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/olia-app-fr/security/olia-app-fr-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Legal Tech
- Software-as-a-Service
- Artificial Intelligence
- Practice Management
- France
---
