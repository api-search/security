---
api_specs:
- filename: revvo-api-keys-api-openapi.yml
  format: yaml
  label: Revvo Api-keys API
  slug: revvo-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revvo/refs/heads/main/openapi/revvo-api-keys-api-openapi.yml
- filename: revvo-auth-api-openapi.yml
  format: yaml
  label: Revvo Auth API
  slug: revvo-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revvo/refs/heads/main/openapi/revvo-auth-api-openapi.yml
- filename: revvo-device-api-openapi.yml
  format: yaml
  label: Revvo Device API
  slug: revvo-device-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revvo/refs/heads/main/openapi/revvo-device-api-openapi.yml
- filename: revvo-event-api-openapi.yml
  format: yaml
  label: Revvo Event API
  slug: revvo-event-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revvo/refs/heads/main/openapi/revvo-event-api-openapi.yml
- filename: revvo-fleet-api-openapi.yml
  format: yaml
  label: Revvo Fleet API
  slug: revvo-fleet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revvo/refs/heads/main/openapi/revvo-fleet-api-openapi.yml
- filename: revvo-tire-operation-api-openapi.yml
  format: yaml
  label: Revvo Tire Operation API
  slug: revvo-tire-operation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revvo/refs/heads/main/openapi/revvo-tire-operation-api-openapi.yml
- filename: revvo-vehicle-api-openapi.yml
  format: yaml
  label: Revvo Vehicle API
  slug: revvo-vehicle-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revvo/refs/heads/main/openapi/revvo-vehicle-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: revvo.ai
  spf: true
hosts:
- cert_expires: Oct  3 23:08:27 2026 GMT
  host: revvo.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Revvo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Revvo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Revvo
provider_slug: revvo
slug: revvo-domain-security
source_filename: revvo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: revvo.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 23:08:27 2026 GMT\n  hsts: false\ndomains:\n- domain: revvo.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/revvo/refs/heads/main/security/revvo-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Fleet Management
- Transportation
- Tire Management
- TPMS
- Telematics
- IoT
- Logistics
---
