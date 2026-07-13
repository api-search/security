---
api_specs:
- filename: taddy-podcast-openapi.yml
  format: yaml
  label: Taddy Podcast API
  slug: taddy-podcast-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taddy-api/refs/heads/main/openapi/taddy-podcast-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: taddy.org
  spf: true
hosts:
- cert_expires: Oct  4 20:24:33 2026 GMT
  host: taddy.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  6 02:33:19 2026 GMT
  host: api.taddy.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Taddy Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Taddy API, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Taddy API
provider_slug: taddy-api
slug: taddy-api-domain-security
source_filename: taddy-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: taddy.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 20:24:33 2026 GMT\n  hsts: false\n- host: api.taddy.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 02:33:19 2026 GMT\n  hsts: false\ndomains:\n- domain: taddy.org\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/taddy-api/refs/heads/main/security/taddy-api-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Audio
- Comics
- GraphQL
- Media
- Podcasts
- Transcripts
- Webhooks
---
