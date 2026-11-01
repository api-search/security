---
api_specs:
- filename: past-dev-audiences-api-openapi.yml
  format: yaml
  label: past-dev Audiences API
  slug: past-dev-audiences-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/past-dev/openapi/past-dev-audiences-api-openapi.yml
- filename: past-dev-debugging-api-openapi.yml
  format: yaml
  label: past-dev Debugging API
  slug: past-dev-debugging-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/past-dev/openapi/past-dev-debugging-api-openapi.yml
- filename: past-dev-identities-api-openapi.yml
  format: yaml
  label: past-dev Identities API
  slug: past-dev-identities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/past-dev/openapi/past-dev-identities-api-openapi.yml
- filename: past-dev-ingestion-api-openapi.yml
  format: yaml
  label: past-dev Ingestion API
  slug: past-dev-ingestion-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/past-dev/openapi/past-dev-ingestion-api-openapi.yml
- filename: past-dev-management-api-openapi.yml
  format: yaml
  label: past-dev Management API
  slug: past-dev-management-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/past-dev/openapi/past-dev-management-api-openapi.yml
- filename: past-dev-recall-api-openapi.yml
  format: yaml
  label: past-dev Recall API
  slug: past-dev-recall-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/past-dev/openapi/past-dev-recall-api-openapi.yml
- filename: past-dev-webhooks-api-openapi.yml
  format: yaml
  label: past-dev Webhooks API
  slug: past-dev-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/past-dev/openapi/past-dev-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: past.dev
  spf: true
hosts:
- cert_expires: Jan 17 16:34:41 2027 GMT
  host: past.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Past Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for past-dev, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: past-dev
provider_slug: past-dev
slug: past-dev-domain-security
source_filename: past-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: past.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 16:34:41 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: past.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/past-dev/security/past-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Memory
- API
- Platform
- Developer
---
