---
api_specs:
- filename: oruk-ai-affect-api-openapi.yml
  format: yaml
  label: oruk-ai Affect API
  slug: oruk-ai-affect-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/oruk-ai/openapi/oruk-ai-affect-api-openapi.yml
- filename: oruk-ai-audio-api-openapi.yml
  format: yaml
  label: oruk-ai Audio API
  slug: oruk-ai-audio-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/oruk-ai/openapi/oruk-ai-audio-api-openapi.yml
- filename: oruk-ai-client-token-api-openapi.yml
  format: yaml
  label: oruk-ai Client Token API
  slug: oruk-ai-client-token-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/oruk-ai/openapi/oruk-ai-client-token-api-openapi.yml
- filename: oruk-ai-livez-api-openapi.yml
  format: yaml
  label: oruk-ai Livez API
  slug: oruk-ai-livez-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/oruk-ai/openapi/oruk-ai-livez-api-openapi.yml
- filename: oruk-ai-models-api-openapi.yml
  format: yaml
  label: oruk-ai Models API
  slug: oruk-ai-models-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/oruk-ai/openapi/oruk-ai-models-api-openapi.yml
- filename: oruk-ai-orukzero-api-openapi.yml
  format: yaml
  label: oruk-ai Oruk Zero API
  slug: oruk-ai-orukzero-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/oruk-ai/openapi/oruk-ai-orukzero-api-openapi.yml
- filename: oruk-ai-pricing-api-openapi.yml
  format: yaml
  label: oruk-ai Pricing API
  slug: oruk-ai-pricing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/oruk-ai/openapi/oruk-ai-pricing-api-openapi.yml
- filename: oruk-ai-readyz-api-openapi.yml
  format: yaml
  label: oruk-ai Readyz API
  slug: oruk-ai-readyz-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/oruk-ai/openapi/oruk-ai-readyz-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: oruk.ai
  spf: true
hosts:
- cert_expires: Feb 12 04:59:51 2027 GMT
  host: oruk.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  4 21:13:37 2027 GMT
  host: speech-api.oruk.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Oruk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Oruk, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Oruk
provider_slug: oruk-ai
slug: oruk-ai-domain-security
source_filename: oruk-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: oruk.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 12 04:59:51 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: speech-api.oruk.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  4 21:13:37 2027 GMT\n  hsts: null\ndomains:\n- domain: oruk.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/oruk-ai/security/oruk-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Speech
- Artificial Intelligence
- Transcription
- Voice
---
