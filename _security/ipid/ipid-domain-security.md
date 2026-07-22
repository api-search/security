---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ipid.tech
  spf: true
hosts:
- cert_expires: Sep 16 16:09:28 2026 GMT
  host: ipid.tech
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ipid Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ipid, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Ipid
provider_slug: ipid
slug: ipid-domain-security
source_filename: ipid-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ipid.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 16:09:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ipid.tech\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ipid/refs/heads/main/security/ipid-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Payments
- Fraud Prevention
- Identity Verification
- Compliance
- Cross-Border Payments
- Know Your Payee
- Fintech
- Bank Account Verification
---
