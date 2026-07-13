---
api_specs:
- filename: sync-labs-openapi.yml
  format: yaml
  label: Sync Labs API
  slug: sync-labs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sync-labs/refs/heads/main/openapi/sync-labs-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sync.so
  spf: true
hosts:
- cert_expires: Sep 16 10:31:30 2026 GMT
  host: sync.so
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 10:31:30 2026 GMT
  host: api.sync.so
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sync Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sync Labs, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Sync Labs
provider_slug: sync-labs
slug: sync-labs-domain-security
source_filename: sync-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sync.so\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 10:31:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.sync.so\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 10:31:30 2026 GMT\n  hsts: null\ndomains:\n- domain: sync.so\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sync-labs/refs/heads/main/security/sync-labs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Content Localization
- Dubbing
- Lip Sync
- Media
- Video
- Visual AI
---
