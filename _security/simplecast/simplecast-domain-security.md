---
api_specs:
- filename: simplecast-openapi.yml
  format: yaml
  label: Simplecast Podcasts API
  slug: simplecast-podcasts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simplecast/refs/heads/main/openapi/simplecast-openapi.yml
- filename: simplecast-openapi.yml
  format: yaml
  label: Simplecast Episodes API
  slug: simplecast-episodes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simplecast/refs/heads/main/openapi/simplecast-openapi.yml
- filename: simplecast-openapi.yml
  format: yaml
  label: Simplecast Analytics API
  slug: simplecast-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simplecast/refs/heads/main/openapi/simplecast-openapi.yml
- filename: simplecast-openapi.yml
  format: yaml
  label: Simplecast Distribution API
  slug: simplecast-distribution-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simplecast/refs/heads/main/openapi/simplecast-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: simplecast.com
  spf: true
hosts:
- cert_expires: Aug 14 07:16:48 2026 GMT
  host: www.simplecast.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 03:16:30 2026 GMT
  host: apidocs.simplecast.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  6 23:59:59 2026 GMT
  host: api.simplecast.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Simplecast Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Simplecast, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Simplecast
provider_slug: simplecast
slug: simplecast-domain-security
source_filename: simplecast-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.simplecast.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 07:16:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: apidocs.simplecast.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 03:16:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.simplecast.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: simplecast.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/simplecast/refs/heads/main/security/simplecast-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Podcasting
- Podcast Hosting
- Podcast Distribution
- Podcast Analytics
- Audio
- Media
- SiriusXM Media
---
