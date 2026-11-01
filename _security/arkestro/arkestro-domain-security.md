---
api_specs:
- filename: arkestro-webhooks-api-openapi.yml
  format: yaml
  label: Arkestro Webhooks API
  slug: arkestro-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arkestro/openapi/arkestro-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: arkestro.com
  spf: true
hosts:
- cert_expires: Oct  1 07:58:37 2026 GMT
  host: arkestro.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 23 06:49:05 2026 GMT
  host: api.arkestro.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Arkestro Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Arkestro, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Arkestro
provider_slug: arkestro
slug: arkestro-domain-security
source_filename: arkestro-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: arkestro.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 07:58:37 2026 GMT\n  hsts: false\n- host: api.arkestro.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 06:49:05 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: arkestro.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/arkestro/security/arkestro-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Procurement
- Sourcing
- Supply Chain
- Spend Management
- eSourcing
- Supplier Management
- Purchase Orders
- procurement-analytics
- Enterprise Software
- predictive-procurement
- MCP
- Webhook
---
