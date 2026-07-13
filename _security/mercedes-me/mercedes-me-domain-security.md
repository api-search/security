---
api_specs:
- filename: mercedes-me-configurator-api-openapi.yml
  format: yaml
  label: Mercedes-Benz Car Configurator API
  slug: mercedes-me-car-configurator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercedes-me/refs/heads/main/openapi/mercedes-me-configurator-api-openapi.yml
- filename: mercedes-me-dealer-api-openapi.yml
  format: yaml
  label: Mercedes-Benz Dealer API
  slug: mercedes-me-dealer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercedes-me/refs/heads/main/openapi/mercedes-me-dealer-api-openapi.yml
- filename: mercedes-me-vehicle-images-api-openapi.yml
  format: yaml
  label: Mercedes-Benz Vehicle Images API
  slug: mercedes-me-vehicle-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercedes-me/refs/heads/main/openapi/mercedes-me-vehicle-images-api-openapi.yml
- filename: mercedes-me-remote-diagnostic-support-api-openapi.yml
  format: yaml
  label: Mercedes-Benz Remote Diagnostic Support API
  slug: mercedes-me-remote-diagnostic-support-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercedes-me/refs/heads/main/openapi/mercedes-me-remote-diagnostic-support-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mercedes-benz.com
  spf: true
hosts:
- cert_expires: Aug 24 07:24:23 2026 GMT
  host: developer.mercedes-benz.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  7 23:59:59 2027 GMT
  host: api.mercedes-benz.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mercedes Me Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mercedes-Benz Mercedes me, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Mercedes-Benz Mercedes me
provider_slug: mercedes-me
slug: mercedes-me-domain-security
source_filename: mercedes-me-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.mercedes-benz.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 07:24:23 2026 GMT\n  hsts: false\n- host: api.mercedes-benz.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: mercedes-benz.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mercedes-me/refs/heads/main/security/mercedes-me-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Automotive
- Connected Car
- Connected Vehicle
- Daimler
- Fleet Management
- Mercedes me
- Mercedes-Benz
- OEM
- Telematics
- Vehicle Data
---
