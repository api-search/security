---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: vc.systems
  spf: true
hosts:
- cert_expires: Feb  5 23:59:59 2027 GMT
  host: vc.systems
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Virtualcitysystems Gmbh Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for virtualcitySYSTEMS GmbH, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: virtualcitySYSTEMS GmbH
provider_slug: virtualcitysystems-gmbh
slug: virtualcitysystems-gmbh-domain-security
source_filename: virtualcitysystems-gmbh-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: vc.systems\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb  5 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: vc.systems\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/virtualcitysystems-gmbh/security/virtualcitysystems-gmbh-domain-security.yml
summary_line: TLSv1.2 · HSTS
tags:
- Company
- DigitalTwin
- UrbanPlanning
- 3DModels
- Simulation
---
