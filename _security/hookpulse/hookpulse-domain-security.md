---
api_specs:
- filename: openapi.json
  format: json
  label: HookPulse API
  slug: hookpulse-api
  spec_type: OpenAPI
  url: https://hookpulse.net/openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: hookpulse.net
  spf: true
hosts:
- cert_expires: Nov  8 23:28:14 2026 GMT
  host: hookpulse.net
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Hookpulse Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HookPulse, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: HookPulse
provider_slug: hookpulse
slug: hookpulse-domain-security
source_filename: hookpulse-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hookpulse.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  8 23:28:14 2026 GMT\n  hsts: false\ndomains:\n- domain: hookpulse.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hookpulse/refs/heads/main/security/hookpulse-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Monitoring
- Observability
- Cron
- Webhooks
- Heartbeat
- Dead-mans-switch
- Alerting
- Status pages
- Agent-native
- MCP
- x402
- Micropayments
---
