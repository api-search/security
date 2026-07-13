---
api_specs:
- filename: enode-openapi.yml
  format: yaml
  label: Enode Users & Link API
  slug: users-link-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enode/refs/heads/main/openapi/enode-openapi.yml
- filename: enode-openapi.yml
  format: yaml
  label: Enode Vehicles API
  slug: vehicles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enode/refs/heads/main/openapi/enode-openapi.yml
- filename: enode-openapi.yml
  format: yaml
  label: Enode Chargers API
  slug: chargers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enode/refs/heads/main/openapi/enode-openapi.yml
- filename: enode-openapi.yml
  format: yaml
  label: Enode HVAC API
  slug: hvac-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enode/refs/heads/main/openapi/enode-openapi.yml
- filename: enode-openapi.yml
  format: yaml
  label: Enode Batteries & Inverters API
  slug: batteries-inverters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enode/refs/heads/main/openapi/enode-openapi.yml
- filename: enode-openapi.yml
  format: yaml
  label: Enode Smart Charging API
  slug: smart-charging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enode/refs/heads/main/openapi/enode-openapi.yml
- filename: enode-openapi.yml
  format: yaml
  label: Enode Webhooks API
  slug: webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enode/refs/heads/main/openapi/enode-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: enode.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: enode.io
  spf: false
hosts:
- cert_expires: Sep  2 13:20:53 2026 GMT
  host: www.enode.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 11 04:56:20 2026 GMT
  host: developers.enode.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 21 23:59:59 2027 GMT
  host: enode-api.production.enode.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Enode Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Enode, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Enode
provider_slug: enode
slug: enode-domain-security
source_filename: enode-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.enode.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 13:20:53 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developers.enode.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 04:56:20 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: enode-api.production.enode.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: enode.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: enode.io\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/enode/refs/heads/main/security/enode-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Energy
- Electric Vehicles
- EV Charging
- Smart Charging
- Energy Transition
---
