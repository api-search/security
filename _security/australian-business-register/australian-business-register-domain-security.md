---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: abr.gov.au
  spf: true
hosts:
- cert_expires: Feb 16 23:59:59 2027 GMT
  host: abr.gov.au
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Australian Business Register Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Australian Business Register, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Australian Business Register
provider_slug: australian-business-register
slug: australian-business-register-domain-security
source_filename: australian-business-register-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: abr.gov.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 16 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: abr.gov.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/australian-business-register/refs/heads/main/security/australian-business-register-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Government
- Australia
- Business Registry
- ABN
- Tax
- Public Sector
- Open Data
---
