---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: joy.io
  spf: true
  spf_policy: softfail
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: privateaser.com
  note: a detectify-verification TXT record is published on privateaser.com, indicating an external attack-surface scanning service is in use; this is not a published vulnerability disclosure program and no security.txt or disclosure page was found.
  spf: true
  spf_policy: softfail
hosts:
- cert_expires: Nov  3 14:02:12 2026 GMT
  host: joy.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  1 23:59:59 2027 GMT
  host: app.joy.io
  hsts: false
  hsts_max_age: null
  https: true
  note: single-page manager application (nginx); returns HTTP 200 with the same SPA shell for every path
  tls_version: TLSv1.3
- cert_expires: Nov  4 05:15:51 2026 GMT
  host: faq.joy.io
  hsts: true
  hsts_max_age: 86400
  https: true
  note: help center behind Cloudflare, origin Render; serves the provider llms.txt
  tls_version: TLSv1.3
- cert_expires: Feb  1 23:59:59 2027 GMT
  host: www.privateaser.com
  hsts: false
  hsts_max_age: null
  https: true
  note: CloudFront-fronted marketplace; returns HTTP 403 "Request blocked" to non-browser user agents
  tls_version: TLSv1.3
- cert_expires: Feb  1 23:59:59 2027 GMT
  host: manager-api.privateaser.com
  hsts: false
  hsts_max_age: null
  https: true
  note: private backend for the Joy manager app (gunicorn/uvicorn), AWS Cognito user pool auth; HTTP 404 on /, /openapi.json, /openapi.yaml, /swagger.json, /api-docs, /docs, /redoc, /graphql
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Joy Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Joy (ex-Privateaser), probed live across 5 host(s) and 2 registrable domain(s). 5 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Joy (ex-Privateaser)
provider_slug: joy-io
slug: joy-io-domain-security
source_filename: joy-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of the joy.io and privateaser.com hosts reached during enrichment\nnote: >-\n  joy.io (Website), app.joy.io (manager application), faq.joy.io (help center) and the\n  privateaser.com marketplace were probed. manager-api.privateaser.com is the private backend\n  the Joy manager app calls (found in https://app.joy.io/config.js); it is not a published API\n  and every spec path on it returns HTTP 404. Only joy.io serves HSTS with a long max-age;\n  app.joy.io, www.privateaser.com and manager-api.privateaser.com return no HSTS header at all.\n  Neither registrable domain is DNSSEC-signed and neither publishes a CAA record. Both domains\n  publish SPF with a soft-fail (~all) and DMARC at p=none, which monitors but does not enforce.\nhosts:\n- host: joy.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  3 14:02:12 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: app.joy.io\n  https: true\n\
  \  tls_version: TLSv1.3\n  cert_expires: Feb  1 23:59:59 2027 GMT\n  hsts: false\n  hsts_max_age: null\n  note: single-page manager application (nginx); returns HTTP 200 with the same SPA shell for every path\n- host: faq.joy.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  4 05:15:51 2026 GMT\n  hsts: true\n  hsts_max_age: 86400\n  note: help center behind Cloudflare, origin Render; serves the provider llms.txt\n- host: www.privateaser.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  1 23:59:59 2027 GMT\n  hsts: false\n  hsts_max_age: null\n  note: CloudFront-fronted marketplace; returns HTTP 403 \"Request blocked\" to non-browser user agents\n- host: manager-api.privateaser.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  1 23:59:59 2027 GMT\n  hsts: false\n  hsts_max_age: null\n  note: >-\n    private backend for the Joy manager app (gunicorn/uvicorn), AWS Cognito user pool auth;\n    HTTP 404 on /, /openapi.json, /openapi.yaml, /swagger.json,\
  \ /api-docs, /docs, /redoc, /graphql\ndomains:\n- domain: joy.io\n  dnssec: false\n  caa: []\n  spf: true\n  spf_policy: softfail\n  dmarc: true\n  dmarc_policy: none\n- domain: privateaser.com\n  dnssec: false\n  caa: []\n  spf: true\n  spf_policy: softfail\n  dmarc: true\n  dmarc_policy: none\n  note: >-\n    a detectify-verification TXT record is published on privateaser.com, indicating an external\n    attack-surface scanning service is in use; this is not a published vulnerability disclosure\n    program and no security.txt or disclosure page was found.\nx-evidence:\n- url: https://joy.io/\n  status: 200\n- url: https://app.joy.io/\n  status: 200\n- url: https://faq.joy.io/\n  status: 200\n- url: https://www.privateaser.com/\n  status: 200\n- url: https://manager-api.privateaser.com/\n  status: 404\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/joy-io/refs/heads/main/security/joy-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Marketplace
- Reservations
- Bookings
- Restaurant
- Hospitality
- Event
- Software-as-a-Service
- France
---
