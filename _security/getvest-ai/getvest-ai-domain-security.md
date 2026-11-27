---
api_specs:
- filename: getvest-ai-claim-api-openapi.yml
  format: yaml
  label: Vest Claim API
  slug: getvest-ai-claim-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getvest-ai/openapi/getvest-ai-claim-api-openapi.yml
- filename: getvest-ai-estimate-api-openapi.yml
  format: yaml
  label: Vest Estimate API
  slug: getvest-ai-estimate-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getvest-ai/openapi/getvest-ai-estimate-api-openapi.yml
- filename: getvest-ai-stack-api-openapi.yml
  format: yaml
  label: Vest Stack API
  slug: getvest-ai-stack-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getvest-ai/openapi/getvest-ai-stack-api-openapi.yml
- filename: getvest-ai-submit-tool-api-openapi.yml
  format: yaml
  label: Vest Submit Tool API
  slug: getvest-ai-submit-tool-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getvest-ai/openapi/getvest-ai-submit-tool-api-openapi.yml
- filename: getvest-ai-tools-api-openapi.yml
  format: yaml
  label: Vest Tools API
  slug: getvest-ai-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getvest-ai/openapi/getvest-ai-tools-api-openapi.yml
- filename: getvest-ai-wallet-api-openapi.yml
  format: yaml
  label: Vest Wallet API
  slug: getvest-ai-wallet-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getvest-ai/openapi/getvest-ai-wallet-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: getvest.ai
  spf: false
hosts:
- cert_expires: Jan 19 19:10:16 2027 GMT
  host: getvest.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Vest Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vest, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: Vest
provider_slug: getvest-ai
slug: getvest-ai-domain-security
source_filename: getvest-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getvest.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 19:10:16 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: getvest.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/getvest-ai/security/getvest-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Partnerships
- Growth Platform
- Channel Management
- Marketplace Integration
---
