---
api_specs:
- filename: openapi.json
  format: json
  label: Fibery HTTP API
  slug: fibery-http-api
  spec_type: OpenAPI
  url: https://developers.fibery.com/api-reference/openapi.json
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: fibery.com
  spf: false
hosts:
- cert_expires: Oct  4 14:12:56 2026 GMT
  host: fibery.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 13:55:39 2026 GMT
  host: developers.fibery.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fibery Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fibery, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Fibery
provider_slug: fibery
slug: fibery-domain-security
source_filename: fibery-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fibery.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 14:12:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.fibery.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 13:55:39 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: fibery.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fibery/refs/heads/main/security/fibery-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Work Management
- Project Management
- Collaboration
- No-Code
- Automation
- GraphQL
- Webhooks
---
