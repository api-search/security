---
api_specs:
- filename: codehooks-database-rest-api-openapi.yml
  format: yaml
  label: Codehooks Database REST API
  slug: codehooks-database-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codehooks/refs/heads/main/openapi/codehooks-database-rest-api-openapi.yml
- filename: codehooks-events-asyncapi.yml
  format: yaml
  label: Codehooks Events (AsyncAPI)
  slug: codehooks-events
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/codehooks/refs/heads/main/asyncapi/codehooks-events-asyncapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: codehooks.io
  spf: false
hosts:
- cert_expires: Sep 11 20:43:32 2026 GMT
  host: codehooks.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Codehooks Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Codehooks, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Codehooks
provider_slug: codehooks
slug: codehooks-domain-security
source_filename: codehooks-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: codehooks.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 20:43:32 2026 GMT\n  hsts: false\ndomains:\n- domain: codehooks.io\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"digicert.com\"\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/codehooks/refs/heads/main/security/codehooks-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Backend
- Database
- Events
- Hooks
- JavaScript
- NoSQL
- Queues
- Serverless
- Webhooks
- Workers
- Workflows
---
