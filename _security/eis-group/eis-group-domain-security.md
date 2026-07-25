---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: eisgroup.com
  spf: true
hosts:
- cert_expires: Aug 21 18:27:40 2026 GMT
  host: www.eisgroup.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Eis Group Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EIS Group, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: EIS Group
provider_slug: eis-group
slug: eis-group-domain-security
source_filename: eis-group-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.eisgroup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 18:27:40 2026 GMT\n  hsts: false\ndomains:\n- domain: eisgroup.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eis-group/refs/heads/main/security/eis-group-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Insurance
- United States
- Core Systems
- Policy Administration
- Claims
- Billing
- Underwriting
- Property and Casualty
- Life Insurance
- Employee Benefits
- Insurtech
- ACORD
---
