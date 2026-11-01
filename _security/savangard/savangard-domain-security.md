---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: savangard.com
  spf: true
hosts:
- cert_expires: May  4 00:00:00 2027 GMT
  host: savangard.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Savangard Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for IT system integration, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: IT system integration
provider_slug: savangard
slug: savangard-domain-security
source_filename: savangard-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: savangard.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: May  4 00:00:00 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: savangard.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/savangard/security/savangard-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- IT
- Integration
- Consulting
- OpenBanking
- DigitalTransformation
---
