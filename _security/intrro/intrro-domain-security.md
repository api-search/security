---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: intrro.com
  spf: true
hosts:
- cert_expires: Nov 30 00:57:19 2026 GMT
  host: intrro.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Intrro Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Intrro, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Intrro
provider_slug: intrro
slug: intrro-domain-security
source_filename: intrro-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: intrro.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 30 00:57:19 2026 GMT\n  hsts: false\ndomains:\n- domain: intrro.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/intrro/refs/heads/main/security/intrro-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Recruiting
- HR Tech
- Employee Referrals
- Talent Acquisition
- Hiring
- ATS Integration
- SaaS
---
