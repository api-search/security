---
api_specs:
- filename: callfire-openapi-generated.yml
  format: yaml
  label: Callfire API
  slug: callfire-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/callfire/refs/heads/main/openapi/_ae-authored/callfire-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: callfire.com
  spf: true
hosts:
- cert_expires: Dec 24 23:59:59 2026 GMT
  host: www.callfire.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
- cert_expires: Jan  1 23:42:39 2027 GMT
  host: developers.callfire.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 24 23:59:59 2026 GMT
  host: api.callfire.com
  hsts: null
  https: true
  tls_version: TLSv1.2
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Callfire Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Callfire, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Callfire
provider_slug: callfire
slug: callfire-domain-security
source_filename: callfire-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.callfire.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 24 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developers.callfire.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 23:42:39 2027 GMT\n  hsts: false\n- host: api.callfire.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 24 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: callfire.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/callfire/refs/heads/main/security/callfire-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Communications
- Cloud
- Messaging
- Voice
---
