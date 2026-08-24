---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: jenfi.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: paidfi.com
  spf: false
hosts:
- cert_expires: Oct 27 22:41:04 2026 GMT
  host: jenfi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 10 23:59:59 2026 GMT
  host: partners.jenfi.com
  hsts: true
  hsts_header: max-age=60; includeSubDomains; preload
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 16:22:58 2026 GMT
  host: paidfi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Jenfi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jenfi, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Jenfi
provider_slug: jenfi
slug: jenfi-domain-security
source_filename: jenfi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: jenfi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 27 22:41:04 2026 GMT\n  hsts: false\n- host: partners.jenfi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 10 23:59:59 2026 GMT\n  hsts: true\n  hsts_header: max-age=60; includeSubDomains; preload\n- host: paidfi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 16:22:58 2026 GMT\n  hsts: false\ndomains:\n- domain: jenfi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: paidfi.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\nnote: 'Extended by hand from live TLS/DNS probes of the two hosts the automated pass\n  did not collect: partners.jenfi.com (the b2b BNPL partner console) and paidfi.com\n  (the PaidFi marketing site). Same method, same date.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jenfi/refs/heads/main/security/jenfi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Financial Services
- Fintech
- Lending
- SME Finance
- Revenue-Based Financing
- Working Capital
- Supply Chain Finance
- Buy Now Pay Later
- Embedded Finance
- Southeast Asia
- Singapore
- Vietnam
---
