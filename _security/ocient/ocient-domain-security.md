---
api_specs:
- filename: ocient-ocient-http-query-api-api-openapi.yml
  format: yaml
  label: Ocient Ocient HTTP Query API API
  slug: ocient-ocient-http-query-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ocient/refs/heads/main/openapi/ocient-ocient-http-query-api-api-openapi.yml
- filename: ocient-system-information-rest-endpoints-api-openapi.yml
  format: yaml
  label: Ocient System Information REST Endpoints API
  slug: ocient-system-information-rest-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ocient/refs/heads/main/openapi/ocient-system-information-rest-endpoints-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ocient.com
  spf: true
hosts:
- cert_expires: Oct 20 20:02:40 2026 GMT
  host: ocient.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 18 00:01:53 2026 GMT
  host: docs.ocient.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ocient Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ocient, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Ocient
provider_slug: ocient
slug: ocient-domain-security
source_filename: ocient-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ocient.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 20 20:02:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.ocient.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 00:01:53 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: ocient.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ocient/refs/heads/main/security/ocient-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Data
- Analytics
- Data Warehouse
- Database
- SQL
- Artificial Intelligence
- Machine-Learning
- Big Data
- Geospatial
---
