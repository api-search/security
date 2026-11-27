---
api_specs:
- filename: hookpie-account-api-openapi.yml
  format: yaml
  label: Hookpie Account API
  slug: hookpie-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hookpie/openapi/hookpie-account-api-openapi.yml
- filename: hookpie-accounts-api-openapi.yml
  format: yaml
  label: Hookpie Accounts API
  slug: hookpie-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hookpie/openapi/hookpie-accounts-api-openapi.yml
- filename: hookpie-i-api-openapi.yml
  format: yaml
  label: Hookpie I API
  slug: hookpie-i-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hookpie/openapi/hookpie-i-api-openapi.yml
- filename: hookpie-inboxes-api-openapi.yml
  format: yaml
  label: Hookpie Inboxes API
  slug: hookpie-inboxes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hookpie/openapi/hookpie-inboxes-api-openapi.yml
- filename: hookpie-pricing-api-openapi.yml
  format: yaml
  label: Hookpie Pricing API
  slug: hookpie-pricing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hookpie/openapi/hookpie-pricing-api-openapi.yml
- filename: hookpie-usage-api-openapi.yml
  format: yaml
  label: Hookpie Usage API
  slug: hookpie-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hookpie/openapi/hookpie-usage-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: hookpie.com
  spf: true
hosts:
- cert_expires: May 30 23:42:17 2027 GMT
  host: hookpie.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Hookpie Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hookpie, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Hookpie
provider_slug: hookpie
slug: hookpie-domain-security
source_filename: hookpie-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hookpie.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: May 30 23:42:17 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: hookpie.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/hookpie/security/hookpie-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Webhook
- AI Agents
- MCP
- Event Inbox
- Developer Tools
- Pay-as-you-go
---
