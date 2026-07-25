---
api_specs:
- filename: luma-calendars-api-openapi.yml
  format: yaml
  label: Luma Calendars API
  slug: luma-calendars-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/luma/refs/heads/main/openapi/luma-calendars-api-openapi.yml
- filename: luma-events-api-openapi.yml
  format: yaml
  label: Luma Events API
  slug: luma-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/luma/refs/heads/main/openapi/luma-events-api-openapi.yml
- filename: luma-memberships-api-openapi.yml
  format: yaml
  label: Luma Memberships API
  slug: luma-memberships-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/luma/refs/heads/main/openapi/luma-memberships-api-openapi.yml
- filename: luma-miscellaneous-api-openapi.yml
  format: yaml
  label: Luma Miscellaneous API
  slug: luma-miscellaneous-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/luma/refs/heads/main/openapi/luma-miscellaneous-api-openapi.yml
- filename: luma-organizations-api-openapi.yml
  format: yaml
  label: Luma Organizations API
  slug: luma-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/luma/refs/heads/main/openapi/luma-organizations-api-openapi.yml
- filename: luma-webhooks-api-openapi.yml
  format: yaml
  label: Luma Webhooks API
  slug: luma-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/luma/refs/heads/main/openapi/luma-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: luma.com
  spf: true
hosts:
- cert_expires: Sep  7 02:00:29 2026 GMT
  host: docs.luma.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 17:43:45 2026 GMT
  host: public-api.luma.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Luma Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Luma, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Luma
provider_slug: luma
slug: luma-domain-security
source_filename: luma-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.luma.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 02:00:29 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: public-api.luma.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 17:43:45 2026 GMT\n  hsts: true\n  hsts_max_age: 300\ndomains:\n- domain: luma.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/luma/refs/heads/main/security/luma-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Events
- Event Management
- Ticketing
- Community
- Calendars
- Guests
- Attendance
---
