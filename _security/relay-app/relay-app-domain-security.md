---
api_specs:
- filename: relay-app-openapi.yml
  format: yaml
  label: Relay App Automation API
  slug: relay-app-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/relay-app/refs/heads/main/openapi/relay-app-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: relay.app
  spf: true
hosts:
- cert_expires: Sep 14 07:48:12 2026 GMT
  host: www.relay.app
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 13:45:45 2026 GMT
  host: docs.relay.app
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: api.relay.app
  https: false
kind: domain-security
layout: security
method: probed
name: Relay App Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Relay App, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Relay App
provider_slug: relay-app
slug: relay-app-domain-security
source_filename: relay-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.relay.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 07:48:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.relay.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 13:45:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.relay.app\n  https: false\ndomains:\n- domain: relay.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/relay-app/refs/heads/main/security/relay-app-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Automation
- Workflow
- Integration
- No-Code
- AI
- Webhooks
---
