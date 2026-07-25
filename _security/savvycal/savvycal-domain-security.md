---
api_specs:
- filename: savvycal-current-user-api-openapi.yml
  format: yaml
  label: SavvyCal Current User API
  slug: savvycal-current-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/savvycal/refs/heads/main/openapi/savvycal-current-user-api-openapi.yml
- filename: savvycal-events-api-openapi.yml
  format: yaml
  label: SavvyCal Events API
  slug: savvycal-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/savvycal/refs/heads/main/openapi/savvycal-events-api-openapi.yml
- filename: savvycal-scheduling-links-api-openapi.yml
  format: yaml
  label: SavvyCal Scheduling Links API
  slug: savvycal-scheduling-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/savvycal/refs/heads/main/openapi/savvycal-scheduling-links-api-openapi.yml
- filename: savvycal-time-zones-api-openapi.yml
  format: yaml
  label: SavvyCal Time Zones API
  slug: savvycal-time-zones-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/savvycal/refs/heads/main/openapi/savvycal-time-zones-api-openapi.yml
- filename: savvycal-webhooks-api-openapi.yml
  format: yaml
  label: SavvyCal Webhooks API
  slug: savvycal-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/savvycal/refs/heads/main/openapi/savvycal-webhooks-api-openapi.yml
- filename: savvycal-workflows-api-openapi.yml
  format: yaml
  label: SavvyCal Workflows API
  slug: savvycal-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/savvycal/refs/heads/main/openapi/savvycal-workflows-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: savvycal.com
  spf: true
hosts:
- cert_expires: Sep 25 23:21:56 2026 GMT
  host: savvycal.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 10:48:18 2026 GMT
  host: developers.savvycal.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 23:21:56 2026 GMT
  host: api.savvycal.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Savvycal Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SavvyCal, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: SavvyCal
provider_slug: savvycal
slug: savvycal-domain-security
source_filename: savvycal-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: savvycal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 23:21:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.savvycal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 10:48:18 2026 GMT\n  hsts: false\n- host: api.savvycal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 23:21:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: savvycal.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/savvycal/refs/heads/main/security/savvycal-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Scheduling
- Calendar
- Appointments
- Availability
- Booking
- Meetings
- Webhooks
---
