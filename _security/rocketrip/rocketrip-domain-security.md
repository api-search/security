---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: rocketrip.com
  spf: true
hosts:
- cert_expires: Dec 23 13:08:55 2026 GMT
  host: rocketrip.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rocketrip Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rocketrip, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Rocketrip
provider_slug: rocketrip
slug: rocketrip-domain-security
source_filename: rocketrip-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: rocketrip.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 13:08:55 2026 GMT\n  hsts: null\ndomains:\n- domain: rocketrip.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rocketrip/refs/heads/main/security/rocketrip-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Travel
- Corporate Travel
- Expense Management
- Travel Management
- Fintech
- Rewards
---
