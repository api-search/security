---
api_specs:
- filename: cofferdock-com-account-api-openapi.yml
  format: yaml
  label: Cofferdock Account API
  slug: cofferdock-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cofferdock-com/openapi/cofferdock-com-account-api-openapi.yml
- filename: cofferdock-com-data-api-openapi.yml
  format: yaml
  label: Cofferdock Data API
  slug: cofferdock-com-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cofferdock-com/openapi/cofferdock-com-data-api-openapi.yml
- filename: cofferdock-com-documents-api-openapi.yml
  format: yaml
  label: Cofferdock Documents API
  slug: cofferdock-com-documents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cofferdock-com/openapi/cofferdock-com-documents-api-openapi.yml
- filename: cofferdock-com-files-api-openapi.yml
  format: yaml
  label: Cofferdock Files API
  slug: cofferdock-com-files-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cofferdock-com/openapi/cofferdock-com-files-api-openapi.yml
- filename: cofferdock-com-images-api-openapi.yml
  format: yaml
  label: Cofferdock Images API
  slug: cofferdock-com-images-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cofferdock-com/openapi/cofferdock-com-images-api-openapi.yml
- filename: cofferdock-com-pdf-api-openapi.yml
  format: yaml
  label: Cofferdock PDF API
  slug: cofferdock-com-pdf-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cofferdock-com/openapi/cofferdock-com-pdf-api-openapi.yml
- filename: cofferdock-com-validation-api-openapi.yml
  format: yaml
  label: Cofferdock Validation API
  slug: cofferdock-com-validation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cofferdock-com/openapi/cofferdock-com-validation-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cofferdock.com
  spf: true
hosts:
- cert_expires: Dec 26 22:18:24 2026 GMT
  host: cofferdock.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cofferdock Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cofferdock, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Cofferdock
provider_slug: cofferdock-com
slug: cofferdock-com-domain-security
source_filename: cofferdock-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cofferdock.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 22:18:24 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cofferdock.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/cofferdock-com/security/cofferdock-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- QR Codes
- Screenshots
- Automation
---
