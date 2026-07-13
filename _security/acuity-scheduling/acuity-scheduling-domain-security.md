---
api_specs:
- filename: acuity-scheduling-asyncapi.yml
  format: yaml
  label: Acuity Scheduling Webhooks
  slug: webhooks-asyncapi
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/acuity-scheduling/refs/heads/main/openapi/acuity-scheduling-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: acuityscheduling.com
  spf: true
hosts:
- cert_expires: Oct 17 23:59:59 2026 GMT
  host: acuityscheduling.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct  4 07:47:32 2026 GMT
  host: developers.acuityscheduling.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Acuity Scheduling Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Acuity Scheduling, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Acuity Scheduling
provider_slug: acuity-scheduling
slug: acuity-scheduling-domain-security
source_filename: acuity-scheduling-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: acuityscheduling.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developers.acuityscheduling.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 07:47:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: acuityscheduling.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/acuity-scheduling/refs/heads/main/security/acuity-scheduling-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Appointment Scheduling
- Booking
- Calendar
- Scheduling
- Squarespace
---
