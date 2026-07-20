---
api_specs:
- filename: land-insight-api-openapi.yml
  format: yaml
  label: LandTech API
  slug: land-insight-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/land-insight/refs/heads/main/openapi/land-insight-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: land.tech
  spf: true
hosts:
- cert_expires: Sep  4 10:25:59 2026 GMT
  host: land.tech
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 20 23:59:59 2026 GMT
  host: app.land.tech
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Land Insight Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Land Insight, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Land Insight
provider_slug: land-insight
slug: land-insight-domain-security
source_filename: land-insight-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: land.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 10:25:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.land.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 20 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: land.tech\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/land-insight/refs/heads/main/security/land-insight-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Real Estate
- Property
- Land
- Planning
- Geospatial
- Data
- United Kingdom
- PropTech
- Construction
---
