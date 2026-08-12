---
api_specs:
- filename: openserp-oss-openapi.yml
  format: yaml
  label: OpenSERP Server (self-hosted)
  slug: openserp-oss
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openserp/refs/heads/main/openapi/openserp-oss-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: openserp.org
  spf: true
hosts:
- cert_expires: Nov  6 21:12:58 2026 GMT
  host: openserp.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  8 01:23:10 2026 GMT
  host: api.openserp.org
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: 127.0.0.1
  https: false
kind: domain-security
layout: security
method: probed
name: Openserp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpenSERP, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: OpenSERP
provider_slug: openserp
slug: openserp-domain-security
source_filename: openserp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: openserp.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 21:12:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.openserp.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  8 01:23:10 2026 GMT\n  hsts: null\n- host: 127.0.0.1\n  https: false\ndomains:\n- domain: openserp.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openserp/refs/heads/main/security/openserp-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Search
- SERP
- Search API
- Web Scraping
- Content Extraction
- AI Grounding
- Rank Tracking
- Open Source
- Developer Tools
---
