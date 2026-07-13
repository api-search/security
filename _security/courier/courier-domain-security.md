---
api_specs:
- filename: courier-openapi.yml
  format: yaml
  label: Courier Send API
  slug: courier-send-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/courier/refs/heads/main/openapi/courier-openapi.yml
- filename: courier-openapi.yml
  format: yaml
  label: Courier User Profiles API
  slug: courier-user-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/courier/refs/heads/main/openapi/courier-openapi.yml
- filename: courier-openapi.yml
  format: yaml
  label: Courier Lists API
  slug: courier-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/courier/refs/heads/main/openapi/courier-openapi.yml
- filename: courier-openapi.yml
  format: yaml
  label: Courier Events API
  slug: courier-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/courier/refs/heads/main/openapi/courier-openapi.yml
- filename: courier-openapi.yml
  format: yaml
  label: Courier Brands API
  slug: courier-brands-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/courier/refs/heads/main/openapi/courier-openapi.yml
- filename: courier-openapi.yml
  format: yaml
  label: Courier Authentication API
  slug: courier-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/courier/refs/heads/main/openapi/courier-openapi.yml
- filename: courier-asyncapi.yml
  format: yaml
  label: Courier Inbox Real-Time API
  slug: courier-inbox-real-time-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/courier/refs/heads/main/asyncapi/courier-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: courier.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: courier.io
  spf: false
hosts:
- cert_expires: Oct  4 22:32:39 2026 GMT
  host: www.courier.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 11 13:36:56 2026 GMT
  host: api.courier.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 16 18:44:30 2026 GMT
  host: realtime.courier.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Courier Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Courier, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Courier
provider_slug: courier
slug: courier-domain-security
source_filename: courier-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.courier.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 22:32:39 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.courier.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 13:36:56 2026 GMT\n  hsts: null\n- host: realtime.courier.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 18:44:30 2026 GMT\n  hsts: null\ndomains:\n- domain: courier.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: courier.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/courier/refs/heads/main/security/courier-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Notifications
- Email
- SMS
- Push
- API
---
