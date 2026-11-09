---
api_specs:
- filename: byimprint-com-mcp-api-openapi.yml
  format: yaml
  label: byImprint MCP API
  slug: byimprint-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/byimprint-com/openapi/byimprint-com-mcp-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: byimprint.com
  spf: true
hosts:
- cert_expires: Dec  9 03:14:29 2026 GMT
  host: byimprint.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Byimprint Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for byImprint, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: byImprint
provider_slug: byimprint-com
slug: byimprint-com-domain-security
source_filename: byimprint-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: byimprint.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  9 03:14:29 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: byimprint.com\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/byimprint-com/security/byimprint-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Website Design
- Customer Experience
---
