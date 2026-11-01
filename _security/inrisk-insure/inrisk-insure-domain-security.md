---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: inrisk.insure
  spf: true
hosts:
- cert_expires: Dec 26 19:22:05 2026 GMT
  host: inrisk.insure
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Inrisk Insure Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for InRisk, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: InRisk
provider_slug: inrisk-insure
slug: inrisk-insure-domain-security
source_filename: inrisk-insure-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: inrisk.insure\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 19:22:05 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\ndomains:\n- domain: inrisk.insure\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/inrisk-insure/security/inrisk-insure-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Company
- Insurance
- ClimateTech
- Parametric
- FinTech
---
