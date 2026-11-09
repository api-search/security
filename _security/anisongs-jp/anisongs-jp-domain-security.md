---
api_specs:
- filename: anisongs-jp-check-purity-api-openapi.yml
  format: yaml
  label: Anisongs Check Purity API
  slug: anisongs-jp-check-purity-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anisongs-jp/openapi/anisongs-jp-check-purity-api-openapi.yml
- filename: anisongs-jp-create-playlist-api-openapi.yml
  format: yaml
  label: Anisongs Create Playlist API
  slug: anisongs-jp-create-playlist-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anisongs-jp/openapi/anisongs-jp-create-playlist-api-openapi.yml
- filename: anisongs-jp-get-artist-api-openapi.yml
  format: yaml
  label: Anisongs Get Artist API
  slug: anisongs-jp-get-artist-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anisongs-jp/openapi/anisongs-jp-get-artist-api-openapi.yml
- filename: anisongs-jp-get-program-api-openapi.yml
  format: yaml
  label: Anisongs Get Program API
  slug: anisongs-jp-get-program-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anisongs-jp/openapi/anisongs-jp-get-program-api-openapi.yml
- filename: anisongs-jp-search-tracks-api-openapi.yml
  format: yaml
  label: Anisongs Search Tracks API
  slug: anisongs-jp-search-tracks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anisongs-jp/openapi/anisongs-jp-search-tracks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: anisongs.jp
  spf: true
hosts:
- cert_expires: Dec  7 03:52:03 2026 GMT
  host: anisongs.jp
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Anisongs Jp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Anisongs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Anisongs
provider_slug: anisongs-jp
slug: anisongs-jp-domain-security
source_filename: anisongs-jp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: anisongs.jp\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  7 03:52:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: anisongs.jp\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/anisongs-jp/security/anisongs-jp-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Anime
- Music
- Database
- Japanese
- Entertainment
---
