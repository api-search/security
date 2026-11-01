---
api_specs:
- filename: cite42-dev-openapi-generated.yml
  format: yaml
  label: cite42-dev API
  slug: cite42-dev-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cite42-dev/openapi/_ae-authored/cite42-dev-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cite42.dev
  spf: true
hosts:
- cert_expires: Dec 24 23:59:59 2026 GMT
  host: cite42.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cite42 Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for cite42-dev, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: cite42-dev
provider_slug: cite42-dev
slug: cite42-dev-domain-security
source_filename: cite42-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cite42.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cite42.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/cite42-dev/security/cite42-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI
- SEO
- MCP
- Data
- Visibility
---
