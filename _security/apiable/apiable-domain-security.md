---
api_specs:
- filename: apiable-companies-api-openapi.yml
  format: yaml
  label: Apiable Companies API
  slug: apiable-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apiable/refs/heads/main/openapi/apiable-companies-api-openapi.yml
- filename: apiable-custom-properties-api-openapi.yml
  format: yaml
  label: Apiable Custom Properties API
  slug: apiable-custom-properties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apiable/refs/heads/main/openapi/apiable-custom-properties-api-openapi.yml
- filename: apiable-docs-api-openapi.yml
  format: yaml
  label: Apiable Docs API
  slug: apiable-docs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apiable/refs/heads/main/openapi/apiable-docs-api-openapi.yml
- filename: apiable-files-api-openapi.yml
  format: yaml
  label: Apiable Files API
  slug: apiable-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apiable/refs/heads/main/openapi/apiable-files-api-openapi.yml
- filename: apiable-invitations-api-openapi.yml
  format: yaml
  label: Apiable Invitations API
  slug: apiable-invitations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apiable/refs/heads/main/openapi/apiable-invitations-api-openapi.yml
- filename: apiable-plans-api-openapi.yml
  format: yaml
  label: Apiable Plans API
  slug: apiable-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apiable/refs/heads/main/openapi/apiable-plans-api-openapi.yml
- filename: apiable-products-api-openapi.yml
  format: yaml
  label: Apiable Products API
  slug: apiable-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apiable/refs/heads/main/openapi/apiable-products-api-openapi.yml
- filename: apiable-subscriptions-api-openapi.yml
  format: yaml
  label: Apiable Subscriptions API
  slug: apiable-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apiable/refs/heads/main/openapi/apiable-subscriptions-api-openapi.yml
- filename: apiable-teams-api-openapi.yml
  format: yaml
  label: Apiable Teams API
  slug: apiable-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apiable/refs/heads/main/openapi/apiable-teams-api-openapi.yml
- filename: apiable-users-api-openapi.yml
  format: yaml
  label: Apiable Users API
  slug: apiable-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apiable/refs/heads/main/openapi/apiable-users-api-openapi.yml
- filename: apiable-webhooks-api-openapi.yml
  format: yaml
  label: Apiable Webhooks API
  slug: apiable-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apiable/refs/heads/main/openapi/apiable-webhooks-api-openapi.yml
- filename: apiable-server-info-api-openapi.yml
  format: yaml
  label: Apiable Server Info API
  slug: apiable-server-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apiable/refs/heads/main/openapi/apiable-server-info-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: apiable.io
  spf: true
hosts:
- cert_expires: Feb 12 23:59:59 2027 GMT
  host: www.apiable.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 16 23:59:59 2027 GMT
  host: developer.apiable.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Apiable Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Apiable, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Apiable
provider_slug: apiable
slug: apiable-domain-security
source_filename: apiable-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.apiable.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 12 23:59:59 2027 GMT\n  hsts: false\n- host: developer.apiable.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 16 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: apiable.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apiable/refs/heads/main/security/apiable-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Amazon API Gateway
- API Gateway
- API Monetization
- API Portal
- Developer Experience
- Developer Portal
- Developer Tools
- Kong
- Platform
- Self-Service
---
