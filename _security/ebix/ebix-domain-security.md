---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ebix.com
  spf: true
hosts:
- cert_expires: Nov 25 23:59:59 2026 GMT
  host: www.ebix.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Ebix Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ebix, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Ebix
provider_slug: ebix
slug: ebix-domain-security
source_filename: ebix-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ebix.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 25 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ebix.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ebix/refs/heads/main/security/ebix-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Insurance
- United States
- Property and Casualty
- Life Insurance
- Health Insurance
- Employee Benefits
- Agency Management
- Policy Administration
- Claims
- ACORD
- Insurtech
- Market Infrastructure
---
