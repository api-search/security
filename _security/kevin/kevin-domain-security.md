---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: kevin.eu
  spf: true
hosts:
- host: www.kevin.eu
  https: false
kind: domain-security
layout: security
method: probed
name: Kevin Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kevin., probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Kevin.
provider_slug: kevin
slug: kevin-domain-security
source_filename: kevin-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.kevin.eu\n  https: false\ndomains:\n- domain: kevin.eu\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kevin/refs/heads/main/security/kevin-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Payments
- Open Banking
- Account to Account
- PSD2
- Fintech
- Bank Payments
- Payment Initiation
- Account Information
- Europe
---
