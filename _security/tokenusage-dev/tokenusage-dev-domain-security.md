---
api_specs:
- filename: tokenusage-dev-nerfwatch-api-openapi.yml
  format: yaml
  label: tokenusage-dev Nerfwatch API
  slug: tokenusage-dev-nerfwatch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tokenusage-dev/openapi/tokenusage-dev-nerfwatch-api-openapi.yml
- filename: tokenusage-dev-resets-api-openapi.yml
  format: yaml
  label: tokenusage-dev Resets API
  slug: tokenusage-dev-resets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tokenusage-dev/openapi/tokenusage-dev-resets-api-openapi.yml
- filename: tokenusage-dev-resets-atom-api-openapi.yml
  format: yaml
  label: tokenusage-dev Resets.atom API
  slug: tokenusage-dev-resets-atom-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tokenusage-dev/openapi/tokenusage-dev-resets-atom-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: tokenusage.dev
  spf: true
hosts:
- cert_expires: Jan  5 12:03:42 2027 GMT
  host: tokenusage.dev
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Tokenusage Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for tokenusage-dev, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: tokenusage-dev
provider_slug: tokenusage-dev
slug: tokenusage-dev-domain-security
source_filename: tokenusage-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tokenusage.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 12:03:42 2027 GMT\n  hsts: true\n  hsts_max_age: 31556926\ndomains:\n- domain: tokenusage.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/tokenusage-dev/security/tokenusage-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Token Usage
- Artificial Intelligence
- Analytics
- OpenAI
- Anthropic
---
