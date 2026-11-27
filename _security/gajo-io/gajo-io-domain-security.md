---
api_specs:
- filename: gajo-io-a-b-templates-api-openapi.yml
  format: yaml
  label: Gajo A/B Templates API
  slug: gajo-io-a-b-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gajo-io/openapi/gajo-io-a-b-templates-api-openapi.yml
- filename: gajo-io-account-api-openapi.yml
  format: yaml
  label: Gajo Account API
  slug: gajo-io-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gajo-io/openapi/gajo-io-account-api-openapi.yml
- filename: gajo-io-analytics-api-openapi.yml
  format: yaml
  label: Gajo Analytics API
  slug: gajo-io-analytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gajo-io/openapi/gajo-io-analytics-api-openapi.yml
- filename: gajo-io-app-links-api-openapi.yml
  format: yaml
  label: Gajo App Links API
  slug: gajo-io-app-links-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gajo-io/openapi/gajo-io-app-links-api-openapi.yml
- filename: gajo-io-bindings-api-openapi.yml
  format: yaml
  label: Gajo Bindings API
  slug: gajo-io-bindings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gajo-io/openapi/gajo-io-bindings-api-openapi.yml
- filename: gajo-io-route-templates-api-openapi.yml
  format: yaml
  label: Gajo Route Templates API
  slug: gajo-io-route-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gajo-io/openapi/gajo-io-route-templates-api-openapi.yml
- filename: gajo-io-routing-rules-api-openapi.yml
  format: yaml
  label: Gajo Routing Rules API
  slug: gajo-io-routing-rules-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gajo-io/openapi/gajo-io-routing-rules-api-openapi.yml
- filename: gajo-io-urls-api-openapi.yml
  format: yaml
  label: Gajo URLs API
  slug: gajo-io-urls-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gajo-io/openapi/gajo-io-urls-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: gajo.io
  spf: true
hosts:
- cert_expires: Mar  9 23:59:59 2027 GMT
  host: gajo.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Gajo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gajo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Gajo
provider_slug: gajo-io
slug: gajo-io-domain-security
source_filename: gajo-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gajo.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  9 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: gajo.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/gajo-io/security/gajo-io-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- URL Shorteners
- Analytics
- Developer Tool
---
