---
api_specs:
- filename: cbre-cbre-api-openapi.yml
  format: yaml
  label: CBRE Developer API
  slug: cbre-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cbre/refs/heads/main/openapi/cbre-cbre-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cbre.com
  spf: true
hosts:
- cert_expires: Dec  2 23:59:59 2026 GMT
  host: www.cbre.com
  hsts: true
  hsts_max_age: 10368000
  https: true
  tls_version: TLSv1.3
- host: developer.cbre.com
  https: false
- cert_expires: Aug 16 14:34:30 2026 GMT
  host: api.cbre.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cbre Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CBRE, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: CBRE
provider_slug: cbre
slug: cbre-domain-security
source_filename: cbre-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cbre.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 10368000\n- host: developer.cbre.com\n  https: false\n- host: api.cbre.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 14:34:30 2026 GMT\n  hsts: null\ndomains:\n- domain: cbre.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cbre/refs/heads/main/security/cbre-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Analytics
- Commercial Real Estate
- Facilities Management
- Fortune 500
- Investment Management
- Property Management
- Real Estate
- Valuation
---
