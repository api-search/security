---
api_specs:
- filename: audioalpha-io-episode-api-openapi.yml
  format: yaml
  label: AudioAlpha Episode API
  slug: audioalpha-io-episode-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/audioalpha-io/openapi/audioalpha-io-episode-api-openapi.yml
- filename: audioalpha-io-market-api-openapi.yml
  format: yaml
  label: AudioAlpha Market API
  slug: audioalpha-io-market-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/audioalpha-io/openapi/audioalpha-io-market-api-openapi.yml
- filename: audioalpha-io-personal-api-openapi.yml
  format: yaml
  label: AudioAlpha Personal API
  slug: audioalpha-io-personal-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/audioalpha-io/openapi/audioalpha-io-personal-api-openapi.yml
- filename: audioalpha-io-podcast-api-openapi.yml
  format: yaml
  label: AudioAlpha Podcast API
  slug: audioalpha-io-podcast-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/audioalpha-io/openapi/audioalpha-io-podcast-api-openapi.yml
- filename: audioalpha-io-ticker-api-openapi.yml
  format: yaml
  label: AudioAlpha Ticker API
  slug: audioalpha-io-ticker-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/audioalpha-io/openapi/audioalpha-io-ticker-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: audioalpha.io
  spf: true
hosts:
- cert_expires: Dec 17 00:40:28 2026 GMT
  host: audioalpha.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Audioalpha Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AudioAlpha, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: AudioAlpha
provider_slug: audioalpha-io
slug: audioalpha-io-domain-security
source_filename: audioalpha-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: audioalpha.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 17 00:40:28 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: audioalpha.io\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/audioalpha-io/security/audioalpha-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Finance
- Podcasts
- Transcription
- Market Data
- Company
---
