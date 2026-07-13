---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Keboola Storage API
  slug: storage-api
  spec_type: OpenAPI
  url: https://api.keboola.com/?service=storage
- filename: openapi.yaml
  format: yaml
  label: Keboola Management API
  slug: management-api
  spec_type: OpenAPI
  url: https://api.keboola.com/?service=manage
- filename: openapi.yaml
  format: yaml
  label: Keboola Queue API
  slug: queue-api
  spec_type: OpenAPI
  url: https://api.keboola.com/?service=job-queue
- filename: openapi.yaml
  format: yaml
  label: Keboola Scheduler API
  slug: scheduler-api
  spec_type: OpenAPI
  url: https://api.keboola.com/?service=scheduler
- filename: openapi.yaml
  format: yaml
  label: Keboola Developer Portal API
  slug: developer-portal-api
  spec_type: OpenAPI
  url: https://api.keboola.com/?service=developer-portal
- filename: openapi.yaml
  format: yaml
  label: Keboola Encryption API
  slug: encryption-api
  spec_type: OpenAPI
  url: https://api.keboola.com/?service=encryption
- filename: openapi.yaml
  format: yaml
  label: Keboola Notifications API
  slug: notifications-api
  spec_type: OpenAPI
  url: https://api.keboola.com/?service=notification
- filename: openapi.yaml
  format: yaml
  label: Keboola OAuth Broker API
  slug: oauth-broker-api
  spec_type: OpenAPI
  url: https://api.keboola.com/?service=oauth
- filename: openapi.yaml
  format: yaml
  label: Keboola Stream API
  slug: stream-api
  spec_type: OpenAPI
  url: https://api.keboola.com/?service=stream
- filename: openapi.yaml
  format: yaml
  label: Keboola Query API
  slug: query-api
  spec_type: OpenAPI
  url: https://api.keboola.com/?service=query
- filename: openapi.yaml
  format: yaml
  label: Keboola Sandboxes Service API
  slug: sandboxes-api
  spec_type: OpenAPI
  url: https://api.keboola.com/?service=sandboxes-service
- filename: openapi.yaml
  format: yaml
  label: Keboola Vault API
  slug: vault-api
  spec_type: OpenAPI
  url: https://api.keboola.com/?service=vault
- filename: openapi.yaml
  format: yaml
  label: Keboola Billing API
  slug: billing-api
  spec_type: OpenAPI
  url: https://api.keboola.com/?service=billing
- filename: openapi.yaml
  format: yaml
  label: Keboola AI API
  slug: ai-api
  spec_type: OpenAPI
  url: https://api.keboola.com/?service=ai
- filename: openapi.yaml
  format: yaml
  label: Keboola Importer API
  slug: importer-api
  spec_type: OpenAPI
  url: https://api.keboola.com/?service=import
- filename: openapi.yaml
  format: yaml
  label: Keboola Editor API
  slug: editor-api
  spec_type: OpenAPI
  url: https://api.keboola.com/?service=editor
- filename: openapi.yaml
  format: yaml
  label: Keboola Synchronous Actions API
  slug: sync-actions-api
  spec_type: OpenAPI
  url: https://api.keboola.com/?service=sync-actions
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  - 0 iodef "mailto:security@keboola.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: keboola.com
  spf: true
hosts:
- cert_expires: Sep 25 13:51:36 2026 GMT
  host: www.keboola.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 11 23:59:59 2027 GMT
  host: api.keboola.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Feb 11 23:59:59 2027 GMT
  host: connection.keboola.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Keboola Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Keboola, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Keboola
provider_slug: keboola
slug: keboola-domain-security
source_filename: keboola-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.keboola.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 13:51:36 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.keboola.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 11 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: connection.keboola.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 11 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: keboola.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  - 0 iodef \"mailto:security@keboola.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/keboola/refs/heads/main/security/keboola-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Data Platform
- ETL
- ELT
- Data Pipelines
- Data Storage
- Transformations
- Orchestration
- Data Operations
- Cloud Data
- Snowflake
- BigQuery
---
