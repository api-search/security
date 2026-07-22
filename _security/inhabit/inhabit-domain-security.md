---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: inhabitiq.com
  spf: true
hosts:
- cert_expires: Oct  3 15:28:41 2026 GMT
  host: inhabitiq.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Inhabit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Inhabit, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Inhabit
provider_slug: inhabit
slug: inhabit-domain-security
source_filename: inhabit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: inhabitiq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 15:28:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: inhabitiq.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/inhabit/refs/heads/main/security/inhabit-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- PropTech
- Property Management
- Vacation Rentals
- Real Estate
- Multifamily
- Insurance
- Payments
- Tenant Screening
- Software
---
