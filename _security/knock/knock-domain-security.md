---
api_specs:
- filename: knock-openapi.json
  format: json
  label: Knock Workflows API
  slug: knock-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knock/refs/heads/main/openapi/knock-openapi.json
- filename: knock-openapi.json
  format: json
  label: Knock Messages API
  slug: knock-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knock/refs/heads/main/openapi/knock-openapi.json
- filename: knock-openapi.json
  format: json
  label: Knock Users API
  slug: knock-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knock/refs/heads/main/openapi/knock-openapi.json
- filename: knock-openapi.json
  format: json
  label: Knock Objects API
  slug: knock-objects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knock/refs/heads/main/openapi/knock-openapi.json
- filename: knock-openapi.json
  format: json
  label: Knock Feeds API
  slug: knock-feeds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knock/refs/heads/main/openapi/knock-openapi.json
- filename: knock-openapi.json
  format: json
  label: Knock Guides API
  slug: knock-guides-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knock/refs/heads/main/openapi/knock-openapi.json
- filename: knock-openapi.json
  format: json
  label: Knock Schedules API
  slug: knock-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knock/refs/heads/main/openapi/knock-openapi.json
- filename: knock-openapi.json
  format: json
  label: Knock Preferences API
  slug: knock-preferences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knock/refs/heads/main/openapi/knock-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: knock.app
  spf: true
hosts:
- cert_expires: Sep 20 15:29:52 2026 GMT
  host: knock.app
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 21:07:44 2026 GMT
  host: docs.knock.app
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 31 23:59:59 2026 GMT
  host: api.knock.app
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Knock Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Knock, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Knock
provider_slug: knock
slug: knock-domain-security
source_filename: knock-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: knock.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 15:29:52 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: docs.knock.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 21:07:44 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.knock.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: knock.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/knock/refs/heads/main/security/knock-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Notifications
- Email
- SMS
- Push
- Workflows
---
