---
api_specs:
- filename: fiskmas-dev-openapi-generated.yml
  format: yaml
  label: Fiskmås API
  slug: fiskmas-dev-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fiskmas-dev/openapi/_ae-authored/fiskmas-dev-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: fiskmas.dev
  spf: false
hosts:
- cert_expires: Dec  9 21:05:39 2026 GMT
  host: fiskmas.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Fiskmås Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fiskmås, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Fiskmås
provider_slug: fiskmas-dev
slug: fiskmas-dev-domain-security
source_filename: fiskmas-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fiskmas.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  9 21:05:39 2026 GMT\n  hsts: false\ndomains:\n- domain: fiskmas.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/fiskmas-dev/security/fiskmas-dev-domain-security.yml
summary_line: TLSv1.3
tags:
- Artificial Intelligence
- Hosting
- Platform
- MCP
- Agents
---
