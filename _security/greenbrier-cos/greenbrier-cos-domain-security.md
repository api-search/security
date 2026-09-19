---
api_specs:
- filename: greenbrier-cos-catalog-api-openapi.yml
  format: yaml
  label: Greenbrier Companies Catalog API
  slug: greenbrier-cos-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greenbrier-cos/refs/heads/main/openapi/greenbrier-cos-catalog-api-openapi.yml
- filename: greenbrier-cos-discovery-api-openapi.yml
  format: yaml
  label: Greenbrier Companies Discovery API
  slug: greenbrier-cos-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greenbrier-cos/refs/heads/main/openapi/greenbrier-cos-discovery-api-openapi.yml
- filename: greenbrier-cos-export-api-openapi.yml
  format: yaml
  label: Greenbrier Companies Export API
  slug: greenbrier-cos-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greenbrier-cos/refs/heads/main/openapi/greenbrier-cos-export-api-openapi.yml
- filename: greenbrier-cos-gauge-tables-api-openapi.yml
  format: yaml
  label: Greenbrier Companies Gauge Tables API
  slug: greenbrier-cos-gauge-tables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greenbrier-cos/refs/heads/main/openapi/greenbrier-cos-gauge-tables-api-openapi.yml
- filename: greenbrier-cos-pages-api-openapi.yml
  format: yaml
  label: Greenbrier Companies Pages API
  slug: greenbrier-cos-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greenbrier-cos/refs/heads/main/openapi/greenbrier-cos-pages-api-openapi.yml
- filename: greenbrier-cos-posts-api-openapi.yml
  format: yaml
  label: Greenbrier Companies Posts API
  slug: greenbrier-cos-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greenbrier-cos/refs/heads/main/openapi/greenbrier-cos-posts-api-openapi.yml
- filename: greenbrier-cos-products-api-openapi.yml
  format: yaml
  label: Greenbrier Companies Products API
  slug: greenbrier-cos-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greenbrier-cos/refs/heads/main/openapi/greenbrier-cos-products-api-openapi.yml
- filename: greenbrier-cos-railcars-api-openapi.yml
  format: yaml
  label: Greenbrier Companies Railcars API
  slug: greenbrier-cos-railcars-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greenbrier-cos/refs/heads/main/openapi/greenbrier-cos-railcars-api-openapi.yml
- filename: greenbrier-cos-reporting-marks-api-openapi.yml
  format: yaml
  label: Greenbrier Companies Reporting Marks API
  slug: greenbrier-cos-reporting-marks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greenbrier-cos/refs/heads/main/openapi/greenbrier-cos-reporting-marks-api-openapi.yml
- filename: greenbrier-cos-search-api-openapi.yml
  format: yaml
  label: Greenbrier Companies Search API
  slug: greenbrier-cos-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greenbrier-cos/refs/heads/main/openapi/greenbrier-cos-search-api-openapi.yml
- filename: greenbrier-cos-taxonomies-api-openapi.yml
  format: yaml
  label: Greenbrier Companies Taxonomies API
  slug: greenbrier-cos-taxonomies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greenbrier-cos/refs/heads/main/openapi/greenbrier-cos-taxonomies-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: gbrx.com
  spf: true
hosts:
- cert_expires: Oct 25 17:00:45 2026 GMT
  host: www.gbrx.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Mar  6 23:59:59 2027 GMT
  host: tankcar.gbrx.com
  hsts: true
  hsts_max_age: 157680000
  https: true
  tls_version: TLSv1.2
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Greenbrier Cos Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Greenbrier Companies, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Greenbrier Companies
provider_slug: greenbrier-cos
slug: greenbrier-cos-domain-security
source_filename: greenbrier-cos-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.gbrx.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 25 17:00:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: tankcar.gbrx.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar  6 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 157680000\ndomains:\n- domain: gbrx.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/greenbrier-cos/refs/heads/main/security/greenbrier-cos-domain-security.yml
summary_line: TLSv1.2 · HSTS · DNSSEC · DMARC
tags:
- Rail
- Railcars
- Freight
- Transportation
- Manufacturing
- Leasing
- Logistics
- Tank Cars
- Gauge Tables
- Aftermarket Parts
- Content
- Commerce
---
