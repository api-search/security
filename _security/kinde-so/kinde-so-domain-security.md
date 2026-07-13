---
api_specs:
- filename: kinde-so-openapi.yml
  format: yaml
  label: Kinde Users API
  slug: kinde-so-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kinde-so/refs/heads/main/openapi/kinde-so-openapi.yml
- filename: kinde-so-openapi.yml
  format: yaml
  label: Kinde Organizations API
  slug: kinde-so-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kinde-so/refs/heads/main/openapi/kinde-so-openapi.yml
- filename: kinde-so-openapi.yml
  format: yaml
  label: Kinde Roles API
  slug: kinde-so-roles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kinde-so/refs/heads/main/openapi/kinde-so-openapi.yml
- filename: kinde-so-openapi.yml
  format: yaml
  label: Kinde Permissions API
  slug: kinde-so-permissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kinde-so/refs/heads/main/openapi/kinde-so-openapi.yml
- filename: kinde-so-openapi.yml
  format: yaml
  label: Kinde Feature Flags API
  slug: kinde-so-feature-flags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kinde-so/refs/heads/main/openapi/kinde-so-openapi.yml
- filename: kinde-so-openapi.yml
  format: yaml
  label: Kinde Applications API
  slug: kinde-so-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kinde-so/refs/heads/main/openapi/kinde-so-openapi.yml
- filename: kinde-so-openapi.yml
  format: yaml
  label: Kinde Connections API
  slug: kinde-so-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kinde-so/refs/heads/main/openapi/kinde-so-openapi.yml
- filename: kinde-so-openapi.yml
  format: yaml
  label: Kinde APIs and Scopes API
  slug: kinde-so-apis-scopes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kinde-so/refs/heads/main/openapi/kinde-so-openapi.yml
- filename: kinde-so-openapi.yml
  format: yaml
  label: Kinde Subscribers API
  slug: kinde-so-subscribers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kinde-so/refs/heads/main/openapi/kinde-so-openapi.yml
- filename: kinde-so-openapi.yml
  format: yaml
  label: Kinde Business API
  slug: kinde-so-business-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kinde-so/refs/heads/main/openapi/kinde-so-openapi.yml
- filename: kinde-so-openapi.yml
  format: yaml
  label: Kinde Properties API
  slug: kinde-so-properties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kinde-so/refs/heads/main/openapi/kinde-so-openapi.yml
- filename: kinde-so-openapi.yml
  format: yaml
  label: Kinde Webhooks API
  slug: kinde-so-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kinde-so/refs/heads/main/openapi/kinde-so-openapi.yml
- filename: kinde-so-openapi.yml
  format: yaml
  label: Kinde Billing API
  slug: kinde-so-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kinde-so/refs/heads/main/openapi/kinde-so-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: kinde.com
  spf: true
hosts:
- cert_expires: Oct  9 23:59:59 2026 GMT
  host: kinde.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 30 23:59:59 2026 GMT
  host: docs.kinde.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kinde So Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kinde, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Kinde
provider_slug: kinde-so
slug: kinde-so-domain-security
source_filename: kinde-so-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kinde.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.kinde.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 30 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: kinde.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kinde-so/refs/heads/main/security/kinde-so-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Authentication
- User Management
- Identity
- Authorization
- SaaS
- CIAM
---
