---
api_specs:
- filename: captivate-fm-openapi.yml
  format: yaml
  label: Captivate Users API
  slug: captivate-fm-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/captivate-fm/refs/heads/main/openapi/captivate-fm-openapi.yml
- filename: captivate-fm-openapi.yml
  format: yaml
  label: Captivate Shows API
  slug: captivate-fm-shows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/captivate-fm/refs/heads/main/openapi/captivate-fm-openapi.yml
- filename: captivate-fm-openapi.yml
  format: yaml
  label: Captivate Episodes API
  slug: captivate-fm-episodes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/captivate-fm/refs/heads/main/openapi/captivate-fm-openapi.yml
- filename: captivate-fm-openapi.yml
  format: yaml
  label: Captivate Media API
  slug: captivate-fm-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/captivate-fm/refs/heads/main/openapi/captivate-fm-openapi.yml
- filename: captivate-fm-openapi.yml
  format: yaml
  label: Captivate Analytics API
  slug: captivate-fm-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/captivate-fm/refs/heads/main/openapi/captivate-fm-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: captivate.fm
  spf: true
hosts:
- cert_expires: Aug 17 16:38:47 2026 GMT
  host: www.captivate.fm
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 15:48:19 2026 GMT
  host: docs.captivate.fm
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  6 23:59:59 2027 GMT
  host: api.captivate.fm
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Captivate Fm Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Captivate, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Captivate
provider_slug: captivate-fm
slug: captivate-fm-domain-security
source_filename: captivate-fm-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.captivate.fm\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 16:38:47 2026 GMT\n  hsts: false\n- host: docs.captivate.fm\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 15:48:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.captivate.fm\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan  6 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: captivate.fm\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/captivate-fm/refs/heads/main/security/captivate-fm-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Podcasting
- Podcast Hosting
- Episodes
- Media
- Analytics
- RSS
---
