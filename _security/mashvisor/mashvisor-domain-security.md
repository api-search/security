---
api_specs:
- filename: mashvisor-investment-analysis-api-openapi.yml
  format: yaml
  label: Mashvisor Investment Analysis API
  slug: mashvisor-investment-analysis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mashvisor/refs/heads/main/openapi/mashvisor-investment-analysis-api-openapi.yml
- filename: mashvisor-property-info-api-openapi.yml
  format: yaml
  label: Mashvisor Property Info API
  slug: mashvisor-property-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mashvisor/refs/heads/main/openapi/mashvisor-property-info-api-openapi.yml
- filename: mashvisor-rental-rates-api-openapi.yml
  format: yaml
  label: Mashvisor Rental Rates API
  slug: mashvisor-rental-rates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mashvisor/refs/heads/main/openapi/mashvisor-rental-rates-api-openapi.yml
- filename: mashvisor-search-api-openapi.yml
  format: yaml
  label: Mashvisor Search API
  slug: mashvisor-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mashvisor/refs/heads/main/openapi/mashvisor-search-api-openapi.yml
- filename: mashvisor-trends-api-openapi.yml
  format: yaml
  label: Mashvisor Trends API
  slug: mashvisor-trends-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mashvisor/refs/heads/main/openapi/mashvisor-trends-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: mashvisor.com
  spf: true
hosts:
- cert_expires: Sep 23 16:03:05 2026 GMT
  host: mashvisor.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mashvisor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mashvisor, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Mashvisor
provider_slug: mashvisor
slug: mashvisor-domain-security
source_filename: mashvisor-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mashvisor.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 16:03:05 2026 GMT\n  hsts: true\n  hsts_max_age: 0\ndomains:\n- domain: mashvisor.com\n  dnssec: false\n  caa:\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mashvisor/refs/heads/main/security/mashvisor-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Real-Estate
- Property Data
- Analytics
- Rentals
- Airbnb
- Investment
- MLS
- Housing
---
