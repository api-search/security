---
api_specs:
- filename: shortkit-ad-configuration-api-openapi.yml
  format: yaml
  label: ShortKit Ad Configuration API
  slug: shortkit-ad-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shortkit/refs/heads/main/openapi/shortkit-ad-configuration-api-openapi.yml
- filename: shortkit-analytics-api-openapi.yml
  format: yaml
  label: ShortKit Analytics API
  slug: shortkit-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shortkit/refs/heads/main/openapi/shortkit-analytics-api-openapi.yml
- filename: shortkit-content-api-openapi.yml
  format: yaml
  label: ShortKit Content API
  slug: shortkit-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shortkit/refs/heads/main/openapi/shortkit-content-api-openapi.yml
- filename: shortkit-live-streams-api-openapi.yml
  format: yaml
  label: ShortKit Live Streams API
  slug: shortkit-live-streams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shortkit/refs/heads/main/openapi/shortkit-live-streams-api-openapi.yml
- filename: shortkit-surveys-api-openapi.yml
  format: yaml
  label: ShortKit Surveys API
  slug: shortkit-surveys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shortkit/refs/heads/main/openapi/shortkit-surveys-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: shortkit.dev
  spf: true
hosts:
- cert_expires: Sep 21 06:06:57 2026 GMT
  host: www.shortkit.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 06:06:57 2026 GMT
  host: api.shortkit.dev
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Shortkit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ShortKit, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: ShortKit
provider_slug: shortkit
slug: shortkit-domain-security
source_filename: shortkit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.shortkit.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 06:06:57 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.shortkit.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 06:06:57 2026 GMT\n  hsts: null\ndomains:\n- domain: shortkit.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shortkit/refs/heads/main/security/shortkit-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Video
- Short-Form Video
- Video SDK
- Streaming
- Live Streaming
- Content Delivery
- Analytics
- Advertising
- Y Combinator
---
