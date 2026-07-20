---
api_specs:
- filename: leap-meters-openapi-original.yml
  format: yaml
  label: Leap Meter Details API
  slug: meters
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leap/refs/heads/main/openapi/leap-meters-openapi-original.yml
- filename: leap-enrollments-openapi-original.yml
  format: yaml
  label: Leap Meter Enrollment API
  slug: enrollments
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leap/refs/heads/main/openapi/leap-enrollments-openapi-original.yml
- filename: leap-create-meters-openapi-original.yml
  format: yaml
  label: Leap Create Meters API
  slug: create-meters
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leap/refs/heads/main/openapi/leap-create-meters-openapi-original.yml
- filename: leap-dispatching-openapi-original.yml
  format: yaml
  label: Leap Dispatch API v2
  slug: dispatch
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leap/refs/heads/main/openapi/leap-dispatching-openapi-original.yml
- filename: leap-nominations-openapi-original.yml
  format: yaml
  label: Leap Meter Nomination API
  slug: nominations
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leap/refs/heads/main/openapi/leap-nominations-openapi-original.yml
- filename: leap-settlement-openapi-original.yml
  format: yaml
  label: Leap Revenue & Analytics API
  slug: revenue
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leap/refs/heads/main/openapi/leap-settlement-openapi-original.yml
- filename: leap-webhooks-openapi-original.yml
  format: yaml
  label: Leap Webhook Subscription API
  slug: webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leap/refs/heads/main/openapi/leap-webhooks-openapi-original.yml
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
- Webhooks
- Climate Tech
---
