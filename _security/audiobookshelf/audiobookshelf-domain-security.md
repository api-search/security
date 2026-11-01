---
api_specs:
- filename: audiobookshelf-openapi-generated.yml
  format: yaml
  label: Audiobookshelf API
  slug: audiobookshelf-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/audiobookshelf/openapi/_ae-authored/audiobookshelf-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: audiobookshelf.org
  spf: false
hosts:
- cert_expires: Jan 15 19:53:50 2027 GMT
  host: audiobookshelf.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Audiobookshelf Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Audiobookshelf, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: Audiobookshelf
provider_slug: audiobookshelf
slug: audiobookshelf-domain-security
source_filename: audiobookshelf-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: audiobookshelf.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 19:53:50 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: audiobookshelf.org\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/audiobookshelf/security/audiobookshelf-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Company
- Self-Hosted
- Audiobooks
- Podcast
- Media Server
---
