---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: rentspree.com
  spf: true
hosts:
- cert_expires: Oct  4 12:30:04 2026 GMT
  host: www.rentspree.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rentspree Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RentSpree, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: RentSpree
provider_slug: rentspree
slug: rentspree-domain-security
source_filename: rentspree-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.rentspree.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 12:30:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: rentspree.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rentspree/refs/heads/main/security/rentspree-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Real Estate
- Rentals
- Rental Applications
- Tenant Screening
- Credit Check
- Background Check
- Eviction History
- Income Verification
- Renters Insurance
- Rent Payments
- E-Sign
- Leasing
- Listings
- MLS
- PropTech
- Brokerage
- REALTOR Association
---
