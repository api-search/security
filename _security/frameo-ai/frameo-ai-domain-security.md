---
api_specs:
- filename: frameo-ai-account-api-openapi.yml
  format: yaml
  label: Frameo Account API
  slug: frameo-ai-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/frameo-ai/openapi/frameo-ai-account-api-openapi.yml
- filename: frameo-ai-events-api-openapi.yml
  format: yaml
  label: Frameo Events API
  slug: frameo-ai-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/frameo-ai/openapi/frameo-ai-events-api-openapi.yml
- filename: frameo-ai-generations-api-openapi.yml
  format: yaml
  label: Frameo Generations API
  slug: frameo-ai-generations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/frameo-ai/openapi/frameo-ai-generations-api-openapi.yml
- filename: frameo-ai-models-api-openapi.yml
  format: yaml
  label: Frameo Models API
  slug: frameo-ai-models-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/frameo-ai/openapi/frameo-ai-models-api-openapi.yml
- filename: frameo-ai-uploads-api-openapi.yml
  format: yaml
  label: Frameo Uploads API
  slug: frameo-ai-uploads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/frameo-ai/openapi/frameo-ai-uploads-api-openapi.yml
- filename: frameo-ai-webhooks-api-openapi.yml
  format: yaml
  label: Frameo Webhooks API
  slug: frameo-ai-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/frameo-ai/openapi/frameo-ai-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: frameo.ai
  spf: true
hosts:
- cert_expires: Jan 12 12:59:33 2027 GMT
  host: frameo.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Frameo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Frameo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Frameo
provider_slug: frameo-ai
slug: frameo-ai-domain-security
source_filename: frameo-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: frameo.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 12:59:33 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: frameo.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/frameo-ai/security/frameo-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Video
- Production
- Platform
- Creative
---
