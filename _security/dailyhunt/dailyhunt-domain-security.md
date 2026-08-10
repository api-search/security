---
api_specs:
- filename: dailyhunt-catalog-api-openapi.yml
  format: yaml
  label: Dailyhunt Catalog API
  slug: dailyhunt-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dailyhunt/refs/heads/main/openapi/dailyhunt-catalog-api-openapi.yml
- filename: dailyhunt-channels-api-openapi.yml
  format: yaml
  label: Dailyhunt Channels API
  slug: dailyhunt-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dailyhunt/refs/heads/main/openapi/dailyhunt-channels-api-openapi.yml
- filename: dailyhunt-content-fetch-api-openapi.yml
  format: yaml
  label: Dailyhunt Content Fetch API
  slug: dailyhunt-content-fetch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dailyhunt/refs/heads/main/openapi/dailyhunt-content-fetch-api-openapi.yml
- filename: dailyhunt-cricket-api-openapi.yml
  format: yaml
  label: Dailyhunt Cricket API
  slug: dailyhunt-cricket-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dailyhunt/refs/heads/main/openapi/dailyhunt-cricket-api-openapi.yml
- filename: dailyhunt-feedback-api-openapi.yml
  format: yaml
  label: Dailyhunt Feedback API
  slug: dailyhunt-feedback-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dailyhunt/refs/heads/main/openapi/dailyhunt-feedback-api-openapi.yml
- filename: dailyhunt-languages-api-openapi.yml
  format: yaml
  label: Dailyhunt Languages API
  slug: dailyhunt-languages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dailyhunt/refs/heads/main/openapi/dailyhunt-languages-api-openapi.yml
- filename: dailyhunt-products-api-openapi.yml
  format: yaml
  label: Dailyhunt Products API
  slug: dailyhunt-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dailyhunt/refs/heads/main/openapi/dailyhunt-products-api-openapi.yml
- filename: dailyhunt-tracking-api-openapi.yml
  format: yaml
  label: Dailyhunt Tracking API
  slug: dailyhunt-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dailyhunt/refs/heads/main/openapi/dailyhunt-tracking-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: dailyhunt.in
  spf: true
hosts:
- cert_expires: Nov 18 23:59:59 2026 GMT
  host: www.dailyhunt.in
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 07:22:19 2026 GMT
  host: api-syndication.dailyhunt.in
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: feed.dailyhunt.in
  https: false
kind: domain-security
layout: security
method: probed
name: Dailyhunt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dailyhunt, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Dailyhunt
provider_slug: dailyhunt
slug: dailyhunt-domain-security
source_filename: dailyhunt-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dailyhunt.in\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 18 23:59:59 2026 GMT\n  hsts: null\n- host: api-syndication.dailyhunt.in\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 07:22:19 2026 GMT\n  hsts: null\n- host: feed.dailyhunt.in\n  https: false\ndomains:\n- domain: dailyhunt.in\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dailyhunt/refs/heads/main/security/dailyhunt-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- News
- Media
- Content Syndication
- Content
- Advertising
- Video
- Localization
- India
- Mobile
---
