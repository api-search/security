---
api_specs:
- filename: sharethis-ai-summary-api-openapi.yml
  format: yaml
  label: ShareThis AI Summary API
  slug: sharethis-ai-summary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sharethis/refs/heads/main/openapi/sharethis-ai-summary-api-openapi.yml
- filename: sharethis-apps-api-openapi.yml
  format: yaml
  label: ShareThis Apps API
  slug: sharethis-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sharethis/refs/heads/main/openapi/sharethis-apps-api-openapi.yml
- filename: sharethis-audience-api-openapi.yml
  format: yaml
  label: ShareThis Audience API
  slug: sharethis-audience-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sharethis/refs/heads/main/openapi/sharethis-audience-api-openapi.yml
- filename: sharethis-authentication-api-openapi.yml
  format: yaml
  label: ShareThis Authentication API
  slug: sharethis-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sharethis/refs/heads/main/openapi/sharethis-authentication-api-openapi.yml
- filename: sharethis-oauth-clients-api-openapi.yml
  format: yaml
  label: ShareThis OAuth Clients API
  slug: sharethis-oauth-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sharethis/refs/heads/main/openapi/sharethis-oauth-clients-api-openapi.yml
- filename: sharethis-properties-api-openapi.yml
  format: yaml
  label: ShareThis Properties API
  slug: sharethis-properties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sharethis/refs/heads/main/openapi/sharethis-properties-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: sharethis.com
  spf: true
hosts:
- cert_expires: Mar 17 23:59:59 2027 GMT
  host: sharethis.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 17 23:59:59 2027 GMT
  host: platform-api.sharethis.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 10 23:59:59 2026 GMT
  host: count-server.sharethis.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sharethis Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ShareThis, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: ShareThis
provider_slug: sharethis
slug: sharethis-domain-security
source_filename: sharethis-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sharethis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 17 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: platform-api.sharethis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 17 23:59:59 2027 GMT\n  hsts: null\n- host: count-server.sharethis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: sharethis.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sharethis/refs/heads/main/security/sharethis-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Social Sharing
- Website Tools
- Audience Data
- Advertising Technology
- Analytics
- Consent Management
- Publishing
- Model Context Protocol
---
