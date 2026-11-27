---
api_specs:
- filename: blumee-app-catalog-api-openapi.yml
  format: yaml
  label: Blumee Catalog API
  slug: blumee-app-catalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blumee-app/openapi/blumee-app-catalog-api-openapi.yml
- filename: blumee-app-search-api-openapi.yml
  format: yaml
  label: Blumee Search API
  slug: blumee-app-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blumee-app/openapi/blumee-app-search-api-openapi.yml
- filename: blumee-app-service-api-openapi.yml
  format: yaml
  label: Blumee Service API
  slug: blumee-app-service-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blumee-app/openapi/blumee-app-service-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: blumee.app
  spf: true
hosts:
- cert_expires: Dec 13 00:17:23 2026 GMT
  host: blumee.app
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Blumee Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Blumee, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Blumee
provider_slug: blumee-app
slug: blumee-app-domain-security
source_filename: blumee-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: blumee.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 00:17:23 2026 GMT\n  hsts: false\ndomains:\n- domain: blumee.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/blumee-app/security/blumee-app-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Flower Delivery
- E-Commerce
- Germany
- Mobile App
- Online Shopping
---
