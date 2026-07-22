---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ejen2u.com
  spf: true
hosts:
- cert_expires: Oct 13 05:11:11 2026 GMT
  host: ejen2u.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ejen2U Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ejen2u, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Ejen2u
provider_slug: ejen2u
slug: ejen2u-domain-security
source_filename: ejen2u-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ejen2u.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 05:11:11 2026 GMT\n  hsts: false\ndomains:\n- domain: ejen2u.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ejen2u/refs/heads/main/security/ejen2u-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Reseller Management
- Agent Management
- E-Commerce
- SaaS
- Fintech
- Logistics
- MSME
- Malaysia
---
