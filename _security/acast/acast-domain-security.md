---
api_specs:
- filename: acast-openapi.yml
  format: yaml
  label: Acast Shows API
  slug: acast-shows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acast/refs/heads/main/openapi/acast-openapi.yml
- filename: acast-openapi.yml
  format: yaml
  label: Acast Episodes API
  slug: acast-episodes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acast/refs/heads/main/openapi/acast-openapi.yml
- filename: acast-openapi.yml
  format: yaml
  label: Acast Ad Markers API
  slug: acast-ad-markers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acast/refs/heads/main/openapi/acast-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "microsoft.com"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 iodef "mailto:domains@acast.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: acast.com
  spf: true
hosts:
- cert_expires: Sep  9 18:02:09 2026 GMT
  host: www.acast.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 16:04:21 2026 GMT
  host: developers.acast.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: api.acast.com
  https: false
kind: domain-security
layout: security
method: probed
name: Acast Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Acast, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Acast
provider_slug: acast
slug: acast-domain-security
source_filename: acast-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.acast.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 18:02:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.acast.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 16:04:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.acast.com\n  https: false\ndomains:\n- domain: acast.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"microsoft.com\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 iodef \"mailto:domains@acast.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/acast/refs/heads/main/security/acast-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Podcasting
- Podcast Hosting
- Publishing
- Advertising
- Monetization
- Media
- Audio
---
