---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: pscinsurance.com.au
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: pscbroking.co.nz
  spf: true
hosts:
- cert_expires: Sep 20 23:52:34 2026 GMT
  host: www.pscinsurance.com.au
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 12 08:01:48 2026 GMT
  host: www.pscbroking.co.nz
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Psc Insurance Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PSC Insurance, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: PSC Insurance
provider_slug: psc-insurance
slug: psc-insurance-domain-security
source_filename: psc-insurance-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.pscinsurance.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 23:52:34 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.pscbroking.co.nz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 08:01:48 2026 GMT\n  hsts: false\ndomains:\n- domain: pscinsurance.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: pscbroking.co.nz\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/psc-insurance/refs/heads/main/security/psc-insurance-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Insurance
- Australia
- Brokers
- Insurance Brokerage
- Property and Casualty
- Commercial Insurance
- Cyber Insurance
- Intermediary
- Partner Gated
- No Public API
---
