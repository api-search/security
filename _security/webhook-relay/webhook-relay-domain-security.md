---
api_specs:
- filename: webhook-relay-buckets-api-openapi.yml
  format: yaml
  label: Webhook Relay Buckets API
  slug: webhook-relay-buckets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webhook-relay/refs/heads/main/openapi/webhook-relay-buckets-api-openapi.yml
- filename: webhook-relay-domains-api-openapi.yml
  format: yaml
  label: Webhook Relay Domains API
  slug: webhook-relay-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webhook-relay/refs/heads/main/openapi/webhook-relay-domains-api-openapi.yml
- filename: webhook-relay-functions-api-openapi.yml
  format: yaml
  label: Webhook Relay Functions API
  slug: webhook-relay-functions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webhook-relay/refs/heads/main/openapi/webhook-relay-functions-api-openapi.yml
- filename: webhook-relay-inputs-api-openapi.yml
  format: yaml
  label: Webhook Relay Inputs API
  slug: webhook-relay-inputs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webhook-relay/refs/heads/main/openapi/webhook-relay-inputs-api-openapi.yml
- filename: webhook-relay-logs-api-openapi.yml
  format: yaml
  label: Webhook Relay Logs API
  slug: webhook-relay-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webhook-relay/refs/heads/main/openapi/webhook-relay-logs-api-openapi.yml
- filename: webhook-relay-outputs-api-openapi.yml
  format: yaml
  label: Webhook Relay Outputs API
  slug: webhook-relay-outputs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webhook-relay/refs/heads/main/openapi/webhook-relay-outputs-api-openapi.yml
- filename: webhook-relay-tokens-api-openapi.yml
  format: yaml
  label: Webhook Relay Tokens API
  slug: webhook-relay-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webhook-relay/refs/heads/main/openapi/webhook-relay-tokens-api-openapi.yml
- filename: webhook-relay-tunnels-api-openapi.yml
  format: yaml
  label: Webhook Relay Tunnels API
  slug: webhook-relay-tunnels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webhook-relay/refs/heads/main/openapi/webhook-relay-tunnels-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: webhookrelay.com
  spf: true
hosts:
- cert_expires: Dec  7 09:02:55 2026 GMT
  host: webhookrelay.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Webhook Relay Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Webhook Relay, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Webhook Relay
provider_slug: webhook-relay
slug: webhook-relay-domain-security
source_filename: webhook-relay-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: webhookrelay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  7 09:02:55 2026 GMT\n  hsts: false\ndomains:\n- domain: webhookrelay.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/webhook-relay/refs/heads/main/security/webhook-relay-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Webhook
- API Gateway
- Integration
- Developer Tools
---
