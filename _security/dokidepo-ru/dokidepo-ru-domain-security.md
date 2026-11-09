---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: dokidepo.ru
  spf: true
hosts:
- cert_expires: Jan  4 17:34:31 2027 GMT
  host: dokidepo.ru
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Dokidepo Ru Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ДокиДепо, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: ДокиДепо
provider_slug: dokidepo-ru
slug: dokidepo-ru-domain-security
source_filename: dokidepo-ru-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dokidepo.ru\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 17:34:31 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: dokidepo.ru\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/dokidepo-ru/security/dokidepo-ru-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Warehouse
- BusinessTools
- Free
---
