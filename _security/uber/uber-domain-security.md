---
api_specs:
- filename: uber-codes-api-openapi.yml
  format: yaml
  label: Uber Codes API
  slug: uber-codes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uber/refs/heads/main/openapi/uber-codes-api-openapi.yml
- filename: uber-deliveries-api-openapi.yml
  format: yaml
  label: Uber Deliveries API
  slug: uber-deliveries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uber/refs/heads/main/openapi/uber-deliveries-api-openapi.yml
- filename: uber-estimates-api-openapi.yml
  format: yaml
  label: Uber Estimates API
  slug: uber-estimates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uber/refs/heads/main/openapi/uber-estimates-api-openapi.yml
- filename: uber-locations-api-openapi.yml
  format: yaml
  label: Uber Locations API
  slug: uber-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uber/refs/heads/main/openapi/uber-locations-api-openapi.yml
- filename: uber-menus-api-openapi.yml
  format: yaml
  label: Uber Menus API
  slug: uber-menus-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uber/refs/heads/main/openapi/uber-menus-api-openapi.yml
- filename: uber-orders-api-openapi.yml
  format: yaml
  label: Uber Orders API
  slug: uber-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uber/refs/heads/main/openapi/uber-orders-api-openapi.yml
- filename: uber-organizations-api-openapi.yml
  format: yaml
  label: Uber Organizations API
  slug: uber-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uber/refs/heads/main/openapi/uber-organizations-api-openapi.yml
- filename: uber-partners-api-openapi.yml
  format: yaml
  label: Uber Partners API
  slug: uber-partners-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uber/refs/heads/main/openapi/uber-partners-api-openapi.yml
- filename: uber-places-api-openapi.yml
  format: yaml
  label: Uber Places API
  slug: uber-places-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uber/refs/heads/main/openapi/uber-places-api-openapi.yml
- filename: uber-products-api-openapi.yml
  format: yaml
  label: Uber Products API
  slug: uber-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uber/refs/heads/main/openapi/uber-products-api-openapi.yml
- filename: uber-programs-api-openapi.yml
  format: yaml
  label: Uber Programs API
  slug: uber-programs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uber/refs/heads/main/openapi/uber-programs-api-openapi.yml
- filename: uber-redemption-api-openapi.yml
  format: yaml
  label: Uber Redemption API
  slug: uber-redemption-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uber/refs/heads/main/openapi/uber-redemption-api-openapi.yml
- filename: uber-refunds-api-openapi.yml
  format: yaml
  label: Uber Refunds API
  slug: uber-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uber/refs/heads/main/openapi/uber-refunds-api-openapi.yml
- filename: uber-reporting-api-openapi.yml
  format: yaml
  label: Uber Reporting API
  slug: uber-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uber/refs/heads/main/openapi/uber-reporting-api-openapi.yml
- filename: uber-requests-api-openapi.yml
  format: yaml
  label: Uber Requests API
  slug: uber-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uber/refs/heads/main/openapi/uber-requests-api-openapi.yml
- filename: uber-riders-api-openapi.yml
  format: yaml
  label: Uber Riders API
  slug: uber-riders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uber/refs/heads/main/openapi/uber-riders-api-openapi.yml
- filename: uber-stores-api-openapi.yml
  format: yaml
  label: Uber Stores API
  slug: uber-stores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uber/refs/heads/main/openapi/uber-stores-api-openapi.yml
- filename: uber-templates-api-openapi.yml
  format: yaml
  label: Uber Templates API
  slug: uber-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uber/refs/heads/main/openapi/uber-templates-api-openapi.yml
- filename: uber-trips-api-openapi.yml
  format: yaml
  label: Uber Trips API
  slug: uber-trips-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uber/refs/heads/main/openapi/uber-trips-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: uber.com
  spf: true
hosts:
- cert_expires: Feb 16 23:59:59 2027 GMT
  host: developer.uber.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 16 23:59:59 2027 GMT
  host: api.uber.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 16 23:59:59 2027 GMT
  host: sandbox-api.uber.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Uber Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Uber, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Uber
provider_slug: uber
slug: uber-domain-security
source_filename: uber-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.uber.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 16 23:59:59 2027 GMT\n  hsts: null\n- host: api.uber.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 16 23:59:59 2027 GMT\n  hsts: null\n- host: sandbox-api.uber.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 16 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: uber.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uber/refs/heads/main/security/uber-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Ridesharing
- Rides
- Taxis
- Transportation
- Food Delivery
- Delivery
- Logistics
---
