---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: bringy.com
  spf: true
hosts:
- cert_expires: Sep  1 11:24:26 2026 GMT
  host: bringy.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bringy Inc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bringy, Inc., probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Bringy, Inc.
provider_slug: bringy-inc
slug: bringy-inc-domain-security
source_filename: bringy-inc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bringy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 11:24:26 2026 GMT\n  hsts: false\ndomains:\n- domain: bringy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bringy-inc/refs/heads/main/security/bringy-inc-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Insurance
- InsurTech
- Financial Services
- Insurance Brokerage
- Fintech
- Egypt
- Consumer
---
