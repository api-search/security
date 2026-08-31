---
api_specs:
- filename: ontario-energy-board-applications-before-the-oeb-api-openapi.yml
  format: yaml
  label: Ontario Energy Board Applications before the OEB API
  slug: ontario-energy-board-applications-before-the-oeb-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ontario-energy-board/refs/heads/main/openapi/ontario-energy-board-applications-before-the-oeb-api-openapi.yml
- filename: ontario-energy-board-current-electricity-rates-general-service-50-kw-rate-class-api-openapi.yml
  format: yaml
  label: Ontario Energy Board Current Electricity Rates (General Service < 50 kW Rate Class) API
  slug: ontario-energy-board-current-electricity-rates-general-service-50-kw-rate-class-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ontario-energy-board/refs/heads/main/openapi/ontario-energy-board-current-electricity-rates-general-service-50-kw-rate-class-api-openapi.yml
- filename: ontario-energy-board-current-electricity-rates-residential-rate-class-api-openapi.yml
  format: yaml
  label: Ontario Energy Board Current Electricity Rates (Residential Rate Class) API
  slug: ontario-energy-board-current-electricity-rates-residential-rate-class-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ontario-energy-board/refs/heads/main/openapi/ontario-energy-board-current-electricity-rates-residential-rate-class-api-openapi.yml
- filename: ontario-energy-board-current-natural-gas-rates-residential-rate-classes-api-openapi.yml
  format: yaml
  label: Ontario Energy Board Current Natural Gas Rates (Residential Rate Classes) API
  slug: ontario-energy-board-current-natural-gas-rates-residential-rate-classes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ontario-energy-board/refs/heads/main/openapi/ontario-energy-board-current-natural-gas-rates-residential-rate-classes-api-openapi.yml
- filename: ontario-energy-board-electricity-and-natural-gas-distributors-service-areas-api-openapi.yml
  format: yaml
  label: Ontario Energy Board Electricity and Natural Gas Distributors - Service Areas API
  slug: ontario-energy-board-electricity-and-natural-gas-distributors-service-areas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ontario-energy-board/refs/heads/main/openapi/ontario-energy-board-electricity-and-natural-gas-distributors-service-areas-api-openapi.yml
- filename: ontario-energy-board-electricity-distributor-complaints-received-by-the-oeb-api-openapi.yml
  format: yaml
  label: Ontario Energy Board Electricity Distributor Complaints Received by the OEB API
  slug: ontario-energy-board-electricity-distributor-complaints-received-by-the-oeb-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ontario-energy-board/refs/heads/main/openapi/ontario-energy-board-electricity-distributor-complaints-received-by-the-oeb-api-openapi.yml
- filename: ontario-energy-board-electricity-distributor-performance-scorecard-api-openapi.yml
  format: yaml
  label: Ontario Energy Board Electricity Distributor Performance – Scorecard API
  slug: ontario-energy-board-electricity-distributor-performance-scorecard-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ontario-energy-board/refs/heads/main/openapi/ontario-energy-board-electricity-distributor-performance-scorecard-api-openapi.yml
- filename: ontario-energy-board-electricity-reporting-record-keeping-requirements-rrr-section-api-openapi.yml
  format: yaml
  label: 'Ontario Energy Board Electricity Reporting & Record Keeping Requirements (RRR): Section ... API'
  slug: ontario-energy-board-electricity-reporting-record-keeping-requirements-rrr-section-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ontario-energy-board/refs/heads/main/openapi/ontario-energy-board-electricity-reporting-record-keeping-requirements-rrr-section-api-openapi.yml
- filename: ontario-energy-board-historical-regulated-price-plan-electricity-rates-api-openapi.yml
  format: yaml
  label: Ontario Energy Board Historical Regulated Price Plan Electricity Rates API
  slug: ontario-energy-board-historical-regulated-price-plan-electricity-rates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ontario-energy-board/refs/heads/main/openapi/ontario-energy-board-historical-regulated-price-plan-electricity-rates-api-openapi.yml
- filename: ontario-energy-board-licensed-market-participants-api-openapi.yml
  format: yaml
  label: Ontario Energy Board Licensed Market Participants API
  slug: ontario-energy-board-licensed-market-participants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ontario-energy-board/refs/heads/main/openapi/ontario-energy-board-licensed-market-participants-api-openapi.yml
- filename: ontario-energy-board-records-api-openapi.yml
  format: yaml
  label: Ontario Energy Board Records API
  slug: ontario-energy-board-records-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ontario-energy-board/refs/heads/main/openapi/ontario-energy-board-records-api-openapi.yml
- filename: ontario-energy-board-search-metadata-api-openapi.yml
  format: yaml
  label: Ontario Energy Board Search Metadata API
  slug: ontario-energy-board-search-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ontario-energy-board/refs/heads/main/openapi/ontario-energy-board-search-metadata-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: oeb.ca
  spf: true
hosts:
- cert_expires: Dec 27 23:59:59 2026 GMT
  host: www.oeb.ca
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  9 23:59:59 2027 GMT
  host: www.rds.oeb.ca
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ontario Energy Board Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ontario Energy Board, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Ontario Energy Board
provider_slug: ontario-energy-board
slug: ontario-energy-board-domain-security
source_filename: ontario-energy-board-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.oeb.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.rds.oeb.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  9 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: oeb.ca\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ontario-energy-board/refs/heads/main/security/ontario-energy-board-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Energy
- Canada
- Ontario
- Utilities
- Electricity
- Gas
- Green Button
- Smart Metering
- Energy Markets
- Regulator
- Open Data
- Grid
---
