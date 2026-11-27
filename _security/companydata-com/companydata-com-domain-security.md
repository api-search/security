---
api_specs:
- filename: companydata-com-company-api-openapi.yml
  format: yaml
  label: CompanyData Company API
  slug: companydata-com-company-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/companydata-com/openapi/companydata-com-company-api-openapi.yml
- filename: companydata-com-corporate-structure-api-openapi.yml
  format: yaml
  label: CompanyData Corporate Structure API
  slug: companydata-com-corporate-structure-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/companydata-com/openapi/companydata-com-corporate-structure-api-openapi.yml
- filename: companydata-com-domain-enrichment-api-openapi.yml
  format: yaml
  label: CompanyData Domain Enrichment API
  slug: companydata-com-domain-enrichment-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/companydata-com/openapi/companydata-com-domain-enrichment-api-openapi.yml
- filename: companydata-com-lookup-api-openapi.yml
  format: yaml
  label: CompanyData Lookup API
  slug: companydata-com-lookup-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/companydata-com/openapi/companydata-com-lookup-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: companydata.com
  spf: true
hosts:
- cert_expires: Feb  1 14:57:14 2027 GMT
  host: companydata.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: CompanyData Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CompanyData, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: CompanyData
provider_slug: companydata-com
slug: companydata-com-domain-security
source_filename: companydata-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: companydata.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  1 14:57:14 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: companydata.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/companydata-com/security/companydata-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Company Data
- Business Registry
- B2B Data
- Data Enrichment
- KYC
- KYB
- Lead Generation
- MCP
---
