---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: payvyne.com
  spf: false
hosts:
- cert_expires: Sep 25 10:45:19 2026 GMT
  host: www.payvyne.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vyne Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vyne, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Vyne
provider_slug: vyne
slug: vyne-domain-security
source_filename: vyne-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.payvyne.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 10:45:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: payvyne.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vyne/refs/heads/main/security/vyne-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Financial Services
- Payments
- Open Banking
- Account-to-Account
- Pay-by-Bank
- Fintech
- Acquired
- Defunct
---
