---
api_specs:
- filename: z-league-leads-api-openapi.yml
  format: yaml
  label: Z League Leads API
  slug: z-league-leads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/z-league/refs/heads/main/openapi/z-league-leads-api-openapi.yml
- filename: z-league-webhooks-api-openapi.yml
  format: yaml
  label: Z League Webhooks API
  slug: z-league-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/z-league/refs/heads/main/openapi/z-league-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: gomega.ai
  spf: true
hosts:
- cert_expires: Sep  1 01:27:54 2026 GMT
  host: www.gomega.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 26 07:48:29 2026 GMT
  host: docs.gomega.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 20 23:21:17 2026 GMT
  host: app.gomega.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Z League Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Z League, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Z League
provider_slug: z-league
slug: z-league-domain-security
source_filename: z-league-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.gomega.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 01:27:54 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.gomega.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 07:48:29 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.gomega.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 23:21:17 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: gomega.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/z-league/refs/heads/main/security/z-league-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- CRM
- Leads
- Marketing
- AI Agents
- SEO
- Advertising
- Webhook
- Gaming
---
