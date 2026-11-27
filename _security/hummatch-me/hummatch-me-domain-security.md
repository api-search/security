---
api_specs:
- filename: hummatch-me-api-openapi.yml
  format: yaml
  label: HumMatch Partner API API
  slug: hummatch-partner-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hummatch-me/openapi/_original/hummatch-me-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: hummatch.me
  spf: false
hosts:
- cert_expires: Dec 26 13:05:47 2026 GMT
  host: hummatch.me
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: HumMatch Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HumMatch, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: HumMatch
provider_slug: hummatch-me
slug: hummatch-me-domain-security
source_filename: hummatch-me-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hummatch.me\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 13:05:47 2026 GMT\n  hsts: false\ndomains:\n- domain: hummatch.me\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/hummatch-me/security/hummatch-me-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Vocal
- Music
- Karaoke
- Voice
---
