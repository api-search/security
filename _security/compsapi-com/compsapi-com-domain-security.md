---
api_specs:
- filename: compsapi-com-comps-api-openapi.yml
  format: yaml
  label: compsapi-com Comps API
  slug: compsapi-com-comps-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compsapi-com/openapi/compsapi-com-comps-api-openapi.yml
- filename: compsapi-com-health-api-openapi.yml
  format: yaml
  label: compsapi-com Health API
  slug: compsapi-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compsapi-com/openapi/compsapi-com-health-api-openapi.yml
- filename: compsapi-com-sold-api-openapi.yml
  format: yaml
  label: compsapi-com Sold API
  slug: compsapi-com-sold-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compsapi-com/openapi/compsapi-com-sold-api-openapi.yml
- filename: compsapi-com-usage-api-openapi.yml
  format: yaml
  label: compsapi-com Usage API
  slug: compsapi-com-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compsapi-com/openapi/compsapi-com-usage-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: false
  dnssec: false
  domain: compsapi.com
  spf: false
hosts:
- cert_expires: Jan  5 22:00:32 2027 GMT
  host: compsapi.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Compsapi Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for compsapi-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: compsapi-com
provider_slug: compsapi-com
slug: compsapi-com-domain-security
source_filename: compsapi-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: compsapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 22:00:32 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: compsapi.com\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/compsapi-com/security/compsapi-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- eBay
- Data
- Pricing
- Marketplace
---
