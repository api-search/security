---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: spotlock.co
  spf: true
hosts:
- cert_expires: Sep  3 16:32:17 2026 GMT
  host: spotlock.co
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Spotlock Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Spotlock, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Spotlock
provider_slug: spotlock
slug: spotlock-domain-security
source_filename: spotlock-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: spotlock.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 16:32:17 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: spotlock.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spotlock/refs/heads/main/security/spotlock-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Commodity Risk Management
- Hedging
- Risk Management
- Commodities
- Procurement
- Price Intelligence
- Fintech
- Construction
- Manufacturing
---
