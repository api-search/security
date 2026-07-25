---
api_specs:
- filename: vast-ai-accounts-api-openapi.yml
  format: yaml
  label: Vast.ai Accounts API
  slug: vast-ai-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vast-ai/refs/heads/main/openapi/vast-ai-accounts-api-openapi.yml
- filename: vast-ai-billing-api-openapi.yml
  format: yaml
  label: Vast.ai Billing API
  slug: vast-ai-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vast-ai/refs/heads/main/openapi/vast-ai-billing-api-openapi.yml
- filename: vast-ai-instances-api-openapi.yml
  format: yaml
  label: Vast.ai Instances API
  slug: vast-ai-instances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vast-ai/refs/heads/main/openapi/vast-ai-instances-api-openapi.yml
- filename: vast-ai-machines-api-openapi.yml
  format: yaml
  label: Vast.ai Machines API
  slug: vast-ai-machines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vast-ai/refs/heads/main/openapi/vast-ai-machines-api-openapi.yml
- filename: vast-ai-network-volumes-api-openapi.yml
  format: yaml
  label: Vast.ai Network Volumes API
  slug: vast-ai-network-volumes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vast-ai/refs/heads/main/openapi/vast-ai-network-volumes-api-openapi.yml
- filename: vast-ai-search-api-openapi.yml
  format: yaml
  label: Vast.ai Search API
  slug: vast-ai-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vast-ai/refs/heads/main/openapi/vast-ai-search-api-openapi.yml
- filename: vast-ai-serverless-api-openapi.yml
  format: yaml
  label: Vast.ai Serverless API
  slug: vast-ai-serverless-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vast-ai/refs/heads/main/openapi/vast-ai-serverless-api-openapi.yml
- filename: vast-ai-team-api-openapi.yml
  format: yaml
  label: Vast.ai Team API
  slug: vast-ai-team-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vast-ai/refs/heads/main/openapi/vast-ai-team-api-openapi.yml
- filename: vast-ai-templates-api-openapi.yml
  format: yaml
  label: Vast.ai Templates API
  slug: vast-ai-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vast-ai/refs/heads/main/openapi/vast-ai-templates-api-openapi.yml
- filename: vast-ai-volumes-api-openapi.yml
  format: yaml
  label: Vast.ai Volumes API
  slug: vast-ai-volumes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vast-ai/refs/heads/main/openapi/vast-ai-volumes-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: vast.ai
  spf: true
hosts:
- cert_expires: Sep 23 04:06:43 2026 GMT
  host: vast.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 21:26:11 2026 GMT
  host: cloud.vast.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 17 00:55:05 2026 GMT
  host: docs.vast.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vast Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vast.ai, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Vast.ai
provider_slug: vast-ai
slug: vast-ai-domain-security
source_filename: vast-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: vast.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 04:06:43 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: cloud.vast.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 21:26:11 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.vast.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 00:55:05 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: vast.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vast-ai/refs/heads/main/security/vast-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Cloud
- Compute
- GPU
- Machine Learning
- Marketplace
- Serverless
---
