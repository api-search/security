---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: dealmaker.tech
  spf: true
hosts:
- cert_expires: Jan  8 14:21:52 2027 GMT
  host: www.dealmaker.tech
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Dealmaker Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DealMaker, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: DealMaker
provider_slug: dealmaker
slug: dealmaker-domain-security
source_filename: dealmaker-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dealmaker.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 14:21:52 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: dealmaker.tech\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/dealmaker/security/dealmaker-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Fintech
- Capital Raising
- Investment Platform
- Software-as-a-Service
---
