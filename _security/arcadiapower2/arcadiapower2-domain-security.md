---
api_specs:
- filename: arcadiapower2-auth-api-openapi.yml
  format: yaml
  label: Arcadiapower2 Auth API
  slug: arcadiapower2-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcadiapower2/refs/heads/main/openapi/arcadiapower2-auth-api-openapi.yml
- filename: arcadiapower2-bundle-beta-api-openapi.yml
  format: yaml
  label: Arcadiapower2 Bundle (Beta) API
  slug: arcadiapower2-bundle-beta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcadiapower2/refs/heads/main/openapi/arcadiapower2-bundle-beta-api-openapi.yml
- filename: arcadiapower2-bundle-webhook-events-api-openapi.yml
  format: yaml
  label: Arcadiapower2 Bundle Webhook Events API
  slug: arcadiapower2-bundle-webhook-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcadiapower2/refs/heads/main/openapi/arcadiapower2-bundle-webhook-events-api-openapi.yml
- filename: arcadiapower2-plug-api-openapi.yml
  format: yaml
  label: Arcadiapower2 Plug API
  slug: arcadiapower2-plug-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcadiapower2/refs/heads/main/openapi/arcadiapower2-plug-api-openapi.yml
- filename: arcadiapower2-spark-api-openapi.yml
  format: yaml
  label: Arcadiapower2 Spark API
  slug: arcadiapower2-spark-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcadiapower2/refs/heads/main/openapi/arcadiapower2-spark-api-openapi.yml
- filename: arcadiapower2-users-api-openapi.yml
  format: yaml
  label: Arcadiapower2 Users API
  slug: arcadiapower2-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcadiapower2/refs/heads/main/openapi/arcadiapower2-users-api-openapi.yml
- filename: arcadiapower2-utility-accounts-api-openapi.yml
  format: yaml
  label: Arcadiapower2 Utility Accounts API
  slug: arcadiapower2-utility-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcadiapower2/refs/heads/main/openapi/arcadiapower2-utility-accounts-api-openapi.yml
- filename: arcadiapower2-utility-credentials-api-openapi.yml
  format: yaml
  label: Arcadiapower2 Utility Credentials API
  slug: arcadiapower2-utility-credentials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcadiapower2/refs/heads/main/openapi/arcadiapower2-utility-credentials-api-openapi.yml
- filename: arcadiapower2-utility-meters-beta-api-openapi.yml
  format: yaml
  label: Arcadiapower2 Utility Meters (Beta) API
  slug: arcadiapower2-utility-meters-beta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcadiapower2/refs/heads/main/openapi/arcadiapower2-utility-meters-beta-api-openapi.yml
- filename: arcadiapower2-webhook-events-api-openapi.yml
  format: yaml
  label: Arcadiapower2 Webhook Events API
  slug: arcadiapower2-webhook-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcadiapower2/refs/heads/main/openapi/arcadiapower2-webhook-events-api-openapi.yml
- filename: arcadiapower2-webhooks-api-openapi.yml
  format: yaml
  label: Arcadiapower2 Webhooks API
  slug: arcadiapower2-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcadiapower2/refs/heads/main/openapi/arcadiapower2-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: arcadia.com
  spf: true
hosts:
- cert_expires: Nov 22 21:08:20 2026 GMT
  host: www.arcadia.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Arcadiapower2 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Arcadiapower2, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Arcadiapower2
provider_slug: arcadiapower2
slug: arcadiapower2-domain-security
source_filename: arcadiapower2-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.arcadia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 22 21:08:20 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: arcadia.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/arcadiapower2/refs/heads/main/security/arcadiapower2-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Energy
- SaaS
- Enterprise
- Sustainability
- Data
---
