---
api_specs:
- filename: megaphone-openapi.yml
  format: yaml
  label: Megaphone Networks API
  slug: megaphone-networks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/megaphone/refs/heads/main/openapi/megaphone-openapi.yml
- filename: megaphone-openapi.yml
  format: yaml
  label: Megaphone Podcasts API
  slug: megaphone-podcasts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/megaphone/refs/heads/main/openapi/megaphone-openapi.yml
- filename: megaphone-openapi.yml
  format: yaml
  label: Megaphone Episodes API
  slug: megaphone-episodes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/megaphone/refs/heads/main/openapi/megaphone-openapi.yml
- filename: megaphone-openapi.yml
  format: yaml
  label: Megaphone Campaigns and Orders API
  slug: megaphone-campaigns-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/megaphone/refs/heads/main/openapi/megaphone-openapi.yml
- filename: megaphone-openapi.yml
  format: yaml
  label: Megaphone Direct Sales API v2
  slug: megaphone-direct-sales-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/megaphone/refs/heads/main/openapi/megaphone-openapi.yml
- filename: megaphone-openapi.yml
  format: yaml
  label: Megaphone Metrics and Impressions Export API
  slug: megaphone-metrics-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/megaphone/refs/heads/main/openapi/megaphone-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: spotify.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: megaphone.fm
  spf: true
hosts:
- cert_expires: Jan 23 23:59:59 2027 GMT
  host: megaphone.spotify.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 25 23:59:59 2026 GMT
  host: developers.megaphone.fm
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 25 23:59:59 2026 GMT
  host: cms.megaphone.fm
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Megaphone Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Megaphone, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Megaphone
provider_slug: megaphone
slug: megaphone-domain-security
source_filename: megaphone-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: megaphone.spotify.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.megaphone.fm\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 25 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: cms.megaphone.fm\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 25 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: spotify.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: megaphone.fm\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/megaphone/refs/heads/main/security/megaphone-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Podcasting
- Podcast Hosting
- Advertising
- Ad Monetization
- Dynamic Ad Insertion
- Media
- Spotify
---
