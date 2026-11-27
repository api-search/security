---
api_specs:
- filename: compeller-ai-auth-api-openapi.yml
  format: yaml
  label: Compeller Auth API
  slug: compeller-ai-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compeller-ai/openapi/compeller-ai-auth-api-openapi.yml
- filename: compeller-ai-compels-api-openapi.yml
  format: yaml
  label: Compeller Compels API
  slug: compeller-ai-compels-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compeller-ai/openapi/compeller-ai-compels-api-openapi.yml
- filename: compeller-ai-discovery-api-openapi.yml
  format: yaml
  label: Compeller Discovery API
  slug: compeller-ai-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compeller-ai/openapi/compeller-ai-discovery-api-openapi.yml
- filename: compeller-ai-lighting-api-openapi.yml
  format: yaml
  label: Compeller Lighting API
  slug: compeller-ai-lighting-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compeller-ai/openapi/compeller-ai-lighting-api-openapi.yml
- filename: compeller-ai-media-api-openapi.yml
  format: yaml
  label: Compeller Media API
  slug: compeller-ai-media-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compeller-ai/openapi/compeller-ai-media-api-openapi.yml
- filename: compeller-ai-music-api-openapi.yml
  format: yaml
  label: Compeller Music API
  slug: compeller-ai-music-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compeller-ai/openapi/compeller-ai-music-api-openapi.yml
- filename: compeller-ai-renderings-api-openapi.yml
  format: yaml
  label: Compeller Renderings API
  slug: compeller-ai-renderings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compeller-ai/openapi/compeller-ai-renderings-api-openapi.yml
- filename: compeller-ai-webhooks-api-openapi.yml
  format: yaml
  label: Compeller Webhooks API
  slug: compeller-ai-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compeller-ai/openapi/compeller-ai-webhooks-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 iodef "mailto:security@compeller.ai"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: compeller.ai
  spf: true
hosts:
- cert_expires: Jan 24 18:24:05 2027 GMT
  host: compeller.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Compeller Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Compeller, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Compeller
provider_slug: compeller-ai
slug: compeller-ai-domain-security
source_filename: compeller-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: compeller.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 24 18:24:05 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: compeller.ai\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 iodef \"mailto:security@compeller.ai\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/compeller-ai/security/compeller-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Music
- Video Generation
- Live Performance
- Audio Reactive Visuals
- MCP
---
