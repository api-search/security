---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: lockton.com
  spf: true
hosts:
- cert_expires: Sep 19 22:23:56 2026 GMT
  host: global.lockton.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lockton Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lockton, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Lockton
provider_slug: lockton
slug: lockton-domain-security
source_filename: lockton-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: global.lockton.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 22:23:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: lockton.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lockton/refs/heads/main/security/lockton-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Insurance
- United States
- Broker
- Insurance Brokerage
- Property and Casualty
- Employee Benefits
- Reinsurance
- Specialty Insurance
- Risk Management
- ACORD
- Partner Gated
- No Public API
---
