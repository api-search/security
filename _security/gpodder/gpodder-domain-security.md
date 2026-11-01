---
api_specs:
- filename: gpodder-openapi-generated.yml
  format: yaml
  label: gpodder.net API
  slug: gpodder-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gpodder/openapi/_ae-authored/gpodder-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: gpodder.net
  spf: true
hosts:
- cert_expires: Dec 11 12:58:38 2026 GMT
  host: gpodder.net
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Gpodder Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for gpodder.net, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: gpodder.net
provider_slug: gpodder
slug: gpodder-domain-security
source_filename: gpodder-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gpodder.net\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 11 12:58:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: gpodder.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/gpodder/security/gpodder-domain-security.yml
summary_line: TLSv1.2 · HSTS
tags:
- Podcast
- Open-Source
- Sync
- API
- Community
---
