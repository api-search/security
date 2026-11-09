---
api_specs:
- filename: benchgecko-ai-gecko-tests-api-openapi.yml
  format: yaml
  label: BenchGecko Gecko Tests API
  slug: benchgecko-ai-gecko-tests-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/benchgecko-ai/openapi/benchgecko-ai-gecko-tests-api-openapi.yml
- filename: benchgecko-ai-models-api-openapi.yml
  format: yaml
  label: BenchGecko Models API
  slug: benchgecko-ai-models-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/benchgecko-ai/openapi/benchgecko-ai-models-api-openapi.yml
- filename: benchgecko-ai-pricing-api-openapi.yml
  format: yaml
  label: BenchGecko Pricing API
  slug: benchgecko-ai-pricing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/benchgecko-ai/openapi/benchgecko-ai-pricing-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: benchgecko.ai
  spf: true
hosts:
- cert_expires: Jan  1 20:02:11 2027 GMT
  host: benchgecko.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Benchgecko Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BenchGecko, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: BenchGecko
provider_slug: benchgecko-ai
slug: benchgecko-ai-domain-security
source_filename: benchgecko-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: benchgecko.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 20:02:11 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: benchgecko.ai\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/benchgecko-ai/security/benchgecko-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Economy
- Dashboards
- Analytics
- Market Intelligence
---
