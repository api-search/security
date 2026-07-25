---
api_specs:
- filename: census-destinations-api-openapi.yml
  format: yaml
  label: Census Destinations API
  slug: census-destinations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/census/refs/heads/main/openapi/census-destinations-api-openapi.yml
- filename: census-models-api-openapi.yml
  format: yaml
  label: Census Models API
  slug: census-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/census/refs/heads/main/openapi/census-models-api-openapi.yml
- filename: census-segments-api-openapi.yml
  format: yaml
  label: Census Segments API
  slug: census-segments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/census/refs/heads/main/openapi/census-segments-api-openapi.yml
- filename: census-sources-api-openapi.yml
  format: yaml
  label: Census Sources API
  slug: census-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/census/refs/heads/main/openapi/census-sources-api-openapi.yml
- filename: census-syncruns-api-openapi.yml
  format: yaml
  label: Census SyncRuns API
  slug: census-syncruns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/census/refs/heads/main/openapi/census-syncruns-api-openapi.yml
- filename: census-syncs-api-openapi.yml
  format: yaml
  label: Census Syncs API
  slug: census-syncs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/census/refs/heads/main/openapi/census-syncs-api-openapi.yml
- filename: census-workspaces-api-openapi.yml
  format: yaml
  label: Census Workspaces API
  slug: census-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/census/refs/heads/main/openapi/census-workspaces-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: getcensus.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: fivetran.com
  spf: true
hosts:
- cert_expires: Aug 20 00:28:15 2026 GMT
  host: www.getcensus.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 19 20:21:54 2026 GMT
  host: fivetran.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 14 23:59:59 2026 GMT
  host: app.getcensus.com
  hsts: true
  hsts_max_age: 631138519
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Census Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Census, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Census
provider_slug: census
slug: census-domain-security
source_filename: census-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.getcensus.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 00:28:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: fivetran.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 20:21:54 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.getcensus.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 631138519\ndomains:\n- domain: getcensus.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: fivetran.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/census/refs/heads/main/security/census-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Connectors
- Data Activation
- Data Warehouse
- Destinations
- Fivetran Activations
- Reverse ETL
- Unified API
---
