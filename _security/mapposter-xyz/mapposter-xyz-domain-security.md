---
api_specs:
- filename: mapposter-xyz-checkout-api-openapi.yml
  format: yaml
  label: MapPoster Checkout API
  slug: mapposter-xyz-checkout-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mapposter-xyz/openapi/mapposter-xyz-checkout-api-openapi.yml
- filename: mapposter-xyz-health-api-openapi.yml
  format: yaml
  label: MapPoster Health API
  slug: mapposter-xyz-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mapposter-xyz/openapi/mapposter-xyz-health-api-openapi.yml
- filename: mapposter-xyz-key-api-openapi.yml
  format: yaml
  label: MapPoster Key API
  slug: mapposter-xyz-key-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mapposter-xyz/openapi/mapposter-xyz-key-api-openapi.yml
- filename: mapposter-xyz-keys-api-openapi.yml
  format: yaml
  label: MapPoster Keys API
  slug: mapposter-xyz-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mapposter-xyz/openapi/mapposter-xyz-keys-api-openapi.yml
- filename: mapposter-xyz-me-api-openapi.yml
  format: yaml
  label: MapPoster Me API
  slug: mapposter-xyz-me-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mapposter-xyz/openapi/mapposter-xyz-me-api-openapi.yml
- filename: mapposter-xyz-render-api-openapi.yml
  format: yaml
  label: MapPoster Render API
  slug: mapposter-xyz-render-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mapposter-xyz/openapi/mapposter-xyz-render-api-openapi.yml
- filename: mapposter-xyz-verify-api-openapi.yml
  format: yaml
  label: MapPoster Verify API
  slug: mapposter-xyz-verify-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mapposter-xyz/openapi/mapposter-xyz-verify-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: mapposter.xyz
  spf: true
hosts:
- cert_expires: Dec 31 00:15:14 2026 GMT
  host: mapposter.xyz
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: MapPoster Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MapPoster, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: MapPoster
provider_slug: mapposter-xyz
slug: mapposter-xyz-domain-security
source_filename: mapposter-xyz-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mapposter.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 00:15:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: mapposter.xyz\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/mapposter-xyz/security/mapposter-xyz-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Mapping
- Design
- E-Commerce
- AI Integration
- OpenStreetMap
---
