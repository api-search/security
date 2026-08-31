---
api_specs:
- filename: creditbenchmark-analytics-api-openapi.yml
  format: yaml
  label: Credit Benchmark Analytics API
  slug: creditbenchmark-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/creditbenchmark/refs/heads/main/openapi/creditbenchmark-analytics-api-openapi.yml
- filename: creditbenchmark-authentication-api-openapi.yml
  format: yaml
  label: Credit Benchmark Authentication API
  slug: creditbenchmark-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/creditbenchmark/refs/heads/main/openapi/creditbenchmark-authentication-api-openapi.yml
- filename: creditbenchmark-contributor-data-api-openapi.yml
  format: yaml
  label: Credit Benchmark Contributor Data API
  slug: creditbenchmark-contributor-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/creditbenchmark/refs/heads/main/openapi/creditbenchmark-contributor-data-api-openapi.yml
- filename: creditbenchmark-entity-data-api-openapi.yml
  format: yaml
  label: Credit Benchmark Entity Data API
  slug: creditbenchmark-entity-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/creditbenchmark/refs/heads/main/openapi/creditbenchmark-entity-data-api-openapi.yml
- filename: creditbenchmark-entity-matching-api-openapi.yml
  format: yaml
  label: Credit Benchmark Entity Matching API
  slug: creditbenchmark-entity-matching-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/creditbenchmark/refs/heads/main/openapi/creditbenchmark-entity-matching-api-openapi.yml
- filename: creditbenchmark-portfolio-analytics-api-openapi.yml
  format: yaml
  label: Credit Benchmark Portfolio Analytics API
  slug: creditbenchmark-portfolio-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/creditbenchmark/refs/heads/main/openapi/creditbenchmark-portfolio-analytics-api-openapi.yml
- filename: creditbenchmark-data-api-openapi.yml
  format: yaml
  label: Credit Benchmark Data API
  slug: creditbenchmark-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/creditbenchmark/refs/heads/main/openapi/creditbenchmark-data-api-openapi.yml
- filename: creditbenchmark-entity-resolution-api-openapi.yml
  format: yaml
  label: Credit Benchmark Entity Resolution API
  slug: creditbenchmark-entity-resolution-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/creditbenchmark/refs/heads/main/openapi/creditbenchmark-entity-resolution-api-openapi.yml
- filename: creditbenchmark-metadata-api-openapi.yml
  format: yaml
  label: Credit Benchmark Metadata API
  slug: creditbenchmark-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/creditbenchmark/refs/heads/main/openapi/creditbenchmark-metadata-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issuewild "amazon.com"
  - 0 issuewild "godaddy.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "starfieldtech.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: creditbenchmark.com
  spf: true
hosts:
- cert_expires: Aug  4 10:35:22 2026 GMT
  host: www.creditbenchmark.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug  4 10:35:22 2026 GMT
  host: api.creditbenchmark.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Creditbenchmark Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Credit Benchmark, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Credit Benchmark
provider_slug: creditbenchmark
slug: creditbenchmark-domain-security
source_filename: creditbenchmark-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.creditbenchmark.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  4 10:35:22 2026 GMT\n  hsts: false\n- host: api.creditbenchmark.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  4 10:35:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: creditbenchmark.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"godaddy.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"starfieldtech.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/creditbenchmark/refs/heads/main/security/creditbenchmark-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Credit Risk
- Financial Data
- Credit Ratings
- Analytics
- Risk Management
- Entity Resolution
- Consensus Data
---
