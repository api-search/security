---
api_specs:
- filename: listmonk-bounces-api-openapi.yml
  format: yaml
  label: listmonk Bounces API
  slug: listmonk-bounces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/listmonk/refs/heads/main/openapi/listmonk-bounces-api-openapi.yml
- filename: listmonk-campaigns-api-openapi.yml
  format: yaml
  label: listmonk Campaigns API
  slug: listmonk-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/listmonk/refs/heads/main/openapi/listmonk-campaigns-api-openapi.yml
- filename: listmonk-import-api-openapi.yml
  format: yaml
  label: listmonk Import API
  slug: listmonk-import-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/listmonk/refs/heads/main/openapi/listmonk-import-api-openapi.yml
- filename: listmonk-lists-api-openapi.yml
  format: yaml
  label: listmonk Lists API
  slug: listmonk-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/listmonk/refs/heads/main/openapi/listmonk-lists-api-openapi.yml
- filename: listmonk-media-api-openapi.yml
  format: yaml
  label: listmonk Media API
  slug: listmonk-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/listmonk/refs/heads/main/openapi/listmonk-media-api-openapi.yml
- filename: listmonk-subscribers-api-openapi.yml
  format: yaml
  label: listmonk Subscribers API
  slug: listmonk-subscribers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/listmonk/refs/heads/main/openapi/listmonk-subscribers-api-openapi.yml
- filename: listmonk-templates-api-openapi.yml
  format: yaml
  label: listmonk Templates API
  slug: listmonk-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/listmonk/refs/heads/main/openapi/listmonk-templates-api-openapi.yml
- filename: listmonk-transactional-api-openapi.yml
  format: yaml
  label: listmonk Transactional API
  slug: listmonk-transactional-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/listmonk/refs/heads/main/openapi/listmonk-transactional-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: listmonk.app
  spf: false
hosts:
- cert_expires: Sep 25 15:01:18 2026 GMT
  host: listmonk.app
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Listmonk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for listmonk, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: listmonk
provider_slug: listmonk
slug: listmonk-domain-security
source_filename: listmonk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: listmonk.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 15:01:18 2026 GMT\n  hsts: false\ndomains:\n- domain: listmonk.app\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/listmonk/refs/heads/main/security/listmonk-domain-security.yml
summary_line: TLSv1.3
tags:
- Email
- Newsletter
- Mailing List
- Marketing
- Transactional Email
- Campaigns
- Subscribers
- Bounce Handling
- Open Source
- Self-Hosted
- Go
- PostgreSQL
---
