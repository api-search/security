---
api_specs:
- filename: swaggerhub-registry-api-openapi.yml
  format: yaml
  label: SwaggerHub Registry API
  slug: swaggerhub-registry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swaggerhub/refs/heads/main/openapi/swaggerhub-registry-api-openapi.yml
- filename: swaggerhub-user-management-openapi.yml
  format: yaml
  label: SwaggerHub User Management API
  slug: swaggerhub-user-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swaggerhub/refs/heads/main/openapi/swaggerhub-user-management-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: swagger.io
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: smartbear.com
  spf: true
hosts:
- cert_expires: Oct  4 16:46:01 2026 GMT
  host: swagger.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 15:02:27 2026 GMT
  host: support.smartbear.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 14 23:59:59 2026 GMT
  host: api.swaggerhub.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Swaggerhub Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SwaggerHub, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: SwaggerHub
provider_slug: swaggerhub
slug: swaggerhub-domain-security
source_filename: swaggerhub-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: swagger.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 16:46:01 2026 GMT\n  hsts: false\n- host: support.smartbear.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 15:02:27 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.swaggerhub.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 14 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: swagger.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: smartbear.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/swaggerhub/refs/heads/main/security/swaggerhub-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- API Design
- API Management
- API Registry
- Documentation
- OpenAPI
- SmartBear
---
