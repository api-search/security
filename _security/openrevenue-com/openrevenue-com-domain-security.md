---
api_specs:
- filename: openrevenue-com-account-api-openapi.yml
  format: yaml
  label: OpenRevenue Account API
  slug: openrevenue-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openrevenue-com/openapi/openrevenue-com-account-api-openapi.yml
- filename: openrevenue-com-analytics-api-openapi.yml
  format: yaml
  label: OpenRevenue Analytics API
  slug: openrevenue-com-analytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openrevenue-com/openapi/openrevenue-com-analytics-api-openapi.yml
- filename: openrevenue-com-funnels-api-openapi.yml
  format: yaml
  label: OpenRevenue Funnels API
  slug: openrevenue-com-funnels-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openrevenue-com/openapi/openrevenue-com-funnels-api-openapi.yml
- filename: openrevenue-com-performance-api-openapi.yml
  format: yaml
  label: OpenRevenue Performance API
  slug: openrevenue-com-performance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openrevenue-com/openapi/openrevenue-com-performance-api-openapi.yml
- filename: openrevenue-com-visitors-api-openapi.yml
  format: yaml
  label: OpenRevenue Visitors API
  slug: openrevenue-com-visitors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openrevenue-com/openapi/openrevenue-com-visitors-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: openrevenue.com
  spf: true
hosts:
- cert_expires: Feb 10 07:43:01 2027 GMT
  host: openrevenue.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: OpenRevenue Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpenRevenue, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: OpenRevenue
provider_slug: openrevenue-com
slug: openrevenue-com-domain-security
source_filename: openrevenue-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: openrevenue.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 10 07:43:01 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: openrevenue.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/openrevenue-com/security/openrevenue-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Analytics
- Web
- Privacy
- Revenue
- Marketing
- Company
---
