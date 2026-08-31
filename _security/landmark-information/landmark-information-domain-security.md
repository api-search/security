---
api_specs:
- filename: landmark-information-activities-api-openapi.yml
  format: yaml
  label: Landmark Information Group Activities API
  slug: landmark-information-activities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/landmark-information/refs/heads/main/openapi/landmark-information-activities-api-openapi.yml
- filename: landmark-information-cases-api-openapi.yml
  format: yaml
  label: Landmark Information Group Cases API
  slug: landmark-information-cases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/landmark-information/refs/heads/main/openapi/landmark-information-cases-api-openapi.yml
- filename: landmark-information-document-vaults-api-openapi.yml
  format: yaml
  label: Landmark Information Group Document Vaults API
  slug: landmark-information-document-vaults-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/landmark-information/refs/heads/main/openapi/landmark-information-document-vaults-api-openapi.yml
- filename: landmark-information-documents-api-openapi.yml
  format: yaml
  label: Landmark Information Group Documents API
  slug: landmark-information-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/landmark-information/refs/heads/main/openapi/landmark-information-documents-api-openapi.yml
- filename: landmark-information-milestones-api-openapi.yml
  format: yaml
  label: Landmark Information Group Milestones API
  slug: landmark-information-milestones-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/landmark-information/refs/heads/main/openapi/landmark-information-milestones-api-openapi.yml
- filename: landmark-information-order-experience-api-api-openapi.yml
  format: yaml
  label: Landmark Information Group Order Experience API
  slug: landmark-information-order-experience-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/landmark-information/refs/heads/main/openapi/landmark-information-order-experience-api-api-openapi.yml
- filename: landmark-information-quotes-api-openapi.yml
  format: yaml
  label: Landmark Information Group Quotes API
  slug: landmark-information-quotes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/landmark-information/refs/heads/main/openapi/landmark-information-quotes-api-openapi.yml
- filename: landmark-information-transaction-requests-api-openapi.yml
  format: yaml
  label: Landmark Information Group Transaction Requests API
  slug: landmark-information-transaction-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/landmark-information/refs/heads/main/openapi/landmark-information-transaction-requests-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: landmark.co.uk
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: landmarkcloudservices.com
  spf: true
hosts:
- cert_expires: Sep 15 06:16:41 2026 GMT
  host: www.landmark.co.uk
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 10 23:59:59 2027 GMT
  host: www.landmarkcloudservices.com
  hsts: true
  hsts_max_age: 10886400
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 27 23:59:59 2027 GMT
  host: api.landmarkcloudservices.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Landmark Information Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Landmark Information Group, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Landmark Information Group
provider_slug: landmark-information
slug: landmark-information-domain-security
source_filename: landmark-information-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.landmark.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 06:16:41 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: www.landmarkcloudservices.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 10886400\n- host: api.landmarkcloudservices.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 27 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: landmark.co.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: landmarkcloudservices.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/landmark-information/refs/heads/main/security/landmark-information-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Real-Estate
- United Kingdom
- PropTech
- Property Data
- Conveyancing
- Land Registry
- Geospatial
- Valuation
- Anti-Money Laundering
- Planning Data
- Mortgage
---
