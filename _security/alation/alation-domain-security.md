---
api_specs:
- filename: alation-data-catalog-openapi.yaml
  format: yaml
  label: Alation Data Catalog API
  slug: data-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alation/refs/heads/main/openapi/alation-data-catalog-openapi.yaml
- filename: alation-lineage-openapi.yaml
  format: yaml
  label: Alation Lineage API
  slug: lineage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alation/refs/heads/main/openapi/alation-lineage-openapi.yaml
- filename: alation-governance-openapi.yaml
  format: yaml
  label: Alation Governance API
  slug: governance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alation/refs/heads/main/openapi/alation-governance-openapi.yaml
- filename: alation-search-openapi.yaml
  format: yaml
  label: Alation Search API
  slug: search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alation/refs/heads/main/openapi/alation-search-openapi.yaml
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
- AI
---
