---
api_specs:
- filename: circuit-depots-api-openapi.yml
  format: yaml
  label: Circuit Depots API
  slug: circuit-depots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/circuit/refs/heads/main/openapi/circuit-depots-api-openapi.yml
- filename: circuit-drivers-api-openapi.yml
  format: yaml
  label: Circuit Drivers API
  slug: circuit-drivers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/circuit/refs/heads/main/openapi/circuit-drivers-api-openapi.yml
- filename: circuit-live-plans-api-openapi.yml
  format: yaml
  label: Circuit Live Plans API
  slug: circuit-live-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/circuit/refs/heads/main/openapi/circuit-live-plans-api-openapi.yml
- filename: circuit-live-stops-api-openapi.yml
  format: yaml
  label: Circuit Live Stops API
  slug: circuit-live-stops-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/circuit/refs/heads/main/openapi/circuit-live-stops-api-openapi.yml
- filename: circuit-members-api-openapi.yml
  format: yaml
  label: Circuit Members API
  slug: circuit-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/circuit/refs/heads/main/openapi/circuit-members-api-openapi.yml
- filename: circuit-operations-api-openapi.yml
  format: yaml
  label: Circuit Operations API
  slug: circuit-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/circuit/refs/heads/main/openapi/circuit-operations-api-openapi.yml
- filename: circuit-plans-api-openapi.yml
  format: yaml
  label: Circuit Plans API
  slug: circuit-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/circuit/refs/heads/main/openapi/circuit-plans-api-openapi.yml
- filename: circuit-routes-api-openapi.yml
  format: yaml
  label: Circuit Routes API
  slug: circuit-routes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/circuit/refs/heads/main/openapi/circuit-routes-api-openapi.yml
- filename: circuit-stops-api-openapi.yml
  format: yaml
  label: Circuit Stops API
  slug: circuit-stops-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/circuit/refs/heads/main/openapi/circuit-stops-api-openapi.yml
- filename: circuit-team-api-openapi.yml
  format: yaml
  label: Circuit Team API
  slug: circuit-team-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/circuit/refs/heads/main/openapi/circuit-team-api-openapi.yml
- filename: circuit-unassigned-stops-api-openapi.yml
  format: yaml
  label: Circuit Unassigned Stops API
  slug: circuit-unassigned-stops-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/circuit/refs/heads/main/openapi/circuit-unassigned-stops-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: spoke.com
  spf: true
hosts:
- cert_expires: Sep  9 03:23:44 2026 GMT
  host: spoke.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 01:38:55 2026 GMT
  host: developer.dispatch.spoke.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 09:24:19 2026 GMT
  host: api.spoke.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Circuit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Circuit, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Circuit
provider_slug: circuit
slug: circuit-domain-security
source_filename: circuit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: spoke.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 03:23:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.dispatch.spoke.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 01:38:55 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.spoke.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 09:24:19 2026 GMT\n  hsts: null\ndomains:\n- domain: spoke.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/circuit/refs/heads/main/security/circuit-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Delivery
- Logistics
- Last Mile
- Route Optimization
- Dispatch
- Courier
- Fleet
- Proof of Delivery
- Field Service
---
