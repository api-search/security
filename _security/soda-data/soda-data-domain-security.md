---
api_specs:
- filename: soda-data-cloud-api-v4-openapi.yml
  format: yaml
  label: Soda Cloud API v4
  slug: soda-data
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soda-data/refs/heads/main/openapi/_original/soda-data-cloud-api-v4-openapi.yml
- filename: soda-data-attributes-api-openapi.yml
  format: yaml
  label: Soda Attributes API
  slug: soda-data-attributes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soda-data/refs/heads/main/openapi/soda-data-attributes-api-openapi.yml
- filename: soda-data-checks-api-openapi.yml
  format: yaml
  label: Soda Checks API
  slug: soda-data-checks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soda-data/refs/heads/main/openapi/soda-data-checks-api-openapi.yml
- filename: soda-data-contracts-api-openapi.yml
  format: yaml
  label: Soda Contracts API
  slug: soda-data-contracts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soda-data/refs/heads/main/openapi/soda-data-contracts-api-openapi.yml
- filename: soda-data-data-standards-api-openapi.yml
  format: yaml
  label: Soda Data Standards API
  slug: soda-data-data-standards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soda-data/refs/heads/main/openapi/soda-data-data-standards-api-openapi.yml
- filename: soda-data-datasets-api-openapi.yml
  format: yaml
  label: Soda Datasets API
  slug: soda-data-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soda-data/refs/heads/main/openapi/soda-data-datasets-api-openapi.yml
- filename: soda-data-datasources-api-openapi.yml
  format: yaml
  label: Soda Datasources API
  slug: soda-data-datasources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soda-data/refs/heads/main/openapi/soda-data-datasources-api-openapi.yml
- filename: soda-data-discovered-datasets-api-openapi.yml
  format: yaml
  label: Soda Discovered Datasets API
  slug: soda-data-discovered-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soda-data/refs/heads/main/openapi/soda-data-discovered-datasets-api-openapi.yml
- filename: soda-data-incidents-api-openapi.yml
  format: yaml
  label: Soda Incidents API
  slug: soda-data-incidents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soda-data/refs/heads/main/openapi/soda-data-incidents-api-openapi.yml
- filename: soda-data-licensing-api-openapi.yml
  format: yaml
  label: Soda Licensing API
  slug: soda-data-licensing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soda-data/refs/heads/main/openapi/soda-data-licensing-api-openapi.yml
- filename: soda-data-notification-rules-api-openapi.yml
  format: yaml
  label: Soda Notification Rules API
  slug: soda-data-notification-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soda-data/refs/heads/main/openapi/soda-data-notification-rules-api-openapi.yml
- filename: soda-data-runners-api-openapi.yml
  format: yaml
  label: Soda Runners API
  slug: soda-data-runners-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soda-data/refs/heads/main/openapi/soda-data-runners-api-openapi.yml
- filename: soda-data-scans-api-openapi.yml
  format: yaml
  label: Soda Scans API
  slug: soda-data-scans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soda-data/refs/heads/main/openapi/soda-data-scans-api-openapi.yml
- filename: soda-data-secrets-api-openapi.yml
  format: yaml
  label: Soda Secrets API
  slug: soda-data-secrets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soda-data/refs/heads/main/openapi/soda-data-secrets-api-openapi.yml
- filename: soda-data-users-api-openapi.yml
  format: yaml
  label: Soda Users API
  slug: soda-data-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soda-data/refs/heads/main/openapi/soda-data-users-api-openapi.yml
- filename: soda-data-utility-api-openapi.yml
  format: yaml
  label: Soda Utility API
  slug: soda-data-utility-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soda-data/refs/heads/main/openapi/soda-data-utility-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: soda.io
  spf: true
hosts:
- cert_expires: Oct  3 15:10:10 2026 GMT
  host: www.soda.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 26 23:59:59 2027 GMT
  host: cloud.soda.io
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 28 23:59:59 2027 GMT
  host: cloud.us.soda.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Soda Data Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Soda, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Soda
provider_slug: soda-data
slug: soda-data-domain-security
source_filename: soda-data-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.soda.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 15:10:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: cloud.soda.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 26 23:59:59 2027 GMT\n  hsts: null\n- host: cloud.us.soda.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 28 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: soda.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/soda-data/refs/heads/main/security/soda-data-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AIOps
- Data Quality
- Data Observability
- Data Contracts
- Data Governance
- Anomaly Detection
- Data Monitoring
- Data Testing
---
