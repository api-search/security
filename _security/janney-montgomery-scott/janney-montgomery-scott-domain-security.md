---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: janney.com
  spf: true
hosts:
- cert_expires: Sep 14 20:22:14 2026 GMT
  host: www.janney.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Janney Montgomery Scott Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Janney Montgomery Scott, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Janney Montgomery Scott
provider_slug: janney-montgomery-scott
slug: janney-montgomery-scott-domain-security
source_filename: janney-montgomery-scott-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.janney.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 20:22:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: janney.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/janney-montgomery-scott/refs/heads/main/security/janney-montgomery-scott-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Asset Management
- Brokerage
- Capital Markets
- Financial Planning
- Financial Services
- Investment Banking
- Investment Management
- Private Company
- Wealth Management
---
