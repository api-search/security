---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: equator-principles.com
  spf: true
hosts:
- cert_expires: Sep 15 16:22:29 2026 GMT
  host: equator-principles.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Equator Principles Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Equator Principles, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Equator Principles
provider_slug: equator-principles
slug: equator-principles-domain-security
source_filename: equator-principles-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: equator-principles.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 16:22:29 2026 GMT\n  hsts: true\n  hsts_max_age: 300\ndomains:\n- domain: equator-principles.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/equator-principles/refs/heads/main/security/equator-principles-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Environmental Social Governance
- Financial Services
- Risk Management
- Sustainability
---
