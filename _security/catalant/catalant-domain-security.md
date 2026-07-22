---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: catalant.com
  spf: false
hosts:
- cert_expires: Sep 19 23:59:59 2026 GMT
  host: catalant.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Catalant Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Catalant, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: Catalant
provider_slug: catalant
slug: catalant-domain-security
source_filename: catalant-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: catalant.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: catalant.com\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/catalant/refs/heads/main/security/catalant-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- Company
- Consulting
- Talent Marketplace
- Professional Services
- Independent Consultants
- Strategy
- Digital and AI
- Expert Network
---
