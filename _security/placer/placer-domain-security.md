---
api_specs:
- filename: placer-papi-openapi.json
  format: json
  label: Placer Public API (PAPI)
  slug: placer-public-api-papi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/placer/refs/heads/main/openapi/placer-papi-openapi.json
description: ''
domains:
- caa:
  - 0 contactemail "admin@placer.ai"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: placer.ai
  spf: true
hosts:
- cert_expires: Oct  2 09:41:26 2026 GMT
  host: placer.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 23 08:43:21 2026 GMT
  host: papi.placer.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Placer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Placer, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Placer
provider_slug: placer
slug: placer-domain-security
source_filename: placer-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: placer.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 09:41:26 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: papi.placer.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 08:43:21 2026 GMT\n  hsts: null\ndomains:\n- domain: placer.ai\n  dnssec: false\n  caa:\n  - 0 contactemail \"admin@placer.ai\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/placer/refs/heads/main/security/placer-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Location Analytics
- Foot Traffic
- Geospatial
- Retail Analytics
- Real Estate
- Consumer Insights
- Data
---
