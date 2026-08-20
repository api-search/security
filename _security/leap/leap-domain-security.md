---
api_specs:
- filename: leap-create-meters-api-openapi.yml
  format: yaml
  label: Leap create meters API
  slug: leap-create-meters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leap/refs/heads/main/openapi/leap-create-meters-api-openapi.yml
- filename: leap-group-dispatches-api-openapi.yml
  format: yaml
  label: Leap group-dispatches API
  slug: leap-group-dispatches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leap/refs/heads/main/openapi/leap-group-dispatches-api-openapi.yml
- filename: leap-meter-details-api-openapi.yml
  format: yaml
  label: Leap Meter Details API
  slug: leap-meter-details-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leap/refs/heads/main/openapi/leap-meter-details-api-openapi.yml
- filename: leap-meter-dispatches-api-openapi.yml
  format: yaml
  label: Leap meter-dispatches API
  slug: leap-meter-dispatches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leap/refs/heads/main/openapi/leap-meter-dispatches-api-openapi.yml
- filename: leap-meter-enrollment-api-openapi.yml
  format: yaml
  label: Leap meter enrollment API
  slug: leap-meter-enrollment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leap/refs/heads/main/openapi/leap-meter-enrollment-api-openapi.yml
- filename: leap-nominations-api-openapi.yml
  format: yaml
  label: Leap nominations API
  slug: leap-nominations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leap/refs/heads/main/openapi/leap-nominations-api-openapi.yml
- filename: leap-performance-api-openapi.yml
  format: yaml
  label: Leap performance API
  slug: leap-performance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leap/refs/heads/main/openapi/leap-performance-api-openapi.yml
- filename: leap-provisional-assets-api-openapi.yml
  format: yaml
  label: Leap provisional assets API
  slug: leap-provisional-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leap/refs/heads/main/openapi/leap-provisional-assets-api-openapi.yml
- filename: leap-revenue-api-openapi.yml
  format: yaml
  label: Leap revenue API
  slug: leap-revenue-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leap/refs/heads/main/openapi/leap-revenue-api-openapi.yml
- filename: leap-webhooks-api-openapi.yml
  format: yaml
  label: Leap webhooks API
  slug: leap-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leap/refs/heads/main/openapi/leap-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: leap.energy
  spf: true
hosts:
- cert_expires: Oct 10 08:51:23 2026 GMT
  host: www.leap.energy
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 16:10:59 2026 GMT
  host: developer.leap.energy
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  7 23:59:59 2026 GMT
  host: api.leap.energy
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Leap Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Leap, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Leap
provider_slug: leap
slug: leap-domain-security
source_filename: leap-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.leap.energy\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 08:51:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.leap.energy\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 16:10:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.leap.energy\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov  7 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: leap.energy\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/leap/refs/heads/main/security/leap-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Energy
- Electricity
- Virtual Power Plant
- Demand Response
- Distributed Energy Resources
- Grid Services
- Energy Markets
- Battery Storage
- EV Charging
- Smart Buildings
- Metering
- Webhook
- Climate Tech
---
