---
api_specs:
- filename: zcal-openapi.yml
  format: yaml
  label: Zcal Scheduling Links
  slug: scheduling-links
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zcal/refs/heads/main/openapi/zcal-openapi.yml
- filename: zcal-openapi.yml
  format: yaml
  label: Zcal Bookings
  slug: bookings
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zcal/refs/heads/main/openapi/zcal-openapi.yml
- filename: zcal-openapi.yml
  format: yaml
  label: Zcal Integrations and Webhooks
  slug: integrations-webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zcal/refs/heads/main/openapi/zcal-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: zcal.co
  spf: true
hosts:
- cert_expires: Aug 24 08:54:24 2026 GMT
  host: zcal.co
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  1 02:25:00 2026 GMT
  host: help.zcal.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zcal Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zcal, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Zcal
provider_slug: zcal
slug: zcal-domain-security
source_filename: zcal-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: zcal.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 08:54:24 2026 GMT\n  hsts: false\n- host: help.zcal.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 02:25:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: zcal.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zcal/refs/heads/main/security/zcal-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Scheduling
- Calendar
- Booking
- Meetings
- Webhooks
---
