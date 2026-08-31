---
api_specs:
- filename: reposit-power-auth-api-openapi.yml
  format: yaml
  label: Reposit Power Auth API
  slug: reposit-power-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reposit-power/refs/heads/main/openapi/reposit-power-auth-api-openapi.yml
- filename: reposit-power-battery-api-openapi.yml
  format: yaml
  label: Reposit Power Battery API
  slug: reposit-power-battery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reposit-power/refs/heads/main/openapi/reposit-power-battery-api-openapi.yml
- filename: reposit-power-curtailment-api-openapi.yml
  format: yaml
  label: Reposit Power Curtailment API
  slug: reposit-power-curtailment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reposit-power/refs/heads/main/openapi/reposit-power-curtailment-api-openapi.yml
- filename: reposit-power-deployment-api-openapi.yml
  format: yaml
  label: Reposit Power Deployment API
  slug: reposit-power-deployment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reposit-power/refs/heads/main/openapi/reposit-power-deployment-api-openapi.yml
- filename: reposit-power-dispatch-api-openapi.yml
  format: yaml
  label: Reposit Power Dispatch API
  slug: reposit-power-dispatch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reposit-power/refs/heads/main/openapi/reposit-power-dispatch-api-openapi.yml
- filename: reposit-power-inverter-api-openapi.yml
  format: yaml
  label: Reposit Power Inverter API
  slug: reposit-power-inverter-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reposit-power/refs/heads/main/openapi/reposit-power-inverter-api-openapi.yml
- filename: reposit-power-network-api-openapi.yml
  format: yaml
  label: Reposit Power Network API
  slug: reposit-power-network-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reposit-power/refs/heads/main/openapi/reposit-power-network-api-openapi.yml
- filename: reposit-power-node-api-openapi.yml
  format: yaml
  label: Reposit Power Node API
  slug: reposit-power-node-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reposit-power/refs/heads/main/openapi/reposit-power-node-api-openapi.yml
- filename: reposit-power-power-station-api-openapi.yml
  format: yaml
  label: Reposit Power Power Station API
  slug: reposit-power-power-station-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reposit-power/refs/heads/main/openapi/reposit-power-power-station-api-openapi.yml
- filename: reposit-power-solar-api-openapi.yml
  format: yaml
  label: Reposit Power Solar API
  slug: reposit-power-solar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reposit-power/refs/heads/main/openapi/reposit-power-solar-api-openapi.yml
- filename: reposit-power-users-api-openapi.yml
  format: yaml
  label: Reposit Power Users API
  slug: reposit-power-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reposit-power/refs/heads/main/openapi/reposit-power-users-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: repositpower.com
  spf: true
hosts:
- cert_expires: Sep 30 00:17:39 2026 GMT
  host: repositpower.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  5 22:00:28 2026 GMT
  host: fleet.repositpower.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 02:30:35 2026 GMT
  host: api.repositpower.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Reposit Power Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Reposit Power, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Reposit Power
provider_slug: reposit-power
slug: reposit-power-domain-security
source_filename: reposit-power-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: repositpower.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 00:17:39 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: fleet.repositpower.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 22:00:28 2026 GMT\n  hsts: false\n- host: api.repositpower.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 02:30:35 2026 GMT\n  hsts: false\ndomains:\n- domain: repositpower.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reposit-power/refs/heads/main/security/reposit-power-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Energy
- Australia
- Utilities
- Electricity
- Batteries
- DER
- Virtual Power Plant
- Demand Response
- Solar
- Grid
- Energy Markets
- Smart Metering
- Storage
- Flexibility
---
