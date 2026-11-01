---
api_specs:
- filename: sellfy-content-api-openapi.yml
  format: yaml
  label: Sellfy Content API
  slug: sellfy-content-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sellfy/openapi/sellfy-content-api-openapi.yml
- filename: sellfy-discovery-api-openapi.yml
  format: yaml
  label: Sellfy Discovery API
  slug: sellfy-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sellfy/openapi/sellfy-discovery-api-openapi.yml
- filename: sellfy-feeds-api-openapi.yml
  format: yaml
  label: Sellfy Feeds API
  slug: sellfy-feeds-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sellfy/openapi/sellfy-feeds-api-openapi.yml
- filename: sellfy-licenses-api-openapi.yml
  format: yaml
  label: Sellfy Licenses API
  slug: sellfy-licenses-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sellfy/openapi/sellfy-licenses-api-openapi.yml
- filename: sellfy-ping-api-openapi.yml
  format: yaml
  label: Sellfy Ping API
  slug: sellfy-ping-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sellfy/openapi/sellfy-ping-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sellfy.com
  spf: true
hosts:
- cert_expires: Jan 10 14:46:50 2027 GMT
  host: sellfy.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Sellfy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sellfy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Sellfy
provider_slug: sellfy
slug: sellfy-domain-security
source_filename: sellfy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sellfy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 14:46:50 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: sellfy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/sellfy/security/sellfy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- e-commerce
- digital-products
- SaaS
- payments
- creators
---
