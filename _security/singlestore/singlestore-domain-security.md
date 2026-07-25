---
api_specs:
- filename: singlestore-files-api-openapi.yml
  format: yaml
  label: SingleStore Files API
  slug: singlestore-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/singlestore/refs/heads/main/openapi/singlestore-files-api-openapi.yml
- filename: singlestore-health-api-openapi.yml
  format: yaml
  label: SingleStore Health API
  slug: singlestore-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/singlestore/refs/heads/main/openapi/singlestore-health-api-openapi.yml
- filename: singlestore-jobs-api-openapi.yml
  format: yaml
  label: SingleStore Jobs API
  slug: singlestore-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/singlestore/refs/heads/main/openapi/singlestore-jobs-api-openapi.yml
- filename: singlestore-organizations-api-openapi.yml
  format: yaml
  label: SingleStore Organizations API
  slug: singlestore-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/singlestore/refs/heads/main/openapi/singlestore-organizations-api-openapi.yml
- filename: singlestore-queries-api-openapi.yml
  format: yaml
  label: SingleStore Queries API
  slug: singlestore-queries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/singlestore/refs/heads/main/openapi/singlestore-queries-api-openapi.yml
- filename: singlestore-regions-api-openapi.yml
  format: yaml
  label: SingleStore Regions API
  slug: singlestore-regions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/singlestore/refs/heads/main/openapi/singlestore-regions-api-openapi.yml
- filename: singlestore-secrets-api-openapi.yml
  format: yaml
  label: SingleStore Secrets API
  slug: singlestore-secrets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/singlestore/refs/heads/main/openapi/singlestore-secrets-api-openapi.yml
- filename: singlestore-workspacegroups-api-openapi.yml
  format: yaml
  label: SingleStore WorkspaceGroups API
  slug: singlestore-workspacegroups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/singlestore/refs/heads/main/openapi/singlestore-workspacegroups-api-openapi.yml
- filename: singlestore-workspaces-api-openapi.yml
  format: yaml
  label: SingleStore Workspaces API
  slug: singlestore-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/singlestore/refs/heads/main/openapi/singlestore-workspaces-api-openapi.yml
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
