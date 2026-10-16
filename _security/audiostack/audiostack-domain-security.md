---
api_specs:
- filename: audiostack-openapi-generated.yml
  format: yaml
  label: AudioStack API
  slug: audiostack-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/audiostack/refs/heads/main/openapi/_ae-authored/audiostack-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: audiostack.ai
  spf: true
hosts:
- cert_expires: Dec 16 09:33:48 2026 GMT
  host: audiostack.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Audiostack Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AudioStack, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: AudioStack
provider_slug: audiostack
slug: audiostack-domain-security
source_filename: audiostack-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: audiostack.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 16 09:33:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: audiostack.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/audiostack/refs/heads/main/security/audiostack-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI
- Audio
- Advertising
- Platform
---
