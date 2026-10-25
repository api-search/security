---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: nib.com.au
  spf: true
hosts:
- cert_expires: Dec  4 21:47:18 2026 GMT
  host: www.nib.com.au
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  4 21:47:18 2026 GMT
  host: my.nib.com.au
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  4 21:47:18 2026 GMT
  host: id.nib.com.au
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Nib Health Funds Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for nib, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: nib
provider_slug: nib-health-funds
slug: nib-health-funds-domain-security
source_filename: nib-health-funds-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nib.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  4 21:47:18 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\n- host: my.nib.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  4 21:47:18 2026 GMT\n  hsts: null\n- host: id.nib.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  4 21:47:18 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\ndomains:\n- domain: nib.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nib-health-funds/refs/heads/main/security/nib-health-funds-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Insurance
- Australia
- Health Insurance
- Carrier
- Claims
- Private Health Insurance
- Travel Insurance
- New Zealand
- NDIS
---
