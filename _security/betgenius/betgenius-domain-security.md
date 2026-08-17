---
api_specs:
- filename: betgenius-booking-v2-openapi.yml
  format: yaml
  label: BetGenius Booking API V2
  slug: betgenius-booking-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/betgenius/refs/heads/main/openapi/betgenius-booking-v2-openapi.yml
- filename: betgenius-booking-v1-openapi.yml
  format: yaml
  label: BetGenius Booking API V1
  slug: betgenius-booking-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/betgenius/refs/heads/main/openapi/betgenius-booking-v1-openapi.yml
- filename: betgenius-video-v3-openapi.yml
  format: yaml
  label: BetGenius Video Streaming API v3
  slug: betgenius-video-streaming-api-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/betgenius/refs/heads/main/openapi/betgenius-video-v3-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: betgenius.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: geniussports.com
  spf: true
hosts:
- host: www.betgenius.com
  https: false
- cert_expires: Dec 26 23:59:59 2026 GMT
  host: dataservices.betgenius.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 28 23:59:59 2026 GMT
  host: api.geniussports.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Betgenius Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BetGenius, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: BetGenius
provider_slug: betgenius
slug: betgenius-domain-security
source_filename: betgenius-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.betgenius.com\n  https: false\n- host: dataservices.betgenius.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: api.geniussports.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: betgenius.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: geniussports.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/betgenius/refs/heads/main/security/betgenius-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Sportsbook
- Sports Betting
- Sports Data
- Odds Feeds
- Trading Services
- Risk Management
- Live Streaming
- In-Play Betting
- BetBuilder
- Player Engagement
- Marketing Technology
- Gambling
---
