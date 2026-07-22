---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: waypay.ca
  spf: true
hosts:
- host: waypay.ca
  https: false
kind: domain-security
layout: security
method: probed
name: Waypay Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for WayPay, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: WayPay
provider_slug: waypay
slug: waypay-domain-security
source_filename: waypay-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: waypay.ca\n  https: false\ndomains:\n- domain: waypay.ca\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/waypay/refs/heads/main/security/waypay-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Payments
- Fintech
- Accounts Payable
- B2B
- Canada
- Financial Services
- Acquired
---
