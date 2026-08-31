---
api_specs:
- filename: metaplane-api-openapi.yml
  format: yaml
  label: Metaplane API
  slug: metaplane
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metaplane/refs/heads/main/openapi/_original/metaplane-api-openapi.yml
- filename: metaplane-connections-api-openapi.yml
  format: yaml
  label: Metaplane Connections API
  slug: metaplane-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metaplane/refs/heads/main/openapi/metaplane-connections-api-openapi.yml
- filename: metaplane-monitors-api-openapi.yml
  format: yaml
  label: Metaplane Monitors API
  slug: metaplane-monitors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metaplane/refs/heads/main/openapi/metaplane-monitors-api-openapi.yml
- filename: metaplane-tags-api-openapi.yml
  format: yaml
  label: Metaplane Tags API
  slug: metaplane-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metaplane/refs/heads/main/openapi/metaplane-tags-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: metaplane.dev
  spf: true
hosts:
- cert_expires: Oct 15 13:45:36 2026 GMT
  host: www.metaplane.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 26 20:45:25 2026 GMT
  host: dev.api.metaplane.dev
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Metaplane Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Metaplane, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Metaplane
provider_slug: metaplane
slug: metaplane-domain-security
source_filename: metaplane-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.metaplane.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 13:45:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: dev.api.metaplane.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 20:45:25 2026 GMT\n  hsts: null\ndomains:\n- domain: metaplane.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/metaplane/refs/heads/main/security/metaplane-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AIOps
- Data Observability
- Data Quality
- Anomaly Detection
- Data Lineage
- Monitoring
- Analytics
- Data Engineering
- dbt
- Snowflake
---
