---
api_specs:
- filename: userpilot-analytex-openapi.json
  format: json
  label: Userpilot Realtime API (analytex)
  slug: userpilot-realtime-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/userpilot/refs/heads/main/openapi/userpilot-analytex-openapi.json
- filename: userpilot-appex-openapi.json
  format: json
  label: Userpilot Analytics Export API (appex)
  slug: userpilot-analytics-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/userpilot/refs/heads/main/openapi/userpilot-appex-openapi.json
- filename: userpilot-openapi.json
  format: json
  label: Userpilot API
  slug: userpilot-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/userpilot/refs/heads/main/openapi/userpilot-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: userpilot.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: userpilot.io
  spf: true
hosts:
- cert_expires: Sep 19 15:00:39 2026 GMT
  host: userpilot.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 23 09:42:59 2026 GMT
  host: docs.userpilot.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 15 23:59:59 2027 GMT
  host: analytex.userpilot.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Userpilot Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Userpilot, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Userpilot
provider_slug: userpilot
slug: userpilot-domain-security
source_filename: userpilot-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: userpilot.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 15:00:39 2026 GMT\n  hsts: false\n- host: docs.userpilot.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 09:42:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: analytex.userpilot.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: userpilot.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: userpilot.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/userpilot/refs/heads/main/security/userpilot-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Product
- Onboarding
- In-App Guidance
- Analytics
- Customer Success
---
