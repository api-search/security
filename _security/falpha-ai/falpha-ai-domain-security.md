---
api_specs:
- filename: falpha-ai-account-api-openapi.yml
  format: yaml
  label: fAlpha Account API
  slug: falpha-ai-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/falpha-ai/openapi/falpha-ai-account-api-openapi.yml
- filename: falpha-ai-discovery-api-openapi.yml
  format: yaml
  label: fAlpha Discovery API
  slug: falpha-ai-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/falpha-ai/openapi/falpha-ai-discovery-api-openapi.yml
- filename: falpha-ai-events-api-openapi.yml
  format: yaml
  label: fAlpha Events API
  slug: falpha-ai-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/falpha-ai/openapi/falpha-ai-events-api-openapi.yml
- filename: falpha-ai-health-api-openapi.yml
  format: yaml
  label: fAlpha Health API
  slug: falpha-ai-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/falpha-ai/openapi/falpha-ai-health-api-openapi.yml
- filename: falpha-ai-news-api-openapi.yml
  format: yaml
  label: fAlpha News API
  slug: falpha-ai-news-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/falpha-ai/openapi/falpha-ai-news-api-openapi.yml
- filename: falpha-ai-signals-api-openapi.yml
  format: yaml
  label: fAlpha Signals API
  slug: falpha-ai-signals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/falpha-ai/openapi/falpha-ai-signals-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: falpha.ai
  spf: true
hosts:
- cert_expires: Apr 14 23:59:59 2027 GMT
  host: falpha.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: fAlpha Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for fAlpha, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: fAlpha
provider_slug: falpha-ai
slug: falpha-ai-domain-security
source_filename: falpha-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: falpha.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 14 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: falpha.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/falpha-ai/security/falpha-ai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Finance
- Artificial Intelligence
- Trading
- Validation
- Analytics
---
