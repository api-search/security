---
api_specs:
- filename: music-story-artist-api-openapi.yml
  format: yaml
  label: Music Story Artist API
  slug: music-story-artist-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/music-story/refs/heads/main/openapi/music-story-artist-api-openapi.yml
- filename: music-story-music-story-api-api-openapi.yml
  format: yaml
  label: Music Story Music Story API
  slug: music-story-music-story-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/music-story/refs/heads/main/openapi/music-story-music-story-api-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: music-story.com
  spf: true
hosts:
- cert_expires: Dec  7 07:03:55 2026 GMT
  host: music-story.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Music Story Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Music Story, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Music Story
provider_slug: music-story
slug: music-story-domain-security
source_filename: music-story-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: music-story.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  7 07:03:55 2026 GMT\n  hsts: false\ndomains:\n- domain: music-story.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/music-story/refs/heads/main/security/music-story-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Music
- Metadata
- Services
---
