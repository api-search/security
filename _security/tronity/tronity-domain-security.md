---
api_specs:
- filename: tronity-openapi.yml
  format: yaml
  label: TRONITY Vehicles API
  slug: tronity-vehicles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tronity/refs/heads/main/openapi/tronity-openapi.yml
- filename: tronity-openapi.yml
  format: yaml
  label: TRONITY Vehicle Data API
  slug: tronity-vehicle-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tronity/refs/heads/main/openapi/tronity-openapi.yml
- filename: tronity-openapi.yml
  format: yaml
  label: TRONITY Charging & Battery API
  slug: tronity-charging-battery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tronity/refs/heads/main/openapi/tronity-openapi.yml
- filename: tronity-openapi.yml
  format: yaml
  label: TRONITY Commands API
  slug: tronity-commands-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tronity/refs/heads/main/openapi/tronity-openapi.yml
- filename: tronity-openapi.yml
  format: yaml
  label: TRONITY Webhooks API
  slug: tronity-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tronity/refs/heads/main/openapi/tronity-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: tronity.tech
  spf: true
hosts:
- cert_expires: Sep 17 22:55:38 2026 GMT
  host: www.tronity.tech
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 05:31:07 2026 GMT
  host: app.tronity.tech
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 17 22:55:38 2026 GMT
  host: api.tronity.tech
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tronity Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TRONITY, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: TRONITY
provider_slug: tronity
slug: tronity-domain-security
source_filename: tronity-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tronity.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 22:55:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.tronity.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 05:31:07 2026 GMT\n  hsts: false\n- host: api.tronity.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 22:55:38 2026 GMT\n  hsts: null\ndomains:\n- domain: tronity.tech\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tronity/refs/heads/main/security/tronity-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Connected Car
- EV
- Telematics
- Fleet
- Vehicle Data
---
