---
api_specs:
- filename: jebbit-openapi-original.json
  format: json
  label: Jebbit API
  slug: jebbit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jebbit/refs/heads/main/openapi/jebbit-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: jebbit.com
  spf: true
hosts:
- cert_expires: Aug 24 07:32:45 2026 GMT
  host: jebbit.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 22 23:59:59 2027 GMT
  host: api2.jebbit.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Jebbit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jebbit, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Jebbit
provider_slug: jebbit
slug: jebbit-domain-security
source_filename: jebbit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: jebbit.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 07:32:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api2.jebbit.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 22 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: jebbit.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jebbit/refs/heads/main/security/jebbit-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Interactive Experiences
- Zero-Party Data
- First-Party Data
- Marketing
- Quizzes
- Product Feeds
- Webhooks
- Customer Data
- JSON:API
---
