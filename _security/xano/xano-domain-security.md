---
api_specs:
- filename: xano-openapi.yml
  format: yaml
  label: Xano Metadata Tables & Schema API
  slug: xano-metadata-tables-schema-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xano/refs/heads/main/openapi/xano-openapi.yml
- filename: xano-openapi.yml
  format: yaml
  label: Xano Metadata Records & Content API
  slug: xano-metadata-records-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xano/refs/heads/main/openapi/xano-openapi.yml
- filename: xano-openapi.yml
  format: yaml
  label: Xano Metadata Files API
  slug: xano-metadata-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xano/refs/heads/main/openapi/xano-openapi.yml
- filename: xano-openapi.yml
  format: yaml
  label: Xano Metadata Branches & Workspace API
  slug: xano-metadata-branches-workspace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xano/refs/heads/main/openapi/xano-openapi.yml
- filename: xano-openapi.yml
  format: yaml
  label: Xano Metadata API Groups & Endpoints API
  slug: xano-metadata-api-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xano/refs/heads/main/openapi/xano-openapi.yml
- filename: xano-openapi.yml
  format: yaml
  label: Xano Metadata Auth & Access API
  slug: xano-metadata-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xano/refs/heads/main/openapi/xano-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: xano.com
  spf: true
hosts:
- cert_expires: Aug 15 10:47:19 2026 GMT
  host: www.xano.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  4 03:53:08 2026 GMT
  host: docs.xano.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Xano Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Xano, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Xano
provider_slug: xano
slug: xano-domain-security
source_filename: xano-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.xano.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 15 10:47:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.xano.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 03:53:08 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: xano.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xano/refs/heads/main/security/xano-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- No Code
- Backend as a Service
- BaaS
- API Builder
- Database
- Serverless
---
