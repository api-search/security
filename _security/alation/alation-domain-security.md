---
api_specs:
- filename: alation-aggregated-context-api-openapi.yml
  format: yaml
  label: Alation Aggregated Context API
  slug: alation-aggregated-context-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alation/refs/heads/main/openapi/alation-aggregated-context-api-openapi.yml
- filename: alation-columns-api-openapi.yml
  format: yaml
  label: Alation Columns API
  slug: alation-columns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alation/refs/heads/main/openapi/alation-columns-api-openapi.yml
- filename: alation-custom-fields-api-openapi.yml
  format: yaml
  label: Alation Custom Fields API
  slug: alation-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alation/refs/heads/main/openapi/alation-custom-fields-api-openapi.yml
- filename: alation-data-quality-api-openapi.yml
  format: yaml
  label: Alation Data Quality API
  slug: alation-data-quality-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alation/refs/heads/main/openapi/alation-data-quality-api-openapi.yml
- filename: alation-data-sources-api-openapi.yml
  format: yaml
  label: Alation Data Sources API
  slug: alation-data-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alation/refs/heads/main/openapi/alation-data-sources-api-openapi.yml
- filename: alation-dataflows-api-openapi.yml
  format: yaml
  label: Alation Dataflows API
  slug: alation-dataflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alation/refs/heads/main/openapi/alation-dataflows-api-openapi.yml
- filename: alation-glossary-terms-api-openapi.yml
  format: yaml
  label: Alation Glossary Terms API
  slug: alation-glossary-terms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alation/refs/heads/main/openapi/alation-glossary-terms-api-openapi.yml
- filename: alation-lineage-api-openapi.yml
  format: yaml
  label: Alation Lineage API
  slug: alation-lineage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alation/refs/heads/main/openapi/alation-lineage-api-openapi.yml
- filename: alation-policies-api-openapi.yml
  format: yaml
  label: Alation Policies API
  slug: alation-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alation/refs/heads/main/openapi/alation-policies-api-openapi.yml
- filename: alation-schemas-api-openapi.yml
  format: yaml
  label: Alation Schemas API
  slug: alation-schemas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alation/refs/heads/main/openapi/alation-schemas-api-openapi.yml
- filename: alation-search-api-openapi.yml
  format: yaml
  label: Alation Search API
  slug: alation-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alation/refs/heads/main/openapi/alation-search-api-openapi.yml
- filename: alation-tables-api-openapi.yml
  format: yaml
  label: Alation Tables API
  slug: alation-tables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alation/refs/heads/main/openapi/alation-tables-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: alation.com
  spf: true
hosts:
- cert_expires: Sep  3 23:18:39 2026 GMT
  host: alation.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 07:56:03 2026 GMT
  host: developer.alation.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: your-instance.alation.com
  https: false
kind: domain-security
layout: security
method: probed
name: Alation Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Alation, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Alation
provider_slug: alation
slug: alation-domain-security
source_filename: alation-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: alation.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 23:18:39 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.alation.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 07:56:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: your-instance.alation.com\n  https: false\ndomains:\n- domain: alation.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alation/refs/heads/main/security/alation-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Data Catalog
- Data Governance
- Data Intelligence
- Data Lineage
- Data Quality
- Business Glossary
- Metadata Management
- Artificial Intelligence
---
