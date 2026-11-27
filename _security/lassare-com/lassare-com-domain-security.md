---
api_specs:
- filename: lassare-com-admin-api-openapi.yml
  format: yaml
  label: Lassare Admin API
  slug: lassare-com-admin-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lassare-com/openapi/lassare-com-admin-api-openapi.yml
- filename: lassare-com-decision-api-openapi.yml
  format: yaml
  label: Lassare Decision API
  slug: lassare-com-decision-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lassare-com/openapi/lassare-com-decision-api-openapi.yml
- filename: lassare-com-health-api-openapi.yml
  format: yaml
  label: Lassare Health API
  slug: lassare-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lassare-com/openapi/lassare-com-health-api-openapi.yml
- filename: lassare-com-logs-api-openapi.yml
  format: yaml
  label: Lassare Logs API
  slug: lassare-com-logs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lassare-com/openapi/lassare-com-logs-api-openapi.yml
- filename: lassare-com-settings-api-openapi.yml
  format: yaml
  label: Lassare Settings API
  slug: lassare-com-settings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lassare-com/openapi/lassare-com-settings-api-openapi.yml
- filename: lassare-com-slack-api-openapi.yml
  format: yaml
  label: Lassare Slack API
  slug: lassare-com-slack-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lassare-com/openapi/lassare-com-slack-api-openapi.yml
- filename: lassare-com-teams-api-openapi.yml
  format: yaml
  label: Lassare Teams API
  slug: lassare-com-teams-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lassare-com/openapi/lassare-com-teams-api-openapi.yml
- filename: lassare-com-webhook-decisions-api-openapi.yml
  format: yaml
  label: Lassare Webhook Decisions API
  slug: lassare-com-webhook-decisions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lassare-com/openapi/lassare-com-webhook-decisions-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: lassare.com
  spf: true
hosts:
- cert_expires: Mar  6 23:59:59 2027 GMT
  host: lassare.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Lassare Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lassare, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Lassare
provider_slug: lassare-com
slug: lassare-com-domain-security
source_filename: lassare-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lassare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  6 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: lassare.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/lassare-com/security/lassare-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Human-in-the-Loop
- MCP Protocol
- Remote agent control
- Developer Tools
---
