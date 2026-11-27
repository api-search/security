---
api_specs:
- filename: musicatlas-ai-openapi-generated.yml
  format: yaml
  label: MusicAtlas API
  slug: musicatlas-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/musicatlas-ai/openapi/_ae-authored/musicatlas-ai-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: musicatlas.ai
  spf: true
hosts:
- cert_expires: Dec 30 00:04:39 2026 GMT
  host: musicatlas.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: MusicAtlas Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MusicAtlas, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: MusicAtlas
provider_slug: musicatlas-ai
slug: musicatlas-ai-domain-security
source_filename: musicatlas-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: musicatlas.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 00:04:39 2026 GMT\n  hsts: false\ndomains:\n- domain: musicatlas.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/musicatlas-ai/security/musicatlas-ai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Music
- Search
- Discovery
- Open Data
---
