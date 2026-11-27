---
api_specs:
- filename: paperlantern-ai-fastapi-api-openapi.yml
  format: yaml
  label: Paper Lantern Fast API
  slug: paperlantern-ai-fastapi-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/paperlantern-ai/openapi/paperlantern-ai-fastapi-api-openapi.yml
- filename: paperlantern-ai-health-api-openapi.yml
  format: yaml
  label: Paper Lantern Health API
  slug: paperlantern-ai-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/paperlantern-ai/openapi/paperlantern-ai-health-api-openapi.yml
- filename: paperlantern-ai-learning-api-openapi.yml
  format: yaml
  label: Paper Lantern Learning API
  slug: paperlantern-ai-learning-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/paperlantern-ai/openapi/paperlantern-ai-learning-api-openapi.yml
- filename: paperlantern-ai-neurips-api-openapi.yml
  format: yaml
  label: Paper Lantern Neurips API
  slug: paperlantern-ai-neurips-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/paperlantern-ai/openapi/paperlantern-ai-neurips-api-openapi.yml
- filename: paperlantern-ai-newsletters-api-openapi.yml
  format: yaml
  label: Paper Lantern Newsletters API
  slug: paperlantern-ai-newsletters-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/paperlantern-ai/openapi/paperlantern-ai-newsletters-api-openapi.yml
- filename: paperlantern-ai-paper-search-api-openapi.yml
  format: yaml
  label: Paper Lantern Paper Search API
  slug: paperlantern-ai-paper-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/paperlantern-ai/openapi/paperlantern-ai-paper-search-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: paperlantern.ai
  spf: false
hosts:
- cert_expires: Dec 26 00:04:52 2026 GMT
  host: paperlantern.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Paper Lantern Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Paper Lantern, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Paper Lantern
provider_slug: paperlantern-ai
slug: paperlantern-ai-domain-security
source_filename: paperlantern-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: paperlantern.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 00:04:52 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: paperlantern.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/paperlantern-ai/security/paperlantern-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
---
