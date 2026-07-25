---
api_specs:
- filename: redfin-csv-export-api-openapi.yml
  format: yaml
  label: Redfin CSV Export API
  slug: redfin-csv-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/redfin/refs/heads/main/openapi/redfin-csv-export-api-openapi.yml
- filename: redfin-market-tracker-api-openapi.yml
  format: yaml
  label: Redfin Market Tracker API
  slug: redfin-market-tracker-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/redfin/refs/heads/main/openapi/redfin-market-tracker-api-openapi.yml
- filename: redfin-market-trends-api-openapi.yml
  format: yaml
  label: Redfin Market Trends API
  slug: redfin-market-trends-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/redfin/refs/heads/main/openapi/redfin-market-trends-api-openapi.yml
- filename: redfin-neighborhood-api-openapi.yml
  format: yaml
  label: Redfin Neighborhood API
  slug: redfin-neighborhood-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/redfin/refs/heads/main/openapi/redfin-neighborhood-api-openapi.yml
- filename: redfin-property-details-api-openapi.yml
  format: yaml
  label: Redfin Property Details API
  slug: redfin-property-details-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/redfin/refs/heads/main/openapi/redfin-property-details-api-openapi.yml
- filename: redfin-search-api-openapi.yml
  format: yaml
  label: Redfin Search API
  slug: redfin-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/redfin/refs/heads/main/openapi/redfin-search-api-openapi.yml
- filename: redfin-valuation-api-openapi.yml
  format: yaml
  label: Redfin Valuation API
  slug: redfin-valuation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/redfin/refs/heads/main/openapi/redfin-valuation-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: redfin.com
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: amazonaws.com
  spf: true
hosts:
- cert_expires: Nov 21 23:59:59 2026 GMT
  host: www.redfin.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 30 23:59:59 2026 GMT
  host: redfin-public-data.s3.us-west-2.amazonaws.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Redfin Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Redfin, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: Redfin
provider_slug: redfin
slug: redfin-domain-security
source_filename: redfin-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.redfin.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 21 23:59:59 2026 GMT\n  hsts: false\n- host: redfin-public-data.s3.us-west-2.amazonaws.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 30 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: redfin.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n- domain: amazonaws.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/redfin/refs/heads/main/security/redfin-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- CSV Export
- GIS
- Home Values
- Housing Market
- Listings
- Property Data
- Real Estate
---
