---
api_specs:
- filename: companyenrich-batches-api-openapi.yml
  format: yaml
  label: CompanyEnrich Batches API
  slug: companyenrich-batches-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/companyenrich/openapi/companyenrich-batches-api-openapi.yml
- filename: companyenrich-company-bulk-enrichment-api-openapi.yml
  format: yaml
  label: CompanyEnrich Company / Bulk Enrichment API
  slug: companyenrich-company-bulk-enrichment-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/companyenrich/openapi/companyenrich-company-bulk-enrichment-api-openapi.yml
- filename: companyenrich-company-enrichment-api-openapi.yml
  format: yaml
  label: CompanyEnrich Company / Enrichment API
  slug: companyenrich-company-enrichment-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/companyenrich/openapi/companyenrich-company-enrichment-api-openapi.yml
- filename: companyenrich-company-search-api-openapi.yml
  format: yaml
  label: CompanyEnrich Company / Search API
  slug: companyenrich-company-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/companyenrich/openapi/companyenrich-company-search-api-openapi.yml
- filename: companyenrich-company-search-export-api-openapi.yml
  format: yaml
  label: CompanyEnrich Company / Search Export API
  slug: companyenrich-company-search-export-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/companyenrich/openapi/companyenrich-company-search-export-api-openapi.yml
- filename: companyenrich-geo-api-openapi.yml
  format: yaml
  label: CompanyEnrich Geo API
  slug: companyenrich-geo-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/companyenrich/openapi/companyenrich-geo-api-openapi.yml
- filename: companyenrich-industries-api-openapi.yml
  format: yaml
  label: CompanyEnrich Industries API
  slug: companyenrich-industries-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/companyenrich/openapi/companyenrich-industries-api-openapi.yml
- filename: companyenrich-keywords-api-openapi.yml
  format: yaml
  label: CompanyEnrich Keywords API
  slug: companyenrich-keywords-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/companyenrich/openapi/companyenrich-keywords-api-openapi.yml
- filename: companyenrich-people-enrichment-api-openapi.yml
  format: yaml
  label: CompanyEnrich People / Enrichment API
  slug: companyenrich-people-enrichment-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/companyenrich/openapi/companyenrich-people-enrichment-api-openapi.yml
- filename: companyenrich-people-search-api-openapi.yml
  format: yaml
  label: CompanyEnrich People / Search API
  slug: companyenrich-people-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/companyenrich/openapi/companyenrich-people-search-api-openapi.yml
- filename: companyenrich-people-search-export-api-openapi.yml
  format: yaml
  label: CompanyEnrich People / Search Export API
  slug: companyenrich-people-search-export-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/companyenrich/openapi/companyenrich-people-search-export-api-openapi.yml
- filename: companyenrich-positions-api-openapi.yml
  format: yaml
  label: CompanyEnrich Positions API
  slug: companyenrich-positions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/companyenrich/openapi/companyenrich-positions-api-openapi.yml
- filename: companyenrich-technologies-api-openapi.yml
  format: yaml
  label: CompanyEnrich Technologies API
  slug: companyenrich-technologies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/companyenrich/openapi/companyenrich-technologies-api-openapi.yml
- filename: companyenrich-user-api-openapi.yml
  format: yaml
  label: CompanyEnrich User API
  slug: companyenrich-user-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/companyenrich/openapi/companyenrich-user-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: companyenrich.com
  spf: true
hosts:
- cert_expires: Feb  4 11:58:10 2027 GMT
  host: companyenrich.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 27 14:12:44 2026 GMT
  host: docs.companyenrich.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  8 06:07:18 2027 GMT
  host: api.companyenrich.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: CompanyEnrich Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CompanyEnrich, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: CompanyEnrich
provider_slug: companyenrich
slug: companyenrich-domain-security
source_filename: companyenrich-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: companyenrich.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  4 11:58:10 2027 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: docs.companyenrich.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 14:12:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.companyenrich.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 06:07:18 2027 GMT\n  hsts: null\ndomains:\n- domain: companyenrich.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/companyenrich/security/companyenrich-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- B2B
- Data
- Data Enrichment
- Artificial Intelligence
---
