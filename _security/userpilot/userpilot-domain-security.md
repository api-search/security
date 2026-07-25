---
api_specs:
- filename: userpilot-analytics-api-openapi.yml
  format: yaml
  label: Userpilot Analytics API
  slug: userpilot-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/userpilot/refs/heads/main/openapi/userpilot-analytics-api-openapi.yml
- filename: userpilot-background-jobs-api-openapi.yml
  format: yaml
  label: Userpilot Background Jobs API
  slug: userpilot-background-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/userpilot/refs/heads/main/openapi/userpilot-background-jobs-api-openapi.yml
- filename: userpilot-companies-api-openapi.yml
  format: yaml
  label: Userpilot Companies API
  slug: userpilot-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/userpilot/refs/heads/main/openapi/userpilot-companies-api-openapi.yml
- filename: userpilot-imports-api-openapi.yml
  format: yaml
  label: Userpilot Imports API
  slug: userpilot-imports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/userpilot/refs/heads/main/openapi/userpilot-imports-api-openapi.yml
- filename: userpilot-real-time-api-openapi.yml
  format: yaml
  label: Userpilot Real-time API
  slug: userpilot-real-time-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/userpilot/refs/heads/main/openapi/userpilot-real-time-api-openapi.yml
- filename: userpilot-track-api-openapi.yml
  format: yaml
  label: Userpilot Track API
  slug: userpilot-track-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/userpilot/refs/heads/main/openapi/userpilot-track-api-openapi.yml
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
