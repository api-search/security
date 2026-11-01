---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: jenny.mortgage
  spf: true
hosts:
- cert_expires: Jan  4 00:03:47 2027 GMT
  host: jenny.mortgage
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Jenny Mortgage Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mortgage Tools by Jenny, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Mortgage Tools by Jenny
provider_slug: jenny-mortgage
slug: jenny-mortgage-domain-security
source_filename: jenny-mortgage-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: jenny.mortgage\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 00:03:47 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: jenny.mortgage\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/jenny-mortgage/security/jenny-mortgage-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Mortgage
- Calculator
- AI
- Canada
---
