---
api_specs:
- filename: tulimoa-com-openapi-generated.yml
  format: yaml
  label: tulimoa-com API
  slug: tulimoa-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tulimoa-com/openapi/_ae-authored/tulimoa-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: tulimoa.com
  spf: true
hosts:
- cert_expires: Jan 24 19:53:33 2027 GMT
  host: tulimoa.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Tulimoa Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for tulimoa-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: tulimoa-com
provider_slug: tulimoa-com
slug: tulimoa-com-domain-security
source_filename: tulimoa-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tulimoa.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 24 19:53:33 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: tulimoa.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/tulimoa-com/security/tulimoa-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Directory
- AI
- MCP
- Reviews
---
