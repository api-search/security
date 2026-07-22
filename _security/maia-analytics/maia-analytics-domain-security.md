---
api_specs:
- filename: maia-analytics-openapi-original.json
  format: json
  label: MAIA API
  slug: maia-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maia-analytics/refs/heads/main/openapi/maia-analytics-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: maia-analytics.com
  spf: true
hosts:
- cert_expires: Aug 25 14:48:32 2026 GMT
  host: www.maia-analytics.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Maia Analytics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Maia-analytics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Maia-analytics
provider_slug: maia-analytics
slug: maia-analytics-domain-security
source_filename: maia-analytics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.maia-analytics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 14:48:32 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: maia-analytics.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/maia-analytics/refs/heads/main/security/maia-analytics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Developer Tools
- Geospatial
- GIS
- Location Intelligence
- Mapping
- Artificial Intelligence
- Analytics
---
