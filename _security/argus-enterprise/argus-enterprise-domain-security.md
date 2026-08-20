---
api_specs:
- filename: argus-enterprise-authentication-api-openapi.yml
  format: yaml
  label: ARGUS Enterprise Authentication API
  slug: argus-enterprise-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argus-enterprise/refs/heads/main/openapi/argus-enterprise-authentication-api-openapi.yml
- filename: argus-enterprise-cash-flows-api-openapi.yml
  format: yaml
  label: ARGUS Enterprise Cash Flows API
  slug: argus-enterprise-cash-flows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argus-enterprise/refs/heads/main/openapi/argus-enterprise-cash-flows-api-openapi.yml
- filename: argus-enterprise-events-api-openapi.yml
  format: yaml
  label: ARGUS Enterprise Events API
  slug: argus-enterprise-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argus-enterprise/refs/heads/main/openapi/argus-enterprise-events-api-openapi.yml
- filename: argus-enterprise-health-api-openapi.yml
  format: yaml
  label: ARGUS Enterprise Health API
  slug: argus-enterprise-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argus-enterprise/refs/heads/main/openapi/argus-enterprise-health-api-openapi.yml
- filename: argus-enterprise-leases-api-openapi.yml
  format: yaml
  label: ARGUS Enterprise Leases API
  slug: argus-enterprise-leases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argus-enterprise/refs/heads/main/openapi/argus-enterprise-leases-api-openapi.yml
- filename: argus-enterprise-portfolios-api-openapi.yml
  format: yaml
  label: ARGUS Enterprise Portfolios API
  slug: argus-enterprise-portfolios-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argus-enterprise/refs/heads/main/openapi/argus-enterprise-portfolios-api-openapi.yml
- filename: argus-enterprise-properties-api-openapi.yml
  format: yaml
  label: ARGUS Enterprise Properties API
  slug: argus-enterprise-properties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argus-enterprise/refs/heads/main/openapi/argus-enterprise-properties-api-openapi.yml
- filename: argus-enterprise-reports-api-openapi.yml
  format: yaml
  label: ARGUS Enterprise Reports API
  slug: argus-enterprise-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argus-enterprise/refs/heads/main/openapi/argus-enterprise-reports-api-openapi.yml
- filename: argus-enterprise-subscriptions-api-openapi.yml
  format: yaml
  label: ARGUS Enterprise Subscriptions API
  slug: argus-enterprise-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argus-enterprise/refs/heads/main/openapi/argus-enterprise-subscriptions-api-openapi.yml
- filename: argus-enterprise-tenants-api-openapi.yml
  format: yaml
  label: ARGUS Enterprise Tenants API
  slug: argus-enterprise-tenants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argus-enterprise/refs/heads/main/openapi/argus-enterprise-tenants-api-openapi.yml
- filename: argus-enterprise-users-api-openapi.yml
  format: yaml
  label: ARGUS Enterprise Users API
  slug: argus-enterprise-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argus-enterprise/refs/heads/main/openapi/argus-enterprise-users-api-openapi.yml
- filename: argus-enterprise-valuations-api-openapi.yml
  format: yaml
  label: ARGUS Enterprise Valuations API
  slug: argus-enterprise-valuations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argus-enterprise/refs/heads/main/openapi/argus-enterprise-valuations-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: altusgroup.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: altusplatform.com
  spf: false
hosts:
- cert_expires: Sep  1 17:18:54 2026 GMT
  host: www.altusgroup.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  1 17:18:54 2026 GMT
  host: cloud.altusplatform.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 05:35:04 2026 GMT
  host: api.argusenterprise.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Argus Enterprise Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ARGUS Enterprise, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: ARGUS Enterprise
provider_slug: argus-enterprise
slug: argus-enterprise-domain-security
source_filename: argus-enterprise-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.altusgroup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 17:18:54 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: cloud.altusplatform.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 17:18:54 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.argusenterprise.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 05:35:04 2026 GMT\n  hsts: null\ndomains:\n- domain: altusgroup.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: altusplatform.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/argus-enterprise/refs/heads/main/security/argus-enterprise-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Altus Group
- Asset Management
- Cash Flow Modeling
- Commercial Real Estate
- Portfolio-Management
- Valuation
---
