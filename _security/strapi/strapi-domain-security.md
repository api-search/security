---
api_specs:
- filename: strapi-rest-api-openapi.yml
  format: yaml
  label: Strapi REST API
  slug: strapi-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/strapi/refs/heads/main/openapi/strapi-rest-api-openapi.yml
- filename: strapi-admin-panel-api-openapi.yml
  format: yaml
  label: Strapi Admin Panel API
  slug: strapi-admin-panel-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/strapi/refs/heads/main/openapi/strapi-admin-panel-api-openapi.yml
- filename: strapi-users-and-permissions-api-openapi.yml
  format: yaml
  label: Strapi Users and Permissions API
  slug: strapi-users-permissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/strapi/refs/heads/main/openapi/strapi-users-and-permissions-api-openapi.yml
- filename: strapi-webhooks-asyncapi.yml
  format: yaml
  label: Strapi Webhooks
  slug: strapi-webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/strapi/refs/heads/main/asyncapi/strapi-webhooks-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: strapi.io
  spf: true
hosts:
- cert_expires: Nov  7 23:59:59 2026 GMT
  host: strapi.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  7 23:59:59 2026 GMT
  host: docs.strapi.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Strapi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Strapi, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Strapi
provider_slug: strapi
slug: strapi-domain-security
source_filename: strapi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: strapi.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  7 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.strapi.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  7 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: strapi.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/strapi/refs/heads/main/security/strapi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- CMS
- Content Management
- Headless CMS
- Node.js
- Open Source
---
