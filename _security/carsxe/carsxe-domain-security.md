---
api_specs:
- filename: carsxe-specifications-api-openapi.yml
  format: yaml
  label: CarsXE Specifications API
  slug: carsxe-specifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/carsxe/refs/heads/main/openapi/carsxe-specifications-api-openapi.yml
- filename: carsxe-market-value-api-openapi.yml
  format: yaml
  label: CarsXE Market Value API
  slug: carsxe-market-value-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/carsxe/refs/heads/main/openapi/carsxe-market-value-api-openapi.yml
- filename: carsxe-plate-api-openapi.yml
  format: yaml
  label: CarsXE Plate Decoder API
  slug: carsxe-plate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/carsxe/refs/heads/main/openapi/carsxe-plate-api-openapi.yml
- filename: carsxe-recalls-api-openapi.yml
  format: yaml
  label: CarsXE Recalls API
  slug: carsxe-recalls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/carsxe/refs/heads/main/openapi/carsxe-recalls-api-openapi.yml
- filename: carsxe-history-api-openapi.yml
  format: yaml
  label: CarsXE History API
  slug: carsxe-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/carsxe/refs/heads/main/openapi/carsxe-history-api-openapi.yml
- filename: carsxe-images-api-openapi.yml
  format: yaml
  label: CarsXE Images API
  slug: carsxe-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/carsxe/refs/heads/main/openapi/carsxe-images-api-openapi.yml
- filename: carsxe-recognition-api-openapi.yml
  format: yaml
  label: CarsXE Recognition API
  slug: carsxe-recognition-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/carsxe/refs/heads/main/openapi/carsxe-recognition-api-openapi.yml
- filename: carsxe-year-make-model-api-openapi.yml
  format: yaml
  label: CarsXE Year Make Model API
  slug: carsxe-year-make-model-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/carsxe/refs/heads/main/openapi/carsxe-year-make-model-api-openapi.yml
- filename: carsxe-lien-theft-api-openapi.yml
  format: yaml
  label: CarsXE Lien & Theft API
  slug: carsxe-lien-theft-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/carsxe/refs/heads/main/openapi/carsxe-lien-theft-api-openapi.yml
- filename: carsxe-auth-api-openapi.yml
  format: yaml
  label: CarsXE Auth API
  slug: carsxe-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/carsxe/refs/heads/main/openapi/carsxe-auth-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: carsxe.com
  spf: true
hosts:
- cert_expires: Dec  1 03:08:59 2026 GMT
  host: carsxe.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 17 17:43:06 2026 GMT
  host: api.carsxe.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  4 21:17:59 2026 GMT
  host: mcp.carsxe.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Carsxe Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CarsXE, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: CarsXE
provider_slug: carsxe
slug: carsxe-domain-security
source_filename: carsxe-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: carsxe.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  1 03:08:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.carsxe.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 17 17:43:06 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: mcp.carsxe.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  4 21:17:59 2026 GMT\n  hsts: null\ndomains:\n- domain: carsxe.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/carsxe/refs/heads/main/security/carsxe-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Automotive
- Vehicles
- VIN
- Vehicle Data
- License Plate
- OCR
- Automobiles
- Recalls
- Market Value
- Vehicle History
- Model Context Protocol
- Agents
---
