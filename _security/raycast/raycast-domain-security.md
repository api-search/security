---
api_specs:
- filename: raycast-openapi.yml
  format: yaml
  label: Raycast Extension API (SDK)
  slug: raycast-extension-api-sdk
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/raycast/refs/heads/main/openapi/raycast-openapi.yml
- filename: raycast-openapi.yml
  format: yaml
  label: Raycast AI API
  slug: raycast-ai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/raycast/refs/heads/main/openapi/raycast-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: raycast.com
  spf: true
hosts:
- cert_expires: Aug 15 08:28:25 2026 GMT
  host: www.raycast.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 31 13:47:38 2026 GMT
  host: developers.raycast.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Raycast Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Raycast, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Raycast
provider_slug: raycast
slug: raycast-domain-security
source_filename: raycast-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.raycast.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 15 08:28:25 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developers.raycast.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 13:47:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: raycast.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/raycast/refs/heads/main/security/raycast-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Productivity
- Launcher
- Extensions
- SDK
- AI
- macOS
---
