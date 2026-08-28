---
api_specs:
- filename: mercedes-me-components-api-openapi.yml
  format: yaml
  label: Mercedes-Benz Mercedes me Components API
  slug: mercedes-me-components-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercedes-me/refs/heads/main/openapi/mercedes-me-components-api-openapi.yml
- filename: mercedes-me-configurations-api-openapi.yml
  format: yaml
  label: Mercedes-Benz Mercedes me Configurations API
  slug: mercedes-me-configurations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercedes-me/refs/heads/main/openapi/mercedes-me-configurations-api-openapi.yml
- filename: mercedes-me-dealer-search-api-openapi.yml
  format: yaml
  label: Mercedes-Benz Mercedes me Dealer search API
  slug: mercedes-me-dealer-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercedes-me/refs/heads/main/openapi/mercedes-me-dealer-search-api-openapi.yml
- filename: mercedes-me-diagnostic-trouble-code-dtc-snapshots-api-openapi.yml
  format: yaml
  label: Mercedes-Benz Mercedes me Diagnostic Trouble Code (DTC) Snapshots API
  slug: mercedes-me-diagnostic-trouble-code-dtc-snapshots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercedes-me/refs/heads/main/openapi/mercedes-me-diagnostic-trouble-code-dtc-snapshots-api-openapi.yml
- filename: mercedes-me-diagnostic-trouble-codes-dtc-s-api-openapi.yml
  format: yaml
  label: Mercedes-Benz Mercedes me Diagnostic Trouble Codes (DTC's) API
  slug: mercedes-me-diagnostic-trouble-codes-dtc-s-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercedes-me/refs/heads/main/openapi/mercedes-me-diagnostic-trouble-codes-dtc-s-api-openapi.yml
- filename: mercedes-me-electronical-control-units-ecu-s-api-openapi.yml
  format: yaml
  label: Mercedes-Benz Mercedes me Electronical Control Units (ECU's) API
  slug: mercedes-me-electronical-control-units-ecu-s-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercedes-me/refs/heads/main/openapi/mercedes-me-electronical-control-units-ecu-s-api-openapi.yml
- filename: mercedes-me-images-api-openapi.yml
  format: yaml
  label: Mercedes-Benz Mercedes me Images API
  slug: mercedes-me-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercedes-me/refs/heads/main/openapi/mercedes-me-images-api-openapi.yml
- filename: mercedes-me-perspectives-api-openapi.yml
  format: yaml
  label: Mercedes-Benz Mercedes me Perspectives API
  slug: mercedes-me-perspectives-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercedes-me/refs/heads/main/openapi/mercedes-me-perspectives-api-openapi.yml
- filename: mercedes-me-references-api-openapi.yml
  format: yaml
  label: Mercedes-Benz Mercedes me References API
  slug: mercedes-me-references-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercedes-me/refs/heads/main/openapi/mercedes-me-references-api-openapi.yml
- filename: mercedes-me-resources-api-openapi.yml
  format: yaml
  label: Mercedes-Benz Mercedes me Resources API
  slug: mercedes-me-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercedes-me/refs/heads/main/openapi/mercedes-me-resources-api-openapi.yml
- filename: mercedes-me-saved-configurations-api-openapi.yml
  format: yaml
  label: Mercedes-Benz Mercedes me Saved configurations API
  slug: mercedes-me-saved-configurations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercedes-me/refs/heads/main/openapi/mercedes-me-saved-configurations-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mercedes-benz.com
  spf: true
hosts:
- cert_expires: Oct 23 06:26:18 2026 GMT
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
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.mercedes-benz.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 06:26:18 2026 GMT\n  hsts: false\n- host: api.mercedes-benz.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: mercedes-benz.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
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
