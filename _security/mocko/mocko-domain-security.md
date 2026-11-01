---
api_specs:
- filename: mocko-mocko-api-api-openapi.yml
  format: yaml
  label: Mocko API
  slug: mocko-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mocko/openapi/mocko-mocko-api-api-openapi.yml
- filename: mocko-core-openapi-generated.yml
  format: yaml
  label: Mocko core API
  slug: core-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mocko/openapi/_ae-authored/mocko-core-openapi-generated.yml
- filename: mocko-creating-mocks-openapi-generated.yml
  format: yaml
  label: Mocko creating mocks API
  slug: creating-mocks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mocko/openapi/_ae-authored/mocko-creating-mocks-openapi-generated.yml
- filename: mocko-recipes-openapi-generated.yml
  format: yaml
  label: Mocko Recipes Overview API
  slug: recipes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mocko/openapi/_ae-authored/mocko-recipes-openapi-generated.yml
- filename: mocko-v1-openapi-generated.yml
  format: yaml
  label: Mocko Legacy v1 docs API
  slug: v1-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mocko/openapi/_ae-authored/mocko-v1-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: mocko.dev
  spf: true
hosts:
- cert_expires: Nov 22 10:14:20 2026 GMT
  host: mocko.dev
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Mocko Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mocko, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Mocko
provider_slug: mocko
slug: mocko-domain-security
source_filename: mocko-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mocko.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 22 10:14:20 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: mocko.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/mocko/security/mocko-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- API Mocking
- Development Tools
- Testing
- Collaboration
---
