---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: zincwork.com
  spf: true
hosts:
- cert_expires: Oct  2 18:44:07 2026 GMT
  host: zincwork.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zinc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zinc, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Zinc
provider_slug: zinc
slug: zinc-domain-security
source_filename: zinc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: zincwork.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 18:44:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: zincwork.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zinc/refs/heads/main/security/zinc-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Background Checks
- Employment Screening
- Identity Verification
- Human Resources
- Recruiting
- Compliance
- HR Tech
---
