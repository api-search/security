---
api_specs:
- filename: smartcar-charging-api-openapi.yml
  format: yaml
  label: Smartcar Charging API
  slug: smartcar-charging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartcar/refs/heads/main/openapi/smartcar-charging-api-openapi.yml
- filename: smartcar-connections-api-openapi.yml
  format: yaml
  label: Smartcar Connections API
  slug: smartcar-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartcar/refs/heads/main/openapi/smartcar-connections-api-openapi.yml
- filename: smartcar-navigation-api-openapi.yml
  format: yaml
  label: Smartcar Navigation API
  slug: smartcar-navigation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartcar/refs/heads/main/openapi/smartcar-navigation-api-openapi.yml
- filename: smartcar-security-api-openapi.yml
  format: yaml
  label: Smartcar Security API
  slug: smartcar-security-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartcar/refs/heads/main/openapi/smartcar-security-api-openapi.yml
- filename: smartcar-vehicle-data-api-openapi.yml
  format: yaml
  label: Smartcar Vehicle Data API
  slug: smartcar-vehicle-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartcar/refs/heads/main/openapi/smartcar-vehicle-data-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: smartcar.com
  spf: true
hosts:
- cert_expires: Aug 28 05:34:35 2026 GMT
  host: smartcar.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 23:59:59 2026 GMT
  host: vehicle.api.smartcar.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 23:59:59 2026 GMT
  host: management.api.smartcar.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Smartcar Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Smartcar, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Smartcar
provider_slug: smartcar
slug: smartcar-domain-security
source_filename: smartcar-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: smartcar.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 05:34:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: vehicle.api.smartcar.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 23:59:59 2026 GMT\n  hsts: null\n- host: management.api.smartcar.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: smartcar.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/smartcar/refs/heads/main/security/smartcar-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Automotive
- Connected Vehicles
- IoT
- Mobility
- Fleet Management
- EV Management
- Telematics
---
