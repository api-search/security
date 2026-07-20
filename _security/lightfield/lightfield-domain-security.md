---
api_specs:
- filename: lightfield-openapi-original.yml
  format: yaml
  label: Lightfield API
  slug: lightfield-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lightfield/refs/heads/main/openapi/lightfield-openapi-original.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: lightfield.app
  spf: true
hosts:
- cert_expires: Aug 23 14:10:11 2026 GMT
  host: lightfield.app
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 22:59:52 2026 GMT
  host: docs.lightfield.app
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  1 23:59:59 2026 GMT
  host: api.lightfield.app
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lightfield Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lightfield, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Lightfield
provider_slug: lightfield
slug: lightfield-domain-security
source_filename: lightfield-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lightfield.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 14:10:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.lightfield.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 22:59:52 2026 GMT\n  hsts: false\n- host: api.lightfield.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: lightfield.app\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lightfield/refs/heads/main/security/lightfield-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Applications
- CRM
- Sales
- Artificial Intelligence
- Agents
- Customer Relationship Management
- Go To Market
- Productivity
- SaaS
---
