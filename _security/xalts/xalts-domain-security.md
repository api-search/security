---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: xalts.io
  spf: true
hosts:
- cert_expires: Aug 21 13:52:07 2026 GMT
  host: xalts.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Xalts Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Xalts, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Xalts
provider_slug: xalts
slug: xalts-domain-security
source_filename: xalts-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: xalts.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 13:52:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: xalts.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xalts/refs/heads/main/security/xalts-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Treasury
- Trade Finance
- AI Agents
- Banking
- Liquidity
---
