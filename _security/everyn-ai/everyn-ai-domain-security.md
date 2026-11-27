---
api_specs:
- filename: everyn-ai-alert-rules-api-openapi.yml
  format: yaml
  label: Everyn Alert Rules API
  slug: everyn-ai-alert-rules-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/everyn-ai/openapi/everyn-ai-alert-rules-api-openapi.yml
- filename: everyn-ai-billing-api-openapi.yml
  format: yaml
  label: Everyn Billing API
  slug: everyn-ai-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/everyn-ai/openapi/everyn-ai-billing-api-openapi.yml
- filename: everyn-ai-callable-jobs-api-openapi.yml
  format: yaml
  label: Everyn Callable Jobs API
  slug: everyn-ai-callable-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/everyn-ai/openapi/everyn-ai-callable-jobs-api-openapi.yml
- filename: everyn-ai-dataset-uploads-api-openapi.yml
  format: yaml
  label: Everyn Dataset Uploads API
  slug: everyn-ai-dataset-uploads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/everyn-ai/openapi/everyn-ai-dataset-uploads-api-openapi.yml
- filename: everyn-ai-datasets-api-openapi.yml
  format: yaml
  label: Everyn Datasets API
  slug: everyn-ai-datasets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/everyn-ai/openapi/everyn-ai-datasets-api-openapi.yml
- filename: everyn-ai-exports-api-openapi.yml
  format: yaml
  label: Everyn Exports API
  slug: everyn-ai-exports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/everyn-ai/openapi/everyn-ai-exports-api-openapi.yml
- filename: everyn-ai-health-api-openapi.yml
  format: yaml
  label: Everyn Health API
  slug: everyn-ai-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/everyn-ai/openapi/everyn-ai-health-api-openapi.yml
- filename: everyn-ai-job-specs-api-openapi.yml
  format: yaml
  label: Everyn Job Specs API
  slug: everyn-ai-job-specs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/everyn-ai/openapi/everyn-ai-job-specs-api-openapi.yml
- filename: everyn-ai-models-api-openapi.yml
  format: yaml
  label: Everyn Models API
  slug: everyn-ai-models-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/everyn-ai/openapi/everyn-ai-models-api-openapi.yml
- filename: everyn-ai-organization-admin-api-openapi.yml
  format: yaml
  label: Everyn Organization Admin API
  slug: everyn-ai-organization-admin-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/everyn-ai/openapi/everyn-ai-organization-admin-api-openapi.yml
- filename: everyn-ai-runs-api-openapi.yml
  format: yaml
  label: Everyn Runs API
  slug: everyn-ai-runs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/everyn-ai/openapi/everyn-ai-runs-api-openapi.yml
- filename: everyn-ai-usage-api-openapi.yml
  format: yaml
  label: Everyn Usage API
  slug: everyn-ai-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/everyn-ai/openapi/everyn-ai-usage-api-openapi.yml
- filename: everyn-ai-webhooks-api-openapi.yml
  format: yaml
  label: Everyn Webhooks API
  slug: everyn-ai-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/everyn-ai/openapi/everyn-ai-webhooks-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: everyn.ai
  spf: true
hosts:
- cert_expires: Jan 13 20:55:51 2027 GMT
  host: everyn.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Everyn Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Everyn, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Everyn
provider_slug: everyn-ai
slug: everyn-ai-domain-security
source_filename: everyn-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: everyn.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 20:55:51 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: everyn.ai\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/everyn-ai/security/everyn-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Automation
- Productivity
- Agents
- Platform
---
