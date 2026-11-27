---
api_specs:
- filename: hireeli-io-buyer-agent-api-openapi.yml
  format: yaml
  label: Eli Buyer Agent API
  slug: hireeli-io-buyer-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hireeli-io/openapi/hireeli-io-buyer-agent-api-openapi.yml
- filename: hireeli-io-legacy-api-openapi.yml
  format: yaml
  label: Eli Legacy API
  slug: hireeli-io-legacy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hireeli-io/openapi/hireeli-io-legacy-api-openapi.yml
- filename: hireeli-io-own-site-execution-api-openapi.yml
  format: yaml
  label: Eli Own-site execution API
  slug: hireeli-io-own-site-execution-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hireeli-io/openapi/hireeli-io-own-site-execution-api-openapi.yml
- filename: hireeli-io-public-api-openapi.yml
  format: yaml
  label: Eli Public API
  slug: hireeli-io-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hireeli-io/openapi/hireeli-io-public-api-openapi.yml
- filename: hireeli-io-workspace-reads-api-openapi.yml
  format: yaml
  label: Eli Workspace reads API
  slug: hireeli-io-workspace-reads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hireeli-io/openapi/hireeli-io-workspace-reads-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: hireeli.io
  spf: true
hosts:
- cert_expires: Jan  3 17:18:08 2027 GMT
  host: hireeli.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Eli Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Eli, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Eli
provider_slug: hireeli-io
slug: hireeli-io-domain-security
source_filename: hireeli-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hireeli.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 17:18:08 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: hireeli.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/hireeli-io/security/hireeli-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Growth
- SEO
- Automation
- B2B
---
