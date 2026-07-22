---
api_specs:
- filename: upsun-openapi-original.json
  format: json
  label: Upsun REST API
  slug: upsun-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upsun/refs/heads/main/openapi/upsun-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: upsun.com
  spf: true
hosts:
- cert_expires: Sep  3 03:29:55 2026 GMT
  host: upsun.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 11 13:16:30 2026 GMT
  host: developer.upsun.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 13 07:18:51 2026 GMT
  host: api.upsun.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Upsun Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Upsun, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Upsun
provider_slug: upsun
slug: upsun-domain-security
source_filename: upsun-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: upsun.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 03:29:55 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\n- host: developer.upsun.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 13:16:30 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.upsun.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 07:18:51 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: upsun.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/upsun/refs/heads/main/security/upsun-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Infrastructure Saas
- Cloud
- PaaS
- Hosting
- Deployment
- DevOps
- Containers
- Observability
---
