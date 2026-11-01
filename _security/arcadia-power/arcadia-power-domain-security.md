---
api_specs:
- filename: arcadia-power-accounts-api-openapi.yml
  format: yaml
  label: Arcadia Accounts API
  slug: arcadia-power-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcadia-power/openapi/arcadia-power-accounts-api-openapi.yml
- filename: arcadia-power-credentials-api-openapi.yml
  format: yaml
  label: Arcadia Credentials API
  slug: arcadia-power-credentials-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcadia-power/openapi/arcadia-power-credentials-api-openapi.yml
- filename: arcadia-power-files-api-openapi.yml
  format: yaml
  label: Arcadia Files API
  slug: arcadia-power-files-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcadia-power/openapi/arcadia-power-files-api-openapi.yml
- filename: arcadia-power-intervals-api-openapi.yml
  format: yaml
  label: Arcadia Intervals API
  slug: arcadia-power-intervals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcadia-power/openapi/arcadia-power-intervals-api-openapi.yml
- filename: arcadia-power-meters-api-openapi.yml
  format: yaml
  label: Arcadia Meters API
  slug: arcadia-power-meters-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcadia-power/openapi/arcadia-power-meters-api-openapi.yml
- filename: arcadia-power-providers-api-openapi.yml
  format: yaml
  label: Arcadia Providers API
  slug: arcadia-power-providers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcadia-power/openapi/arcadia-power-providers-api-openapi.yml
- filename: arcadia-power-sites-api-openapi.yml
  format: yaml
  label: Arcadia Sites API
  slug: arcadia-power-sites-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcadia-power/openapi/arcadia-power-sites-api-openapi.yml
- filename: arcadia-power-statements-api-openapi.yml
  format: yaml
  label: Arcadia Statements API
  slug: arcadia-power-statements-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcadia-power/openapi/arcadia-power-statements-api-openapi.yml
- filename: arcadia-power-webhooks-api-openapi.yml
  format: yaml
  label: Arcadia Webhooks API
  slug: arcadia-power-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcadia-power/openapi/arcadia-power-webhooks-api-openapi.yml
- filename: arcadia-power-api-keys-api-openapi.yml
  format: yaml
  label: Arcadia API Keys API
  slug: arcadia-power-api-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcadia-power/openapi/arcadia-power-api-keys-api-openapi.yml
- filename: arcadia-power-authentication-api-openapi.yml
  format: yaml
  label: Arcadia Authentication API
  slug: arcadia-power-authentication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcadia-power/openapi/arcadia-power-authentication-api-openapi.yml
- filename: arcadia-power-business-units-api-openapi.yml
  format: yaml
  label: Arcadia Business Units API
  slug: arcadia-power-business-units-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcadia-power/openapi/arcadia-power-business-units-api-openapi.yml
- filename: arcadia-power-custom-data-api-openapi.yml
  format: yaml
  label: Arcadia Custom Data API
  slug: arcadia-power-custom-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcadia-power/openapi/arcadia-power-custom-data-api-openapi.yml
- filename: arcadia-power-deletion-api-openapi.yml
  format: yaml
  label: Arcadia Deletion API
  slug: arcadia-power-deletion-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcadia-power/openapi/arcadia-power-deletion-api-openapi.yml
- filename: arcadia-power-discovered-statements-api-openapi.yml
  format: yaml
  label: Arcadia Discovered Statements API
  slug: arcadia-power-discovered-statements-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcadia-power/openapi/arcadia-power-discovered-statements-api-openapi.yml
- filename: arcadia-power-downloads-api-openapi.yml
  format: yaml
  label: Arcadia Downloads API
  slug: arcadia-power-downloads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcadia-power/openapi/arcadia-power-downloads-api-openapi.yml
- filename: arcadia-power-expected-accounts-api-openapi.yml
  format: yaml
  label: Arcadia Expected Accounts API
  slug: arcadia-power-expected-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcadia-power/openapi/arcadia-power-expected-accounts-api-openapi.yml
- filename: arcadia-power-sandbox-statements-api-openapi.yml
  format: yaml
  label: Arcadia Sandbox Statements API
  slug: arcadia-power-sandbox-statements-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcadia-power/openapi/arcadia-power-sandbox-statements-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: arcadia.com
  spf: true
hosts:
- cert_expires: Sep 23 22:05:19 2026 GMT
  host: www.arcadia.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  2 03:20:02 2026 GMT
  host: docs.arcadia.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  4 23:59:59 2026 GMT
  host: api.arcadia.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Arcadia Power Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Arcadia, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Arcadia
provider_slug: arcadia-power
slug: arcadia-power-domain-security
source_filename: arcadia-power-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.arcadia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 22:05:19 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.arcadia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 03:20:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.arcadia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: arcadia.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/arcadia-power/security/arcadia-power-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Energy
- Clean Energy
- Utility Data
- Climate
- Sustainability
- Carbon Accounting
- Solar
- Storage
- EV Charging
- Decarbonization
- Energy Intelligence
- Utilities
---
