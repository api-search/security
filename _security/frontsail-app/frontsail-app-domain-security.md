---
api_specs:
- filename: frontsail-app-describe-api-openapi.yml
  format: yaml
  label: FrontSail Describe API
  slug: frontsail-app-describe-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/frontsail-app/openapi/frontsail-app-describe-api-openapi.yml
- filename: frontsail-app-describe-doc-api-openapi.yml
  format: yaml
  label: FrontSail Describe Doc API
  slug: frontsail-app-describe-doc-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/frontsail-app/openapi/frontsail-app-describe-doc-api-openapi.yml
- filename: frontsail-app-describe-pdf-api-openapi.yml
  format: yaml
  label: FrontSail Describe Pdf API
  slug: frontsail-app-describe-pdf-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/frontsail-app/openapi/frontsail-app-describe-pdf-api-openapi.yml
- filename: frontsail-app-health-api-openapi.yml
  format: yaml
  label: FrontSail Health API
  slug: frontsail-app-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/frontsail-app/openapi/frontsail-app-health-api-openapi.yml
- filename: frontsail-app-render-api-openapi.yml
  format: yaml
  label: FrontSail Render API
  slug: frontsail-app-render-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/frontsail-app/openapi/frontsail-app-render-api-openapi.yml
- filename: frontsail-app-render-doc-api-openapi.yml
  format: yaml
  label: FrontSail Render Doc API
  slug: frontsail-app-render-doc-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/frontsail-app/openapi/frontsail-app-render-doc-api-openapi.yml
- filename: frontsail-app-render-pdf-api-openapi.yml
  format: yaml
  label: FrontSail Render Pdf API
  slug: frontsail-app-render-pdf-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/frontsail-app/openapi/frontsail-app-render-pdf-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: frontsail.app
  spf: false
hosts:
- cert_expires: Mar  6 23:59:59 2027 GMT
  host: frontsail.app
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: FrontSail Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FrontSail, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: FrontSail
provider_slug: frontsail-app
slug: frontsail-app-domain-security
source_filename: frontsail-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: frontsail.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  6 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: frontsail.app\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/frontsail-app/security/frontsail-app-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- FrontSail
- Artificial Intelligence
- Application
- Sites
- Waterloo
---
