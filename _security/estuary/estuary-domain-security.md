---
api_specs:
- filename: estuary-openapi.yml
  format: yaml
  label: Estuary Captures API
  slug: estuary-captures-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/estuary/refs/heads/main/openapi/estuary-openapi.yml
- filename: estuary-openapi.yml
  format: yaml
  label: Estuary Materializations API
  slug: estuary-materializations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/estuary/refs/heads/main/openapi/estuary-openapi.yml
- filename: estuary-openapi.yml
  format: yaml
  label: Estuary Collections API
  slug: estuary-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/estuary/refs/heads/main/openapi/estuary-openapi.yml
- filename: estuary-openapi.yml
  format: yaml
  label: Estuary Catalog Drafts API
  slug: estuary-catalog-drafts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/estuary/refs/heads/main/openapi/estuary-openapi.yml
- filename: estuary-openapi.yml
  format: yaml
  label: Estuary Publications API
  slug: estuary-publications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/estuary/refs/heads/main/openapi/estuary-openapi.yml
- filename: estuary-openapi.yml
  format: yaml
  label: Estuary Connectors API
  slug: estuary-connectors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/estuary/refs/heads/main/openapi/estuary-openapi.yml
- filename: estuary-openapi.yml
  format: yaml
  label: Estuary Tenants & Billing API
  slug: estuary-tenants-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/estuary/refs/heads/main/openapi/estuary-openapi.yml
- filename: estuary-openapi.yml
  format: yaml
  label: Estuary Auth & Tokens API
  slug: estuary-auth-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/estuary/refs/heads/main/openapi/estuary-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: estuary.dev
  spf: true
hosts:
- cert_expires: Sep 10 23:09:48 2026 GMT
  host: estuary.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 02:44:19 2026 GMT
  host: docs.estuary.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 25 00:08:28 2026 GMT
  host: api.estuary.dev
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Estuary Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Estuary, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Estuary
provider_slug: estuary
slug: estuary-domain-security
source_filename: estuary-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: estuary.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 23:09:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.estuary.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 02:44:19 2026 GMT\n  hsts: false\n- host: api.estuary.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 00:08:28 2026 GMT\n  hsts: null\ndomains:\n- domain: estuary.dev\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/estuary/refs/heads/main/security/estuary-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Data Integration
- Streaming ETL
- Change Data Capture
- CDC
- Real-Time Data
- Data Pipelines
---
