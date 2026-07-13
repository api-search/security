---
api_specs:
- filename: up42-openapi.yml
  format: yaml
  label: UP42 Catalog API
  slug: up42-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/up42/refs/heads/main/openapi/up42-openapi.yml
- filename: up42-openapi.yml
  format: yaml
  label: UP42 Tasking API
  slug: up42-tasking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/up42/refs/heads/main/openapi/up42-openapi.yml
- filename: up42-openapi.yml
  format: yaml
  label: UP42 Orders API
  slug: up42-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/up42/refs/heads/main/openapi/up42-openapi.yml
- filename: up42-openapi.yml
  format: yaml
  label: UP42 Storage Assets API
  slug: up42-storage-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/up42/refs/heads/main/openapi/up42-openapi.yml
- filename: up42-openapi.yml
  format: yaml
  label: UP42 STAC Data Management API
  slug: up42-stac-data-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/up42/refs/heads/main/openapi/up42-openapi.yml
- filename: up42-openapi.yml
  format: yaml
  label: UP42 Processing API
  slug: up42-processing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/up42/refs/heads/main/openapi/up42-openapi.yml
- filename: up42-openapi.yml
  format: yaml
  label: UP42 Webhooks API
  slug: up42-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/up42/refs/heads/main/openapi/up42-openapi.yml
- filename: up42-openapi.yml
  format: yaml
  label: UP42 Workspaces and Account API
  slug: up42-workspaces-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/up42/refs/heads/main/openapi/up42-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: up42.com
  spf: true
hosts:
- cert_expires: Oct  7 09:55:08 2026 GMT
  host: up42.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 01:52:24 2026 GMT
  host: docs.up42.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 01:52:24 2026 GMT
  host: api.up42.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Up42 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for UP42, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: UP42
provider_slug: up42
slug: up42-domain-security
source_filename: up42-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: up42.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 09:55:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.up42.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 01:52:24 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.up42.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 01:52:24 2026 GMT\n  hsts: null\ndomains:\n- domain: up42.com\n  dnssec: true\n  caa:\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/up42/refs/heads/main/security/up42-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Geospatial
- Earth Observation
- Satellite Imagery
- Remote Sensing
- STAC
- Tasking
- Catalog
- Airbus
---
