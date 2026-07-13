---
api_specs:
- filename: podbean-openapi.yml
  format: yaml
  label: Podbean Podcasts API
  slug: podbean-podcasts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/podbean/refs/heads/main/openapi/podbean-openapi.yml
- filename: podbean-openapi.yml
  format: yaml
  label: Podbean Episodes API
  slug: podbean-episodes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/podbean/refs/heads/main/openapi/podbean-openapi.yml
- filename: podbean-openapi.yml
  format: yaml
  label: Podbean Media Files API
  slug: podbean-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/podbean/refs/heads/main/openapi/podbean-openapi.yml
- filename: podbean-openapi.yml
  format: yaml
  label: Podbean Analytics API
  slug: podbean-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/podbean/refs/heads/main/openapi/podbean-openapi.yml
- filename: podbean-openapi.yml
  format: yaml
  label: Podbean oEmbed API
  slug: podbean-oembed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/podbean/refs/heads/main/openapi/podbean-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: podbean.com
  spf: true
hosts:
- cert_expires: Oct  3 07:55:00 2026 GMT
  host: www.podbean.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 25 23:59:59 2026 GMT
  host: developers.podbean.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 25 23:59:59 2026 GMT
  host: api.podbean.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Podbean Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Podbean, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Podbean
provider_slug: podbean
slug: podbean-domain-security
source_filename: podbean-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.podbean.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 07:55:00 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: developers.podbean.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.podbean.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: podbean.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/podbean/refs/heads/main/security/podbean-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Podcasting
- Podcast Hosting
- Media
- Audio
- Episodes
- Analytics
- Monetization
---
