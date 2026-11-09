---
api_specs:
- filename: spoken-md-transcripts-api-openapi.yml
  format: yaml
  label: Podcast Transcripts API
  slug: podcast-transcripts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/spoken-md/openapi/spoken-md-transcripts-api-openapi.yml
- filename: spoken-md-well-known-openapi.json
  format: json
  label: Podcast Transcripts API .well-known API
  slug: podcast-transcripts-api-well-known-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/spoken-md/openapi/_original/spoken-md-well-known-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: spoken.md
  spf: true
hosts:
- cert_expires: Mar  4 23:59:59 2027 GMT
  host: spoken.md
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Spoken Md Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for spoken-md, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: spoken-md
provider_slug: spoken-md
slug: spoken-md-domain-security
source_filename: spoken-md-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: spoken.md\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  4 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: spoken.md\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/spoken-md/security/spoken-md-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Podcasts
- Transcripts
- Markdown
- Artificial Intelligence
---
