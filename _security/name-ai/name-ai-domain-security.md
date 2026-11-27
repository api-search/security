---
api_specs:
- filename: name-ai-batch-api-openapi.yml
  format: yaml
  label: Name.ai Batch API
  slug: name-ai-batch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/name-ai/openapi/name-ai-batch-api-openapi.yml
- filename: name-ai-domain-api-openapi.yml
  format: yaml
  label: Name.ai Domain API
  slug: name-ai-domain-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/name-ai/openapi/name-ai-domain-api-openapi.yml
- filename: name-ai-domains-api-openapi.yml
  format: yaml
  label: Name.ai Domains API
  slug: name-ai-domains-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/name-ai/openapi/name-ai-domains-api-openapi.yml
- filename: name-ai-market-api-openapi.yml
  format: yaml
  label: Name.ai Market API
  slug: name-ai-market-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/name-ai/openapi/name-ai-market-api-openapi.yml
- filename: name-ai-pricing-api-openapi.yml
  format: yaml
  label: Name.ai Pricing API
  slug: name-ai-pricing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/name-ai/openapi/name-ai-pricing-api-openapi.yml
- filename: name-ai-tlds-api-openapi.yml
  format: yaml
  label: Name.ai Tlds API
  slug: name-ai-tlds-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/name-ai/openapi/name-ai-tlds-api-openapi.yml
- filename: name-ai-tools-api-openapi.yml
  format: yaml
  label: Name.ai Tools API
  slug: name-ai-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/name-ai/openapi/name-ai-tools-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: name.ai
  spf: true
hosts:
- cert_expires: Jan  3 05:35:52 2027 GMT
  host: name.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Name.ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Name.ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Name.ai
provider_slug: name-ai
slug: name-ai-domain-security
source_filename: name-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: name.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 05:35:52 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: name.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/name-ai/security/name-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Artificial Intelligence
- Domain
- Marketplace
- Software-as-a-Service
---
