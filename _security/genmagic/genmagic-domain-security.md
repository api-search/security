---
api_specs:
- filename: genmagic-agent-api-openapi.yml
  format: yaml
  label: GenMagic Agent API
  slug: genmagic-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/genmagic/openapi/genmagic-agent-api-openapi.yml
- filename: genmagic-audio-api-openapi.yml
  format: yaml
  label: GenMagic Audio API
  slug: genmagic-audio-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/genmagic/openapi/genmagic-audio-api-openapi.yml
- filename: genmagic-benchmarks-api-openapi.yml
  format: yaml
  label: GenMagic Benchmarks API
  slug: genmagic-benchmarks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/genmagic/openapi/genmagic-benchmarks-api-openapi.yml
- filename: genmagic-images-api-openapi.yml
  format: yaml
  label: GenMagic Images API
  slug: genmagic-images-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/genmagic/openapi/genmagic-images-api-openapi.yml
- filename: genmagic-models-api-openapi.yml
  format: yaml
  label: GenMagic Models API
  slug: genmagic-models-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/genmagic/openapi/genmagic-models-api-openapi.yml
- filename: genmagic-text-api-openapi.yml
  format: yaml
  label: GenMagic Text API
  slug: genmagic-text-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/genmagic/openapi/genmagic-text-api-openapi.yml
- filename: genmagic-usage-api-openapi.yml
  format: yaml
  label: GenMagic Usage API
  slug: genmagic-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/genmagic/openapi/genmagic-usage-api-openapi.yml
- filename: genmagic-videos-api-openapi.yml
  format: yaml
  label: GenMagic Videos API
  slug: genmagic-videos-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/genmagic/openapi/genmagic-videos-api-openapi.yml
- filename: genmagic-chat-completions-api-openapi.yml
  format: yaml
  label: GenMagic Chat Completions API
  slug: genmagic-chat-completions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/genmagic/openapi/genmagic-chat-completions-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: genmagic.co
  spf: false
hosts:
- cert_expires: Dec 12 15:07:25 2026 GMT
  host: genmagic.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: GenMagic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GenMagic, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: GenMagic
provider_slug: genmagic
slug: genmagic-domain-security
source_filename: genmagic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: genmagic.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 15:07:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: genmagic.co\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/genmagic/security/genmagic-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Generative AI
- Media
- Subscription
---
