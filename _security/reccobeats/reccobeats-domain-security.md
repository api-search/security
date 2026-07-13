---
api_specs:
- filename: reccobeats-openapi.yml
  format: yaml
  label: ReccoBeats Track API
  slug: reccobeats-track-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reccobeats/refs/heads/main/openapi/reccobeats-openapi.yml
- filename: reccobeats-openapi.yml
  format: yaml
  label: ReccoBeats Audio Features API
  slug: reccobeats-audio-features-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reccobeats/refs/heads/main/openapi/reccobeats-openapi.yml
- filename: reccobeats-openapi.yml
  format: yaml
  label: ReccoBeats Audio Analysis API
  slug: reccobeats-audio-analysis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reccobeats/refs/heads/main/openapi/reccobeats-openapi.yml
- filename: reccobeats-openapi.yml
  format: yaml
  label: ReccoBeats Recommendation API
  slug: reccobeats-recommendation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reccobeats/refs/heads/main/openapi/reccobeats-openapi.yml
- filename: reccobeats-openapi.yml
  format: yaml
  label: ReccoBeats Artist API
  slug: reccobeats-artist-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reccobeats/refs/heads/main/openapi/reccobeats-openapi.yml
- filename: reccobeats-openapi.yml
  format: yaml
  label: ReccoBeats Album API
  slug: reccobeats-album-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reccobeats/refs/heads/main/openapi/reccobeats-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: reccobeats.com
  spf: true
hosts:
- cert_expires: Sep 11 13:47:49 2026 GMT
  host: reccobeats.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 11 13:47:49 2026 GMT
  host: api.reccobeats.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Reccobeats Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ReccoBeats, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: ReccoBeats
provider_slug: reccobeats
slug: reccobeats-domain-security
source_filename: reccobeats-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: reccobeats.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 13:47:49 2026 GMT\n  hsts: false\n- host: api.reccobeats.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 13:47:49 2026 GMT\n  hsts: null\ndomains:\n- domain: reccobeats.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reccobeats/refs/heads/main/security/reccobeats-domain-security.yml
summary_line: TLSv1.3
tags:
- Music
- Recommendations
- Audio Features
- Audio Analysis
- Music Database
- Spotify Alternative
---
