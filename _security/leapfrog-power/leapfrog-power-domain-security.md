---
api_specs:
- filename: leapfrog-power-create-meters-api-openapi.yml
  format: yaml
  label: Leap create meters API
  slug: leapfrog-power-create-meters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leapfrog-power/refs/heads/main/openapi/leapfrog-power-create-meters-api-openapi.yml
- filename: leapfrog-power-group-dispatches-api-openapi.yml
  format: yaml
  label: Leap Group Dispatches API
  slug: leapfrog-power-group-dispatches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leapfrog-power/refs/heads/main/openapi/leapfrog-power-group-dispatches-api-openapi.yml
- filename: leapfrog-power-interval-data-upload-api-openapi.yml
  format: yaml
  label: Leap Interval Data Upload API
  slug: leapfrog-power-interval-data-upload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leapfrog-power/refs/heads/main/openapi/leapfrog-power-interval-data-upload-api-openapi.yml
- filename: leapfrog-power-meter-details-api-openapi.yml
  format: yaml
  label: Leap Meter Details API
  slug: leapfrog-power-meter-details-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leapfrog-power/refs/heads/main/openapi/leapfrog-power-meter-details-api-openapi.yml
- filename: leapfrog-power-meter-dispatches-api-openapi.yml
  format: yaml
  label: Leap Meter Dispatches API
  slug: leapfrog-power-meter-dispatches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leapfrog-power/refs/heads/main/openapi/leapfrog-power-meter-dispatches-api-openapi.yml
- filename: leapfrog-power-meter-enrollment-api-openapi.yml
  format: yaml
  label: Leap meter enrollment API
  slug: leapfrog-power-meter-enrollment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leapfrog-power/refs/heads/main/openapi/leapfrog-power-meter-enrollment-api-openapi.yml
- filename: leapfrog-power-nominations-api-openapi.yml
  format: yaml
  label: Leap Nominations API
  slug: leapfrog-power-nominations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leapfrog-power/refs/heads/main/openapi/leapfrog-power-nominations-api-openapi.yml
- filename: leapfrog-power-performance-api-openapi.yml
  format: yaml
  label: Leap Performance API
  slug: leapfrog-power-performance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leapfrog-power/refs/heads/main/openapi/leapfrog-power-performance-api-openapi.yml
- filename: leapfrog-power-provisional-assets-api-openapi.yml
  format: yaml
  label: Leap provisional assets API
  slug: leapfrog-power-provisional-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leapfrog-power/refs/heads/main/openapi/leapfrog-power-provisional-assets-api-openapi.yml
- filename: leapfrog-power-revenue-api-openapi.yml
  format: yaml
  label: Leap Revenue API
  slug: leapfrog-power-revenue-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leapfrog-power/refs/heads/main/openapi/leapfrog-power-revenue-api-openapi.yml
- filename: leapfrog-power-webhooks-api-openapi.yml
  format: yaml
  label: Leap Webhooks API
  slug: leapfrog-power-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leapfrog-power/refs/heads/main/openapi/leapfrog-power-webhooks-api-openapi.yml
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
name: Leapfrog Power Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Leap, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Leap
provider_slug: leapfrog-power
slug: leapfrog-power-domain-security
source_filename: leapfrog-power-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.leap.energy\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 08:51:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.leap.energy\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 16:10:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.leap.energy\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov  7 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: leap.energy\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/leapfrog-power/refs/heads/main/security/leapfrog-power-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Energy
- United States
- Electricity
- Grid
- Demand Response
- DER
- Virtual Power Plant
- Energy Markets
- Storage Flexibility
- EV Charging
- Smart Metering
---
