---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: exactmods.com
  spf: true
hosts:
- cert_expires: Dec 27 07:32:02 2026 GMT
  host: exactmods.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: ExactMods Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ExactMods, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: ExactMods
provider_slug: exactmods-com
slug: exactmods-com-domain-security
source_filename: exactmods-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: exactmods.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 07:32:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: exactmods.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/exactmods-com/security/exactmods-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- rc
- Marketplace
- Parts
- Upgrades
---
