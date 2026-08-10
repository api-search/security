---
api_specs:
- filename: arccos-golf-clubs-api-openapi.yml
  format: yaml
  label: Arccos Golf Clubs API
  slug: arccos-golf-clubs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arccos-golf/refs/heads/main/openapi/arccos-golf-clubs-api-openapi.yml
- filename: arccos-golf-courses-api-openapi.yml
  format: yaml
  label: Arccos Golf Courses API
  slug: arccos-golf-courses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arccos-golf/refs/heads/main/openapi/arccos-golf-courses-api-openapi.yml
- filename: arccos-golf-rounds-api-openapi.yml
  format: yaml
  label: Arccos Golf Rounds API
  slug: arccos-golf-rounds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arccos-golf/refs/heads/main/openapi/arccos-golf-rounds-api-openapi.yml
- filename: arccos-golf-users-api-openapi.yml
  format: yaml
  label: Arccos Golf Users API
  slug: arccos-golf-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arccos-golf/refs/heads/main/openapi/arccos-golf-users-api-openapi.yml
- filename: arccos-golf-webhooks-api-openapi.yml
  format: yaml
  label: Arccos Golf Webhooks API
  slug: arccos-golf-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arccos-golf/refs/heads/main/openapi/arccos-golf-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: arccosgolf.com
  spf: true
hosts:
- cert_expires: Oct 22 12:05:32 2026 GMT
  host: www.arccosgolf.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 27 23:59:59 2027 GMT
  host: api.arccosgolf.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Arccos Golf Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Arccos Golf, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Arccos Golf
provider_slug: arccos-golf
slug: arccos-golf-domain-security
source_filename: arccos-golf-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.arccosgolf.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 12:05:32 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\n- host: api.arccosgolf.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 27 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: arccosgolf.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/arccos-golf/refs/heads/main/security/arccos-golf-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- golf
- sports-technology
- wearables
- iot
- shot-tracking
- sports-analytics
- performance-analytics
- geospatial
- consumer-hardware
- webhooks
- oauth2
- mcp
- ecommerce
---
