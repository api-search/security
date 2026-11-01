---
api_specs:
- filename: groundmail-dev-automations-api-openapi.yml
  format: yaml
  label: groundmail-dev Automations API
  slug: groundmail-dev-automations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/groundmail-dev/openapi/groundmail-dev-automations-api-openapi.yml
- filename: groundmail-dev-deliverability-api-openapi.yml
  format: yaml
  label: groundmail-dev Deliverability API
  slug: groundmail-dev-deliverability-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/groundmail-dev/openapi/groundmail-dev-deliverability-api-openapi.yml
- filename: groundmail-dev-dmarc-api-openapi.yml
  format: yaml
  label: groundmail-dev Dmarc API
  slug: groundmail-dev-dmarc-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/groundmail-dev/openapi/groundmail-dev-dmarc-api-openapi.yml
- filename: groundmail-dev-domains-api-openapi.yml
  format: yaml
  label: groundmail-dev Domains API
  slug: groundmail-dev-domains-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/groundmail-dev/openapi/groundmail-dev-domains-api-openapi.yml
- filename: groundmail-dev-emails-api-openapi.yml
  format: yaml
  label: groundmail-dev Emails API
  slug: groundmail-dev-emails-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/groundmail-dev/openapi/groundmail-dev-emails-api-openapi.yml
- filename: groundmail-dev-events-api-openapi.yml
  format: yaml
  label: groundmail-dev Events API
  slug: groundmail-dev-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/groundmail-dev/openapi/groundmail-dev-events-api-openapi.yml
- filename: groundmail-dev-inbound-api-openapi.yml
  format: yaml
  label: groundmail-dev Inbound API
  slug: groundmail-dev-inbound-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/groundmail-dev/openapi/groundmail-dev-inbound-api-openapi.yml
- filename: groundmail-dev-integrations-api-openapi.yml
  format: yaml
  label: groundmail-dev Integrations API
  slug: groundmail-dev-integrations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/groundmail-dev/openapi/groundmail-dev-integrations-api-openapi.yml
- filename: groundmail-dev-migrations-api-openapi.yml
  format: yaml
  label: groundmail-dev Migrations API
  slug: groundmail-dev-migrations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/groundmail-dev/openapi/groundmail-dev-migrations-api-openapi.yml
- filename: groundmail-dev-oauth-api-openapi.yml
  format: yaml
  label: groundmail-dev OAuth API
  slug: groundmail-dev-oauth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/groundmail-dev/openapi/groundmail-dev-oauth-api-openapi.yml
- filename: groundmail-dev-smtpcredentials-api-openapi.yml
  format: yaml
  label: groundmail-dev Smtp Credentials API
  slug: groundmail-dev-smtpcredentials-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/groundmail-dev/openapi/groundmail-dev-smtpcredentials-api-openapi.yml
- filename: groundmail-dev-suppressions-api-openapi.yml
  format: yaml
  label: groundmail-dev Suppressions API
  slug: groundmail-dev-suppressions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/groundmail-dev/openapi/groundmail-dev-suppressions-api-openapi.yml
- filename: groundmail-dev-templates-api-openapi.yml
  format: yaml
  label: groundmail-dev Templates API
  slug: groundmail-dev-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/groundmail-dev/openapi/groundmail-dev-templates-api-openapi.yml
- filename: groundmail-dev-tenants-api-openapi.yml
  format: yaml
  label: groundmail-dev Tenants API
  slug: groundmail-dev-tenants-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/groundmail-dev/openapi/groundmail-dev-tenants-api-openapi.yml
- filename: groundmail-dev-test-inbox-api-openapi.yml
  format: yaml
  label: groundmail-dev Test inbox API
  slug: groundmail-dev-test-inbox-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/groundmail-dev/openapi/groundmail-dev-test-inbox-api-openapi.yml
- filename: groundmail-dev-validation-api-openapi.yml
  format: yaml
  label: groundmail-dev Validation API
  slug: groundmail-dev-validation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/groundmail-dev/openapi/groundmail-dev-validation-api-openapi.yml
- filename: groundmail-dev-webhooks-api-openapi.yml
  format: yaml
  label: groundmail-dev Webhooks API
  slug: groundmail-dev-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/groundmail-dev/openapi/groundmail-dev-webhooks-api-openapi.yml
- filename: groundmail-dev-api-keys-api-openapi.yml
  format: yaml
  label: groundmail-dev API Keys API
  slug: groundmail-dev-api-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/groundmail-dev/openapi/groundmail-dev-api-keys-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: groundmail.dev
  spf: true
hosts:
- cert_expires: Jan 18 03:45:12 2027 GMT
  host: groundmail.dev
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Groundmail Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for groundmail-dev, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: groundmail-dev
provider_slug: groundmail-dev
slug: groundmail-dev-domain-security
source_filename: groundmail-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: groundmail.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 18 03:45:12 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: groundmail.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/groundmail-dev/security/groundmail-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Email
- API
- Transactional
- SMTP
- Developer
---
