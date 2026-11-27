---
api_specs:
- filename: falconbuilder-dev-openapi-generated.yml
  format: yaml
  label: Falcon Builder API
  slug: falconbuilder-dev-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/falconbuilder-dev/openapi/_ae-authored/falconbuilder-dev-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: falconbuilder.dev
  spf: true
hosts:
- cert_expires: Dec 31 03:51:23 2026 GMT
  host: falconbuilder.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Falcon Builder Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Falcon Builder, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Falcon Builder
provider_slug: falconbuilder-dev
slug: falconbuilder-dev-domain-security
source_filename: falconbuilder-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: falconbuilder.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 03:51:23 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: falconbuilder.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/falconbuilder-dev/security/falconbuilder-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- No-Code
- Platform
- Automation
- Workflows
---
