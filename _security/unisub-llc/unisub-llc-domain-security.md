---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: unisub.io
  spf: true
hosts:
- cert_expires: Oct 19 10:56:27 2026 GMT
  host: unisub.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Unisub Llc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Unisub LLC, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Unisub LLC
provider_slug: unisub-llc
slug: unisub-llc-domain-security
source_filename: unisub-llc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: unisub.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 19 10:56:27 2026 GMT\n  hsts: false\ndomains:\n- domain: unisub.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unisub-llc/refs/heads/main/security/unisub-llc-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Payments
- Cryptocurrency
- Subscriptions
- Recurring Billing
- Web3
- Blockchain
---
