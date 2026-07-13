---
api_specs:
- filename: logrocket-rest-api-openapi.yml
  format: yaml
  label: LogRocket REST API
  slug: logrocket-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logrocket/refs/heads/main/openapi/logrocket-rest-api-openapi.yml
- filename: logrocket-graphql-api-openapi.yml
  format: yaml
  label: LogRocket GraphQL API
  slug: logrocket-graphql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logrocket/refs/heads/main/openapi/logrocket-graphql-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: logrocket.com
  spf: true
hosts:
- cert_expires: Aug 18 17:06:31 2026 GMT
  host: logrocket.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 14:32:06 2026 GMT
  host: docs.logrocket.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  8 17:31:54 2026 GMT
  host: api.logrocket.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Logrocket Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LogRocket, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: LogRocket
provider_slug: logrocket
slug: logrocket-domain-security
source_filename: logrocket-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: logrocket.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 17:06:31 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: docs.logrocket.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 14:32:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.logrocket.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 17:31:54 2026 GMT\n  hsts: null\ndomains:\n- domain: logrocket.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/logrocket/refs/heads/main/security/logrocket-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Session Replay
- Product Analytics
- Frontend Monitoring
- Logging
- Errors
---
