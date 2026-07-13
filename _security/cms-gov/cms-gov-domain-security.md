---
api_specs:
- filename: cms-gov-blue-button-2-openapi.yml
  format: yaml
  label: CMS Blue Button 2.0 API
  slug: blue-button-2-fhir-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cms-gov/refs/heads/main/openapi/cms-gov-blue-button-2-openapi.yml
- filename: cms-gov-bcda-openapi.yml
  format: yaml
  label: CMS Beneficiary Claims Data API (BCDA)
  slug: beneficiary-claims-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cms-gov/refs/heads/main/openapi/cms-gov-bcda-openapi.yml
- filename: cms-gov-ab2d-openapi.yml
  format: yaml
  label: CMS AB2D API
  slug: ab2d-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cms-gov/refs/heads/main/openapi/cms-gov-ab2d-openapi.yml
- filename: cms-gov-dpc-openapi.yml
  format: yaml
  label: CMS Data at the Point of Care API (DPC)
  slug: data-at-point-of-care-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cms-gov/refs/heads/main/openapi/cms-gov-dpc-openapi.yml
- filename: cms-gov-bfd-openapi.yml
  format: yaml
  label: CMS Beneficiary FHIR Data Server (BFD)
  slug: bfd-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cms-gov/refs/heads/main/openapi/cms-gov-bfd-openapi.yml
- filename: cms-gov-marketplace-openapi.yml
  format: yaml
  label: CMS Marketplace API
  slug: marketplace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cms-gov/refs/heads/main/openapi/cms-gov-marketplace-openapi.yml
- filename: cms-gov-open-data-openapi.yml
  format: yaml
  label: CMS Open Data API (data.cms.gov)
  slug: data-cms-gov-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cms-gov/refs/heads/main/openapi/cms-gov-open-data-openapi.yml
- filename: cms-gov-provider-data-openapi.yml
  format: yaml
  label: CMS Provider Data Catalog API
  slug: provider-data-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cms-gov/refs/heads/main/openapi/cms-gov-provider-data-openapi.yml
- filename: cms-gov-qpp-openapi.yml
  format: yaml
  label: CMS Quality Payment Program API
  slug: quality-payment-program-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cms-gov/refs/heads/main/openapi/cms-gov-qpp-openapi.yml
- filename: cms-gov-mcd-openapi.yml
  format: yaml
  label: CMS Medicare Coverage Database API
  slug: medicare-coverage-database-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cms-gov/refs/heads/main/openapi/cms-gov-mcd-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: cms.gov
  spf: true
hosts:
- cert_expires: Dec 14 23:59:59 2026 GMT
  host: www.cms.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 21 23:59:59 2026 GMT
  host: developer.cms.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 22 23:59:59 2027 GMT
  host: bluebutton.cms.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cms Gov Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CMS — Centers for Medicare & Medicaid Services, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: CMS — Centers for Medicare & Medicaid Services
provider_slug: cms-gov
slug: cms-gov-domain-security
source_filename: cms-gov-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cms.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 14 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.cms.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 21 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: bluebutton.cms.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 22 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cms.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cms-gov/refs/heads/main/security/cms-gov-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Healthcare
- Medicare
- Medicaid
- FHIR
- Bulk Data
- Open Data
- Government
- Federal
- Claims
- Insurance
- ACA
- Marketplace
- Quality
---
