---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: fysio.care
  spf: true
hosts:
- cert_expires: Jan 26 21:12:44 2027 GMT
  host: fysio.care
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Fysio Care Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fysio Care, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Fysio Care
provider_slug: fysio-care
slug: fysio-care-domain-security
source_filename: fysio-care-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fysio.care\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 26 21:12:44 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: fysio.care\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/fysio-care/security/fysio-care-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Health
- Digital Health
- Sweden
- Booking
- Physiotherapy
---
