---
api_specs:
- filename: soda-co-attributes-api-openapi.yml
  format: yaml
  label: Soda Attributes API
  slug: soda-co-attributes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soda-co/refs/heads/main/openapi/soda-co-attributes-api-openapi.yml
- filename: soda-co-checks-api-openapi.yml
  format: yaml
  label: Soda Checks API
  slug: soda-co-checks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soda-co/refs/heads/main/openapi/soda-co-checks-api-openapi.yml
- filename: soda-co-contracts-api-openapi.yml
  format: yaml
  label: Soda Contracts API
  slug: soda-co-contracts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soda-co/refs/heads/main/openapi/soda-co-contracts-api-openapi.yml
- filename: soda-co-datasets-api-openapi.yml
  format: yaml
  label: Soda Datasets API
  slug: soda-co-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soda-co/refs/heads/main/openapi/soda-co-datasets-api-openapi.yml
- filename: soda-co-datasources-api-openapi.yml
  format: yaml
  label: Soda Datasources API
  slug: soda-co-datasources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soda-co/refs/heads/main/openapi/soda-co-datasources-api-openapi.yml
- filename: soda-co-discovered-datasets-api-openapi.yml
  format: yaml
  label: Soda Discovered Datasets API
  slug: soda-co-discovered-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soda-co/refs/heads/main/openapi/soda-co-discovered-datasets-api-openapi.yml
- filename: soda-co-incidents-api-openapi.yml
  format: yaml
  label: Soda Incidents API
  slug: soda-co-incidents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soda-co/refs/heads/main/openapi/soda-co-incidents-api-openapi.yml
- filename: soda-co-notification-rules-api-openapi.yml
  format: yaml
  label: Soda Notification Rules API
  slug: soda-co-notification-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soda-co/refs/heads/main/openapi/soda-co-notification-rules-api-openapi.yml
- filename: soda-co-runners-api-openapi.yml
  format: yaml
  label: Soda Runners API
  slug: soda-co-runners-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soda-co/refs/heads/main/openapi/soda-co-runners-api-openapi.yml
- filename: soda-co-scans-api-openapi.yml
  format: yaml
  label: Soda Scans API
  slug: soda-co-scans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soda-co/refs/heads/main/openapi/soda-co-scans-api-openapi.yml
- filename: soda-co-secrets-api-openapi.yml
  format: yaml
  label: Soda Secrets API
  slug: soda-co-secrets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soda-co/refs/heads/main/openapi/soda-co-secrets-api-openapi.yml
- filename: soda-co-users-api-openapi.yml
  format: yaml
  label: Soda Users API
  slug: soda-co-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soda-co/refs/heads/main/openapi/soda-co-users-api-openapi.yml
- filename: soda-co-utility-api-openapi.yml
  format: yaml
  label: Soda Utility API
  slug: soda-co-utility-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soda-co/refs/heads/main/openapi/soda-co-utility-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: soda.io
  spf: true
hosts:
- cert_expires: Oct  3 11:18:08 2026 GMT
  host: soda.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 06:28:49 2026 GMT
  host: docs.soda.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 10 23:59:59 2026 GMT
  host: cloud.soda.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Soda Co Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Soda, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Soda
provider_slug: soda-co
slug: soda-co-domain-security
source_filename: soda-co-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: soda.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 11:18:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.soda.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 06:28:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: cloud.soda.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: soda.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/soda-co/refs/heads/main/security/soda-co-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Data Quality
- Data Observability
- Data Contracts
- Data Testing
- Data Monitoring
- Data Engineering
---
