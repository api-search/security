---
api_specs:
- filename: arcadia-auth-api-openapi.yml
  format: yaml
  label: Arcadia Auth API
  slug: arcadia-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcadia/refs/heads/main/openapi/arcadia-auth-api-openapi.yml
- filename: arcadia-bundle-beta-api-openapi.yml
  format: yaml
  label: Arcadia Bundle (Beta) API
  slug: arcadia-bundle-beta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcadia/refs/heads/main/openapi/arcadia-bundle-beta-api-openapi.yml
- filename: arcadia-plug-api-openapi.yml
  format: yaml
  label: Arcadia Plug API
  slug: arcadia-plug-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcadia/refs/heads/main/openapi/arcadia-plug-api-openapi.yml
- filename: arcadia-spark-api-openapi.yml
  format: yaml
  label: Arcadia Spark API
  slug: arcadia-spark-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcadia/refs/heads/main/openapi/arcadia-spark-api-openapi.yml
- filename: arcadia-users-api-openapi.yml
  format: yaml
  label: Arcadia Users API
  slug: arcadia-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcadia/refs/heads/main/openapi/arcadia-users-api-openapi.yml
- filename: arcadia-utility-accounts-api-openapi.yml
  format: yaml
  label: Arcadia Utility Accounts API
  slug: arcadia-utility-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcadia/refs/heads/main/openapi/arcadia-utility-accounts-api-openapi.yml
- filename: arcadia-utility-credentials-api-openapi.yml
  format: yaml
  label: Arcadia Utility Credentials API
  slug: arcadia-utility-credentials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcadia/refs/heads/main/openapi/arcadia-utility-credentials-api-openapi.yml
- filename: arcadia-utility-meters-beta-api-openapi.yml
  format: yaml
  label: Arcadia Utility Meters (Beta) API
  slug: arcadia-utility-meters-beta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcadia/refs/heads/main/openapi/arcadia-utility-meters-beta-api-openapi.yml
- filename: arcadia-webhooks-api-openapi.yml
  format: yaml
  label: Arcadia Webhooks API
  slug: arcadia-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcadia/refs/heads/main/openapi/arcadia-webhooks-api-openapi.yml
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
kind: domain-security
layout: security
method: probed
name: Arcadia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Arcadia, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Arcadia
provider_slug: arcadia
slug: arcadia-domain-security
source_filename: arcadia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.arcadia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 22:05:19 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.arcadia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 03:20:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.arcadia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: arcadia.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/arcadia/refs/heads/main/security/arcadia-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Energy
- Utilities
- Clean Energy
- Billing Data
- Interval Data
- Carbon
- Solar
- Tariff
---
