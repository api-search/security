---
api_specs:
- filename: linear-graphql-openapi.yml
  format: yaml
  label: Linear GraphQL API
  slug: linear-graphql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linear/refs/heads/main/openapi/linear-graphql-openapi.yml
- filename: linear-webhooks-asyncapi.yml
  format: yaml
  label: Linear Webhooks API
  slug: linear-webhooks-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/linear/refs/heads/main/asyncapi/linear-webhooks-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: linear.app
  spf: true
hosts:
- cert_expires: Oct  6 22:29:55 2026 GMT
  host: linear.app
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 22:29:55 2026 GMT
  host: api.linear.app
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Linear Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for linear, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: linear
provider_slug: linear
slug: linear-domain-security
source_filename: linear-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: linear.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 22:29:55 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.linear.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 22:29:55 2026 GMT\n  hsts: false\ndomains:\n- domain: linear.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/linear/refs/heads/main/security/linear-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags: []
---
