---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ceezer.earth
  spf: true
hosts:
- cert_expires: Oct 16 10:41:05 2026 GMT
  host: ceezer.earth
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ceezer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CEEZER, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: CEEZER
provider_slug: ceezer
slug: ceezer-domain-security
source_filename: ceezer-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ceezer.earth\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 10:41:05 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ceezer.earth\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ceezer/refs/heads/main/security/ceezer-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Marketplace
- Climate
- Carbon Credits
- Sustainability
- Carbon Markets
- Net Zero
- Energy Attribute Certificates
- ESG
---
