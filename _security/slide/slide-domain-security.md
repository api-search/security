---
api_specs:
- filename: slide-openapi-original.json
  format: json
  label: Slide API
  slug: slide-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/slide/refs/heads/main/openapi/slide-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: slide.tech
  spf: true
hosts:
- cert_expires: Sep  3 18:06:33 2026 GMT
  host: slide.tech
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  7 19:00:49 2026 GMT
  host: docs.slide.tech
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 01:36:19 2026 GMT
  host: api.slide.tech
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Slide Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Slide, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Slide
provider_slug: slide
slug: slide-domain-security
source_filename: slide-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: slide.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 18:06:33 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.slide.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 19:00:49 2026 GMT\n  hsts: false\n- host: api.slide.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 01:36:19 2026 GMT\n  hsts: null\ndomains:\n- domain: slide.tech\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/slide/refs/heads/main/security/slide-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Backup
- Disaster Recovery
- Business Continuity
- BCDR
- Managed Service Providers
- MSP
- Data Protection
- Cloud Storage
- Virtualization
---
