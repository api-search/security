---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: meetleo.com
  spf: true
hosts:
- cert_expires: Sep  3 14:40:37 2026 GMT
  host: www.meetleo.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Leo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LeO, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: LeO
provider_slug: leo
slug: leo-domain-security
source_filename: leo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.meetleo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 14:40:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: meetleo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/leo/refs/heads/main/security/leo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Insurance
- Commercial Insurance
- Property and Casualty
- Employee Benefits
- Insurtech
- Artificial Intelligence
- Sales
- Lead Generation
- Prospecting
---
