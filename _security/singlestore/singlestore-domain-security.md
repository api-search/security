---
api_specs:
- filename: singlestore-data-api-openapi.yml
  format: yaml
  label: SingleStore Data API
  slug: data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/singlestore/refs/heads/main/openapi/singlestore-data-api-openapi.yml
- filename: singlestore-management-api-openapi.yml
  format: yaml
  label: SingleStore Management API
  slug: management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/singlestore/refs/heads/main/openapi/singlestore-management-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: singlestore.com
  spf: true
hosts:
- cert_expires: Oct  4 23:59:59 2026 GMT
  host: www.singlestore.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 30 23:59:59 2027 GMT
  host: docs.singlestore.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 03:39:23 2026 GMT
  host: api.singlestore.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Singlestore Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SingleStore, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: SingleStore
provider_slug: singlestore
slug: singlestore-domain-security
source_filename: singlestore-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.singlestore.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.singlestore.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 30 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.singlestore.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 03:39:23 2026 GMT\n  hsts: null\ndomains:\n- domain: singlestore.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/singlestore/refs/heads/main/security/singlestore-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Database
- SQL
- Analytics
- Cloud
- Distributed SQL
---
