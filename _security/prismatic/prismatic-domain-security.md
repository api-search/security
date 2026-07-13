---
api_specs:
- filename: prismatic-graphql-api-openapi.yml
  format: yaml
  label: Prismatics GraphQL API
  slug: prismatics-graphql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prismatic/refs/heads/main/openapi/prismatic-graphql-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "amazonaws.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: prismatic.io
  spf: true
hosts:
- cert_expires: Feb  8 23:59:59 2027 GMT
  host: prismatic.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  8 23:59:59 2027 GMT
  host: app.prismatic.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Prismatic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Prismatic, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Prismatic
provider_slug: prismatic
slug: prismatic-domain-security
source_filename: prismatic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: prismatic.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  8 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: app.prismatic.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  8 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: prismatic.io\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/prismatic/refs/heads/main/security/prismatic-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Embedded iPaaS
- Integrations
- Workflows
- Connectors
- AI Agents
- MCP
- Code-Native
- Low-Code
---
