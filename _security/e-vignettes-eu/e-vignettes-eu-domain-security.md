---
api_specs:
- filename: e-vignettes-eu-countries-api-openapi.yml
  format: yaml
  label: Vignette ID Countries API
  slug: e-vignettes-eu-countries-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/e-vignettes-eu/openapi/e-vignettes-eu-countries-api-openapi.yml
- filename: e-vignettes-eu-products-api-openapi.yml
  format: yaml
  label: Vignette ID Products API
  slug: e-vignettes-eu-products-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/e-vignettes-eu/openapi/e-vignettes-eu-products-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: e-vignettes.eu
  spf: false
hosts:
- cert_expires: Dec 19 21:45:07 2026 GMT
  host: e-vignettes.eu
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: E Vignettes Eu Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vignette ID, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Vignette ID
provider_slug: e-vignettes-eu
slug: e-vignettes-eu-domain-security
source_filename: e-vignettes-eu-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: e-vignettes.eu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 21:45:07 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: e-vignettes.eu\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/e-vignettes-eu/security/e-vignettes-eu-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Transportation
- Payments
- Europe
- Digital
---
