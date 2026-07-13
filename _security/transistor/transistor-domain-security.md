---
api_specs:
- filename: transistor-openapi.yml
  format: yaml
  label: Transistor Shows API
  slug: transistor-shows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/transistor/refs/heads/main/openapi/transistor-openapi.yml
- filename: transistor-openapi.yml
  format: yaml
  label: Transistor Episodes API
  slug: transistor-episodes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/transistor/refs/heads/main/openapi/transistor-openapi.yml
- filename: transistor-openapi.yml
  format: yaml
  label: Transistor Analytics API
  slug: transistor-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/transistor/refs/heads/main/openapi/transistor-openapi.yml
- filename: transistor-openapi.yml
  format: yaml
  label: Transistor Subscribers API
  slug: transistor-subscribers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/transistor/refs/heads/main/openapi/transistor-openapi.yml
- filename: transistor-openapi.yml
  format: yaml
  label: Transistor Webhooks API
  slug: transistor-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/transistor/refs/heads/main/openapi/transistor-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: transistor.fm
  spf: true
hosts:
- cert_expires: Oct  3 15:13:47 2026 GMT
  host: transistor.fm
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 13 00:29:30 2026 GMT
  host: developers.transistor.fm
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 05:43:46 2026 GMT
  host: api.transistor.fm
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Transistor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Transistor, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Transistor
provider_slug: transistor
slug: transistor-domain-security
source_filename: transistor-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: transistor.fm\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 15:13:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.transistor.fm\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 13 00:29:30 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.transistor.fm\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 05:43:46 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: transistor.fm\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/transistor/refs/heads/main/security/transistor-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Podcasting
- Podcast Hosting
- Analytics
- Media
- Audio
- JSON:API
---
