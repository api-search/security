---
api_specs:
- filename: api-docs.json
  format: json
  label: Gleap REST API
  slug: gleap-rest-api
  spec_type: OpenAPI
  url: https://api.gleap.io/api-docs.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: gleap.io
  spf: true
hosts:
- cert_expires: Oct  1 06:13:56 2026 GMT
  host: gleap.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 03:16:41 2026 GMT
  host: docs.gleap.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Apr 10 23:59:59 2027 GMT
  host: api.gleap.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gleap Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gleap, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Gleap
provider_slug: gleap
slug: gleap-domain-security
source_filename: gleap-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gleap.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 06:13:56 2026 GMT\n  hsts: false\n- host: docs.gleap.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 03:16:41 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.gleap.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 10 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: gleap.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gleap/refs/heads/main/security/gleap-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Customer Feedback
- Bug Reporting
- In-App Support
- Feature Requests
- Roadmap
- Live Chat
- AI Agents
- Session Replay
- Help Center
- Ticketing
- User Feedback
- SaaS
---
