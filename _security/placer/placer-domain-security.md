---
api_specs:
- filename: placer-account-info-api-openapi.yml
  format: yaml
  label: Placer Account Info API
  slug: placer-account-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/placer/refs/heads/main/openapi/placer-account-info-api-openapi.yml
- filename: placer-loyalty-reports-api-openapi.yml
  format: yaml
  label: Placer Loyalty Reports API
  slug: placer-loyalty-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/placer/refs/heads/main/openapi/placer-loyalty-reports-api-openapi.yml
- filename: placer-manage-pois-api-openapi.yml
  format: yaml
  label: Placer Manage POIs API
  slug: placer-manage-pois-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/placer/refs/heads/main/openapi/placer-manage-pois-api-openapi.yml
- filename: placer-ranking-reports-api-openapi.yml
  format: yaml
  label: Placer Ranking Reports API
  slug: placer-ranking-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/placer/refs/heads/main/openapi/placer-ranking-reports-api-openapi.yml
- filename: placer-retail-sales-reports-api-openapi.yml
  format: yaml
  label: Placer Retail Sales Reports API
  slug: placer-retail-sales-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/placer/refs/heads/main/openapi/placer-retail-sales-reports-api-openapi.yml
- filename: placer-trade-area-reports-api-openapi.yml
  format: yaml
  label: Placer Trade Area Reports API
  slug: placer-trade-area-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/placer/refs/heads/main/openapi/placer-trade-area-reports-api-openapi.yml
- filename: placer-visitor-journey-reports-api-openapi.yml
  format: yaml
  label: Placer Visitor Journey Reports API
  slug: placer-visitor-journey-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/placer/refs/heads/main/openapi/placer-visitor-journey-reports-api-openapi.yml
- filename: placer-visits-reports-api-openapi.yml
  format: yaml
  label: Placer Visits Reports API
  slug: placer-visits-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/placer/refs/heads/main/openapi/placer-visits-reports-api-openapi.yml
description: ''
domains:
- caa:
  - 0 contactemail "admin@placer.ai"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: placer.ai
  spf: true
hosts:
- cert_expires: Oct  2 09:41:26 2026 GMT
  host: placer.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 23 08:43:21 2026 GMT
  host: papi.placer.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Placer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Placer, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Placer
provider_slug: placer
slug: placer-domain-security
source_filename: placer-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: placer.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 09:41:26 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: papi.placer.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 08:43:21 2026 GMT\n  hsts: null\ndomains:\n- domain: placer.ai\n  dnssec: false\n  caa:\n  - 0 contactemail \"admin@placer.ai\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/placer/refs/heads/main/security/placer-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Location Analytics
- Foot Traffic
- Geospatial
- Retail Analytics
- Real Estate
- Consumer Insights
- Data
---
