---
api_specs:
- filename: acceldata-alerts-api-openapi.yml
  format: yaml
  label: Acceldata Alerts API
  slug: acceldata-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acceldata/refs/heads/main/openapi/acceldata-alerts-api-openapi.yml
- filename: acceldata-data-quality-rules-api-openapi.yml
  format: yaml
  label: Acceldata Data Quality Rules API
  slug: acceldata-data-quality-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acceldata/refs/heads/main/openapi/acceldata-data-quality-rules-api-openapi.yml
- filename: acceldata-datasets-api-openapi.yml
  format: yaml
  label: Acceldata Datasets API
  slug: acceldata-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acceldata/refs/heads/main/openapi/acceldata-datasets-api-openapi.yml
- filename: acceldata-lineage-api-openapi.yml
  format: yaml
  label: Acceldata Lineage API
  slug: acceldata-lineage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acceldata/refs/heads/main/openapi/acceldata-lineage-api-openapi.yml
- filename: acceldata-pipeline-jobs-api-openapi.yml
  format: yaml
  label: Acceldata Pipeline Jobs API
  slug: acceldata-pipeline-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acceldata/refs/heads/main/openapi/acceldata-pipeline-jobs-api-openapi.yml
- filename: acceldata-roles-api-openapi.yml
  format: yaml
  label: Acceldata Roles API
  slug: acceldata-roles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acceldata/refs/heads/main/openapi/acceldata-roles-api-openapi.yml
- filename: acceldata-users-api-openapi.yml
  format: yaml
  label: Acceldata Users API
  slug: acceldata-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acceldata/refs/heads/main/openapi/acceldata-users-api-openapi.yml
- filename: acceldata-catalog-api-openapi.json
  format: json
  label: Acceldata Catalog API
  slug: acceldata-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acceldata/refs/heads/main/openapi/_original/acceldata-catalog-api-openapi.json
- filename: acceldata-administration-api-openapi.json
  format: json
  label: Acceldata Administration API
  slug: acceldata-administration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acceldata/refs/heads/main/openapi/_original/acceldata-administration-api-openapi.json
- filename: acceldata-tags-api-openapi.json
  format: json
  label: Acceldata Tag Services API
  slug: acceldata-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acceldata/refs/heads/main/openapi/_original/acceldata-tags-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: acceldata.io
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: acceldata.app
  spf: false
hosts:
- cert_expires: Oct 15 01:55:38 2026 GMT
  host: www.acceldata.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 13 23:59:59 2027 GMT
  host: accounts.acceldata.app
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 08:22:21 2026 GMT
  host: docs.acceldata.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Acceldata Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Acceldata, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Acceldata
provider_slug: acceldata
slug: acceldata-domain-security
source_filename: acceldata-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.acceldata.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 01:55:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: accounts.acceldata.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 13 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.acceldata.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  4 08:22:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: acceldata.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: acceldata.app\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/acceldata/refs/heads/main/security/acceldata-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI Agents
- Data Management
- Data Observability
- Data Pipeline
- Data Quality
- Intelligence
- Observability
---
