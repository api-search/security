---
api_specs:
- filename: accelevents-openapi.yml
  format: yaml
  label: Accelevents Events API
  slug: accelevents-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accelevents/refs/heads/main/openapi/accelevents-openapi.yml
- filename: accelevents-openapi.yml
  format: yaml
  label: Accelevents Attendees API
  slug: accelevents-attendees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accelevents/refs/heads/main/openapi/accelevents-openapi.yml
- filename: accelevents-openapi.yml
  format: yaml
  label: Accelevents Ticketing Orders API
  slug: accelevents-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accelevents/refs/heads/main/openapi/accelevents-openapi.yml
- filename: accelevents-openapi.yml
  format: yaml
  label: Accelevents Tickets API
  slug: accelevents-tickets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accelevents/refs/heads/main/openapi/accelevents-openapi.yml
- filename: accelevents-openapi.yml
  format: yaml
  label: Accelevents Sessions API
  slug: accelevents-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accelevents/refs/heads/main/openapi/accelevents-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: accelevents.com
  spf: true
hosts:
- cert_expires: Dec 24 23:59:59 2026 GMT
  host: www.accelevents.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 15:15:38 2026 GMT
  host: developer.accelevents.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 24 23:59:59 2026 GMT
  host: api.accelevents.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Accelevents Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Accelevents, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Accelevents
provider_slug: accelevents
slug: accelevents-domain-security
source_filename: accelevents-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.accelevents.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developer.accelevents.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 15:15:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.accelevents.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 24 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: accelevents.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/accelevents/refs/heads/main/security/accelevents-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Event Management
- Ticketing
- Events
- Registration
- Virtual Events
- Sessions
---
