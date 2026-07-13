---
api_specs:
- filename: cognite-data-fusion-api.yaml
  format: yaml
  label: Cognite Data Fusion API
  slug: cognite-data-fusion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cognite/refs/heads/main/openapi/cognite-data-fusion-api.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cognite.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cognitedata.com
  spf: true
hosts:
- cert_expires: Aug 27 06:18:16 2026 GMT
  host: www.cognite.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 11:32:42 2026 GMT
  host: api-docs.cognite.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 29 22:04:59 2026 GMT
  host: api.cognitedata.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cognite Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cognite, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Cognite
provider_slug: cognite
slug: cognite-domain-security
source_filename: cognite-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cognite.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 06:18:16 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api-docs.cognite.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 11:32:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.cognitedata.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 22:04:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: cognite.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: cognitedata.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cognite/refs/heads/main/security/cognite-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Industrial IoT
- Manufacturing
- Industrial Data
- Digital Twin
- Asset Management
- Time Series
- Industrial AI
---
