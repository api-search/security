---
api_specs:
- filename: sapling-account-api-openapi.yml
  format: yaml
  label: Sapling Account API
  slug: sapling-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sapling/openapi/sapling-account-api-openapi.yml
- filename: sapling-analysis-api-openapi.yml
  format: yaml
  label: Sapling Analysis API
  slug: sapling-analysis-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sapling/openapi/sapling-analysis-api-openapi.yml
- filename: sapling-detection-api-openapi.yml
  format: yaml
  label: Sapling Detection API
  slug: sapling-detection-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sapling/openapi/sapling-detection-api-openapi.yml
- filename: sapling-files-api-openapi.yml
  format: yaml
  label: Sapling Files API
  slug: sapling-files-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sapling/openapi/sapling-files-api-openapi.yml
- filename: sapling-generation-api-openapi.yml
  format: yaml
  label: Sapling Generation API
  slug: sapling-generation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sapling/openapi/sapling-generation-api-openapi.yml
- filename: sapling-proofreading-api-openapi.yml
  format: yaml
  label: Sapling Proofreading API
  slug: sapling-proofreading-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sapling/openapi/sapling-proofreading-api-openapi.yml
- filename: sapling-service-api-openapi.yml
  format: yaml
  label: Sapling Service API
  slug: sapling-service-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sapling/openapi/sapling-service-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 iodef "mailto:security@sapling.ai"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: sapling.ai
  spf: true
hosts:
- cert_expires: Feb 28 23:59:59 2027 GMT
  host: sapling.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Sapling Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sapling, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Sapling
provider_slug: sapling
slug: sapling-domain-security
source_filename: sapling-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sapling.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 28 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: sapling.ai\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 iodef \"mailto:security@sapling.ai\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/sapling/security/sapling-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- AI
- Language-Model
- API
- Enterprise
- Productivity
---
