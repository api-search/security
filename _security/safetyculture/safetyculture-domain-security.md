---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: safetyculture.com
  spf: true
hosts:
- cert_expires: Oct 13 16:05:15 2026 GMT
  host: safetyculture.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Safetyculture Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SafetyCulture, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: SafetyCulture
provider_slug: safetyculture
slug: safetyculture-domain-security
source_filename: safetyculture-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: safetyculture.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 16:05:15 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: safetyculture.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/safetyculture/refs/heads/main/security/safetyculture-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Business Applications
- Safety
- Inspections
- Workplace Operations
- EHS
- Compliance
- Training
- Field Service
- Webhooks
---
