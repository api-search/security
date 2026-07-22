---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: forwardlane.com
  spf: true
hosts:
- cert_expires: Sep 15 12:30:53 2026 GMT
  host: forwardlane.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Forwardlane Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Forwardlane, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Forwardlane
provider_slug: forwardlane
slug: forwardlane-domain-security
source_filename: forwardlane-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: forwardlane.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 12:30:53 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: forwardlane.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/forwardlane/refs/heads/main/security/forwardlane-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Decision Intelligence
- Enterprise AI
- Financial Services
- Private Markets
- Natural Language Analytics
- Compliance
- Wealth Management
---
