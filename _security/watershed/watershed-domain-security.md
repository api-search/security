---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: watershed.com
  spf: true
hosts:
- cert_expires: Aug 15 06:34:36 2026 GMT
  host: watershed.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Watershed Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Watershed, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Watershed
provider_slug: watershed
slug: watershed-domain-security
source_filename: watershed-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: watershed.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 15 06:34:36 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: watershed.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/watershed/refs/heads/main/security/watershed-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Climate
- Carbon Accounting
- ESG
- Sustainability
- Disclosure
- CSRD
- SBTi
- Decarbonization
- Scope 3
- Enterprise
- Reporting
---
