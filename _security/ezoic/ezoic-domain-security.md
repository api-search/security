---
api_specs:
- filename: ezoic-subscriptions-openapi.yml
  format: yaml
  label: Ezoic Subscriptions Server-to-Server REST API
  slug: ezoic-subscriptions-server-to-server-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ezoic/refs/heads/main/openapi/ezoic-subscriptions-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ezoic.com
  spf: true
hosts:
- cert_expires: Oct 16 12:07:58 2026 GMT
  host: www.ezoic.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ezoic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ezoic, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: ezoic
provider_slug: ezoic
slug: ezoic-domain-security
source_filename: ezoic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ezoic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 12:07:58 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: ezoic.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ezoic/refs/heads/main/security/ezoic-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Advertising
- AdTech
- Publisher Monetization
- Analytics
- Subscriptions
- Identity
- MCP
---
