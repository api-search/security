---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: brontir.com
  spf: false
hosts:
- cert_expires: Dec 26 11:21:05 2026 GMT
  host: brontir.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Brontir Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BRONTIR, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: BRONTIR
provider_slug: brontir-com
slug: brontir-com-domain-security
source_filename: brontir-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: brontir.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 11:21:05 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: brontir.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/brontir-com/security/brontir-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Data Integration
- Web Research
- Public Data
- Software-as-a-Service
---
