---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: sourceful.com
  spf: true
hosts:
- cert_expires: Aug 27 09:09:40 2026 GMT
  host: www.sourceful.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sourceful Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sourceful, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Sourceful
provider_slug: sourceful
slug: sourceful-domain-security
source_filename: sourceful-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sourceful.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 09:09:40 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: sourceful.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sourceful/refs/heads/main/security/sourceful-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Packaging
- Sustainable Packaging
- Packaging Design
- Visual AI
- Generative AI
- Image Editing
- Brand Design
- Logo Design
- Product Photography
- Carbon Footprint
- Life Cycle Assessment
- Sustainability
- Manufacturing
- Marketplace
- Consumer Brands
- ISO 42001
- Riverflow
- Manchester
- United Kingdom
---
