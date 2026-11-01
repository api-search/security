---
api_specs:
- filename: citation-co-balance-api-openapi.yml
  format: yaml
  label: Citation Balance API
  slug: citation-co-balance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/citation-co/openapi/citation-co-balance-api-openapi.yml
- filename: citation-co-checks-api-openapi.yml
  format: yaml
  label: Citation Checks API
  slug: citation-co-checks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/citation-co/openapi/citation-co-checks-api-openapi.yml
- filename: citation-co-documents-api-openapi.yml
  format: yaml
  label: Citation Documents API
  slug: citation-co-documents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/citation-co/openapi/citation-co-documents-api-openapi.yml
- filename: citation-co-events-api-openapi.yml
  format: yaml
  label: Citation Events API
  slug: citation-co-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/citation-co/openapi/citation-co-events-api-openapi.yml
- filename: citation-co-exports-api-openapi.yml
  format: yaml
  label: Citation Exports API
  slug: citation-co-exports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/citation-co/openapi/citation-co-exports-api-openapi.yml
- filename: citation-co-files-api-openapi.yml
  format: yaml
  label: Citation Files API
  slug: citation-co-files-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/citation-co/openapi/citation-co-files-api-openapi.yml
- filename: citation-co-imports-api-openapi.yml
  format: yaml
  label: Citation Imports API
  slug: citation-co-imports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/citation-co/openapi/citation-co-imports-api-openapi.yml
- filename: citation-co-jobs-api-openapi.yml
  format: yaml
  label: Citation Jobs API
  slug: citation-co-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/citation-co/openapi/citation-co-jobs-api-openapi.yml
- filename: citation-co-ledger-api-openapi.yml
  format: yaml
  label: Citation Ledger API
  slug: citation-co-ledger-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/citation-co/openapi/citation-co-ledger-api-openapi.yml
- filename: citation-co-me-api-openapi.yml
  format: yaml
  label: Citation Me API
  slug: citation-co-me-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/citation-co/openapi/citation-co-me-api-openapi.yml
- filename: citation-co-pricing-api-openapi.yml
  format: yaml
  label: Citation Pricing API
  slug: citation-co-pricing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/citation-co/openapi/citation-co-pricing-api-openapi.yml
- filename: citation-co-sources-api-openapi.yml
  format: yaml
  label: Citation Sources API
  slug: citation-co-sources-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/citation-co/openapi/citation-co-sources-api-openapi.yml
- filename: citation-co-webhooks-api-openapi.yml
  format: yaml
  label: Citation Webhooks API
  slug: citation-co-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/citation-co/openapi/citation-co-webhooks-api-openapi.yml
- filename: citation-co-write-api-openapi.yml
  format: yaml
  label: Citation Write API
  slug: citation-co-write-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/citation-co/openapi/citation-co-write-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: citation.co
  spf: true
hosts:
- cert_expires: Jan  6 15:40:20 2027 GMT
  host: citation.co
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Citation Co Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Citation, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Citation
provider_slug: citation-co
slug: citation-co-domain-security
source_filename: citation-co-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: citation.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 15:40:20 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: citation.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/citation-co/security/citation-co-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Citation
- Bibliography
- WritingTool
- Academic
- Productivity
---
