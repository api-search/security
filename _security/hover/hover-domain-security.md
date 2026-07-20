---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: hover.to
  spf: true
hosts:
- cert_expires: Oct 12 03:46:46 2026 GMT
  host: hover.to
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 06:19:42 2026 GMT
  host: developers.hover.to
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hover Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HOVER, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: HOVER
provider_slug: hover
slug: hover-domain-security
source_filename: hover-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hover.to\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 03:46:46 2026 GMT\n  hsts: true\n  hsts_max_age: 0\n- host: developers.hover.to\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 06:19:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: hover.to\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hover/refs/heads/main/security/hover-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Enterprise
- Construction
- Roofing
- Insurance
- 3D Modeling
- Property Data
- Measurements
- Home Services
- Geospatial
---
