---
api_specs:
- filename: abm-dev-campaigns-api-openapi.yml
  format: yaml
  label: abm-dev Campaigns API
  slug: abm-dev-campaigns-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/abm-dev/openapi/abm-dev-campaigns-api-openapi.yml
- filename: abm-dev-crm-api-openapi.yml
  format: yaml
  label: abm-dev CRM API
  slug: abm-dev-crm-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/abm-dev/openapi/abm-dev-crm-api-openapi.yml
- filename: abm-dev-enrichment-api-openapi.yml
  format: yaml
  label: abm-dev Enrichment API
  slug: abm-dev-enrichment-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/abm-dev/openapi/abm-dev-enrichment-api-openapi.yml
- filename: abm-dev-enrichment-config-api-openapi.yml
  format: yaml
  label: abm-dev Enrichment Config API
  slug: abm-dev-enrichment-config-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/abm-dev/openapi/abm-dev-enrichment-config-api-openapi.yml
- filename: abm-dev-field-configuration-api-openapi.yml
  format: yaml
  label: abm-dev Field Configuration API
  slug: abm-dev-field-configuration-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/abm-dev/openapi/abm-dev-field-configuration-api-openapi.yml
- filename: abm-dev-health-api-openapi.yml
  format: yaml
  label: abm-dev Health API
  slug: abm-dev-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/abm-dev/openapi/abm-dev-health-api-openapi.yml
- filename: abm-dev-organization-api-openapi.yml
  format: yaml
  label: abm-dev Organization API
  slug: abm-dev-organization-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/abm-dev/openapi/abm-dev-organization-api-openapi.yml
- filename: abm-dev-people-finder-api-openapi.yml
  format: yaml
  label: abm-dev People Finder API
  slug: abm-dev-people-finder-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/abm-dev/openapi/abm-dev-people-finder-api-openapi.yml
- filename: abm-dev-webhooks-api-openapi.yml
  format: yaml
  label: abm-dev Webhooks API
  slug: abm-dev-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/abm-dev/openapi/abm-dev-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: abm.dev
  spf: true
hosts:
- cert_expires: Jan 25 14:27:42 2027 GMT
  host: abm.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Abm Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for abm-dev, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: abm-dev
provider_slug: abm-dev
slug: abm-dev-domain-security
source_filename: abm-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: abm.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 25 14:27:42 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: abm.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/abm-dev/security/abm-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Account-Based Marketing
- AI Agents
- Data Enrichment
- B2B
- Marketing API
---
