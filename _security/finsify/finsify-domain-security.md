---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: finsify.com
  spf: true
hosts:
- cert_expires: Sep  5 00:03:18 2026 GMT
  host: hub.finsify.com
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Finsify Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Finsify, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Finsify
provider_slug: finsify
slug: finsify-domain-security
source_filename: finsify-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hub.finsify.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 00:03:18 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\ndomains:\n- domain: finsify.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/finsify/refs/heads/main/security/finsify-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Financial Services
- Open Banking
- Bank Aggregation
- Financial Data
- Transactions
- Fintech
- Southeast Asia
---
