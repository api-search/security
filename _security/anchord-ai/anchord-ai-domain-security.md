---
api_specs:
- filename: anchord-ai-dupes-api-openapi.yml
  format: yaml
  label: Anchord AI Dupes API
  slug: anchord-ai-dupes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anchord-ai/openapi/anchord-ai-dupes-api-openapi.yml
- filename: anchord-ai-entities-api-openapi.yml
  format: yaml
  label: Anchord AI Entities API
  slug: anchord-ai-entities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anchord-ai/openapi/anchord-ai-entities-api-openapi.yml
- filename: anchord-ai-guard-api-openapi.yml
  format: yaml
  label: Anchord AI Guard API
  slug: anchord-ai-guard-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anchord-ai/openapi/anchord-ai-guard-api-openapi.yml
- filename: anchord-ai-health-api-openapi.yml
  format: yaml
  label: Anchord AI Health API
  slug: anchord-ai-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anchord-ai/openapi/anchord-ai-health-api-openapi.yml
- filename: anchord-ai-ingest-api-openapi.yml
  format: yaml
  label: Anchord AI Ingest API
  slug: anchord-ai-ingest-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anchord-ai/openapi/anchord-ai-ingest-api-openapi.yml
- filename: anchord-ai-links-api-openapi.yml
  format: yaml
  label: Anchord AI Links API
  slug: anchord-ai-links-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anchord-ai/openapi/anchord-ai-links-api-openapi.yml
- filename: anchord-ai-resolve-api-openapi.yml
  format: yaml
  label: Anchord AI Resolve API
  slug: anchord-ai-resolve-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anchord-ai/openapi/anchord-ai-resolve-api-openapi.yml
- filename: anchord-ai-sources-api-openapi.yml
  format: yaml
  label: Anchord AI Sources API
  slug: anchord-ai-sources-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anchord-ai/openapi/anchord-ai-sources-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: anchord.ai
  spf: true
hosts:
- cert_expires: Mar 22 23:59:59 2027 GMT
  host: anchord.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Anchord Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Anchord AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Anchord AI
provider_slug: anchord-ai
slug: anchord-ai-domain-security
source_filename: anchord-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: anchord.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 22 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: anchord.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/anchord-ai/security/anchord-ai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Artificial Intelligence
- Identity
- Trust
- Write-Guard
- Integration
---
