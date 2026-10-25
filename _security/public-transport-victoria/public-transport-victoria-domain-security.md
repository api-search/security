---
api_specs:
- filename: public-transport-victoria-departures-api-openapi.yml
  format: yaml
  label: Public Transport Victoria Departures API
  slug: public-transport-victoria-departures-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/public-transport-victoria/refs/heads/main/openapi/public-transport-victoria-departures-api-openapi.yml
- filename: public-transport-victoria-directions-api-openapi.yml
  format: yaml
  label: Public Transport Victoria Directions API
  slug: public-transport-victoria-directions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/public-transport-victoria/refs/heads/main/openapi/public-transport-victoria-directions-api-openapi.yml
- filename: public-transport-victoria-disruptions-api-openapi.yml
  format: yaml
  label: Public Transport Victoria Disruptions API
  slug: public-transport-victoria-disruptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/public-transport-victoria/refs/heads/main/openapi/public-transport-victoria-disruptions-api-openapi.yml
- filename: public-transport-victoria-fareestimate-api-openapi.yml
  format: yaml
  label: Public Transport Victoria Fare Estimate API
  slug: public-transport-victoria-fareestimate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/public-transport-victoria/refs/heads/main/openapi/public-transport-victoria-fareestimate-api-openapi.yml
- filename: public-transport-victoria-outlets-api-openapi.yml
  format: yaml
  label: Public Transport Victoria Outlets API
  slug: public-transport-victoria-outlets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/public-transport-victoria/refs/heads/main/openapi/public-transport-victoria-outlets-api-openapi.yml
- filename: public-transport-victoria-patterns-api-openapi.yml
  format: yaml
  label: Public Transport Victoria Patterns API
  slug: public-transport-victoria-patterns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/public-transport-victoria/refs/heads/main/openapi/public-transport-victoria-patterns-api-openapi.yml
- filename: public-transport-victoria-routes-api-openapi.yml
  format: yaml
  label: Public Transport Victoria Routes API
  slug: public-transport-victoria-routes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/public-transport-victoria/refs/heads/main/openapi/public-transport-victoria-routes-api-openapi.yml
- filename: public-transport-victoria-routetypes-api-openapi.yml
  format: yaml
  label: Public Transport Victoria Route Types API
  slug: public-transport-victoria-routetypes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/public-transport-victoria/refs/heads/main/openapi/public-transport-victoria-routetypes-api-openapi.yml
- filename: public-transport-victoria-runs-api-openapi.yml
  format: yaml
  label: Public Transport Victoria Runs API
  slug: public-transport-victoria-runs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/public-transport-victoria/refs/heads/main/openapi/public-transport-victoria-runs-api-openapi.yml
- filename: public-transport-victoria-search-api-openapi.yml
  format: yaml
  label: Public Transport Victoria Search API
  slug: public-transport-victoria-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/public-transport-victoria/refs/heads/main/openapi/public-transport-victoria-search-api-openapi.yml
- filename: public-transport-victoria-stops-api-openapi.yml
  format: yaml
  label: Public Transport Victoria Stops API
  slug: public-transport-victoria-stops-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/public-transport-victoria/refs/heads/main/openapi/public-transport-victoria-stops-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: vic.gov.au
  spf: true
hosts:
- cert_expires: Feb 10 23:59:59 2027 GMT
  host: ptv.vic.gov.au
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Public Transport Victoria Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Public Transport Victoria, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Public Transport Victoria
provider_slug: public-transport-victoria
slug: public-transport-victoria-domain-security
source_filename: public-transport-victoria-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ptv.vic.gov.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 10 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: vic.gov.au\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/public-transport-victoria/refs/heads/main/security/public-transport-victoria-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Public Transport
- Government
- Transit
- Timetables
- Australia
- Open Data
---
