---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: eversettled.com
  spf: true
hosts:
- cert_expires: Aug 22 09:07:36 2026 GMT
  host: eversettled.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Eversettled Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Eversettled, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Eversettled
provider_slug: eversettled
slug: eversettled-domain-security
source_filename: eversettled-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: eversettled.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 09:07:36 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: eversettled.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eversettled/refs/heads/main/security/eversettled-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Estate Settlement
- Probate
- Estate Planning
- Legaltech
- Fintech
- AI Assistant
- Consumer
---
