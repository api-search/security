---
api_specs:
- filename: atvenu-atvenu-api-api-openapi.yml
  format: yaml
  label: atVenu AtVenu API
  slug: atvenu-atvenu-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atvenu/refs/heads/main/openapi/atvenu-atvenu-api-api-openapi.yml
- filename: atvenu-download-api-openapi.yml
  format: yaml
  label: atVenu Download API
  slug: atvenu-download-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atvenu/refs/heads/main/openapi/atvenu-download-api-openapi.yml
- filename: atvenu-downloads-api-openapi.yml
  format: yaml
  label: atVenu Downloads API
  slug: atvenu-downloads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atvenu/refs/heads/main/openapi/atvenu-downloads-api-openapi.yml
- filename: atvenu-help-center-api-openapi.yml
  format: yaml
  label: atVenu Help Center API
  slug: atvenu-help-center-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atvenu/refs/heads/main/openapi/atvenu-help-center-api-openapi.yml
- filename: atvenu-incidents-api-openapi.yml
  format: yaml
  label: atVenu Incidents API
  slug: atvenu-incidents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atvenu/refs/heads/main/openapi/atvenu-incidents-api-openapi.yml
- filename: atvenu-incremental-api-openapi.yml
  format: yaml
  label: atVenu Incremental API
  slug: atvenu-incremental-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atvenu/refs/heads/main/openapi/atvenu-incremental-api-openapi.yml
- filename: atvenu-register-api-openapi.yml
  format: yaml
  label: atVenu Register API
  slug: atvenu-register-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atvenu/refs/heads/main/openapi/atvenu-register-api-openapi.yml
- filename: atvenu-services-api-openapi.yml
  format: yaml
  label: atVenu Services API
  slug: atvenu-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atvenu/refs/heads/main/openapi/atvenu-services-api-openapi.yml
- filename: atvenu-sunshine-api-openapi.yml
  format: yaml
  label: atVenu Sunshine API
  slug: atvenu-sunshine-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atvenu/refs/heads/main/openapi/atvenu-sunshine-api-openapi.yml
- filename: atvenu-tickets-api-openapi.yml
  format: yaml
  label: atVenu Tickets API
  slug: atvenu-tickets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atvenu/refs/heads/main/openapi/atvenu-tickets-api-openapi.yml
- filename: atvenu-user-profiles-api-openapi.yml
  format: yaml
  label: atVenu User Profiles API
  slug: atvenu-user-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atvenu/refs/heads/main/openapi/atvenu-user-profiles-api-openapi.yml
- filename: atvenu-users-api-openapi.yml
  format: yaml
  label: atVenu Users API
  slug: atvenu-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atvenu/refs/heads/main/openapi/atvenu-users-api-openapi.yml
- filename: atvenu-webhooks-api-openapi.yml
  format: yaml
  label: atVenu Webhooks API
  slug: atvenu-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atvenu/refs/heads/main/openapi/atvenu-webhooks-api-openapi.yml
- filename: atvenu-webstore-api-openapi.yml
  format: yaml
  label: atVenu Webstore API
  slug: atvenu-webstore-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atvenu/refs/heads/main/openapi/atvenu-webstore-api-openapi.yml
- filename: atvenu-graph-ql-api-openapi.yml
  format: yaml
  label: atVenu Graph QL API
  slug: atvenu-graph-ql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atvenu/refs/heads/main/openapi/atvenu-graph-ql-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: atvenu.com
  spf: true
hosts:
- cert_expires: Dec 13 00:40:48 2026 GMT
  host: www.atvenu.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Atvenu Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for atVenu, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: atVenu
provider_slug: atvenu
slug: atvenu-domain-security
source_filename: atvenu-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.atvenu.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 00:40:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: atvenu.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/atvenu/refs/heads/main/security/atvenu-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Payments
- Live Events
- Commerce
- Point-of-Sale
---
