---
api_specs:
- filename: overview
  format: yaml
  label: Census Management API
  slug: census-management-api
  spec_type: Postman
  url: https://www.postman.com/getcensus/workspace/census-api/overview
- filename: getcensus-destinations-api-openapi.yml
  format: yaml
  label: Census Destinations API
  slug: getcensus-destinations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getcensus/refs/heads/main/openapi/getcensus-destinations-api-openapi.yml
- filename: getcensus-models-api-openapi.yml
  format: yaml
  label: Census Models API
  slug: getcensus-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getcensus/refs/heads/main/openapi/getcensus-models-api-openapi.yml
- filename: getcensus-segments-api-openapi.yml
  format: yaml
  label: Census Segments API
  slug: getcensus-segments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getcensus/refs/heads/main/openapi/getcensus-segments-api-openapi.yml
- filename: getcensus-sources-api-openapi.yml
  format: yaml
  label: Census Sources API
  slug: getcensus-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getcensus/refs/heads/main/openapi/getcensus-sources-api-openapi.yml
- filename: getcensus-syncruns-api-openapi.yml
  format: yaml
  label: Census Sync Runs API
  slug: getcensus-syncruns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getcensus/refs/heads/main/openapi/getcensus-syncruns-api-openapi.yml
- filename: getcensus-syncs-api-openapi.yml
  format: yaml
  label: Census Syncs API
  slug: getcensus-syncs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getcensus/refs/heads/main/openapi/getcensus-syncs-api-openapi.yml
- filename: getcensus-workspaces-api-openapi.yml
  format: yaml
  label: Census Workspaces API
  slug: getcensus-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getcensus/refs/heads/main/openapi/getcensus-workspaces-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: getcensus.com
  spf: true
hosts:
- cert_expires: Oct 18 01:46:34 2026 GMT
  host: www.getcensus.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 28 23:59:59 2027 GMT
  host: developers.getcensus.com
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
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Getcensus Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Census, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Census
provider_slug: getcensus
slug: getcensus-domain-security
source_filename: getcensus-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.getcensus.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 01:46:34 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.getcensus.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 28 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.getcensus.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 631138519\ndomains:\n- domain: getcensus.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/getcensus/refs/heads/main/security/getcensus-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Sync
- Census
- Reverse ETL
- Data Activation
- Data Warehouse
- CRM
- Marketing Automation
- Segments
- SQL
---
