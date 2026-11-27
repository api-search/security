---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: itcons.app
  spf: true
hosts:
- cert_expires: Jan  8 22:28:09 2027 GMT
  host: itcons.app
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Itcons.app Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Itcons.app, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Itcons.app
provider_slug: itcons-app
slug: itcons-app-domain-security
source_filename: itcons-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: itcons.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 22:28:09 2027 GMT\n  hsts: false\ndomains:\n- domain: itcons.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/itcons-app/security/itcons-app-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- FieldWork
- Digital Platform
- Construction
- MunicipalServices
- Logistics
- Gardening
---
