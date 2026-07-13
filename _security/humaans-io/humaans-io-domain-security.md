---
api_specs:
- filename: humaans-api-openapi.yml
  format: yaml
  label: Humaans API
  slug: humaans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/humaans-io/refs/heads/main/openapi/humaans-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: humaans.io
  spf: true
hosts:
- cert_expires: Aug 25 13:23:52 2026 GMT
  host: humaans.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 17:53:42 2026 GMT
  host: docs.humaans.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 18:14:44 2026 GMT
  host: app.humaans.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Humaans Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Humaans, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Humaans
provider_slug: humaans-io
slug: humaans-io-domain-security
source_filename: humaans-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: humaans.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 13:23:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.humaans.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 17:53:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.humaans.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 18:14:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: humaans.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/humaans-io/refs/heads/main/security/humaans-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- HR
- HRIS
- Human Resources
- People Operations
- People Analytics
- Onboarding
- Offboarding
- Performance Management
- Time Off
- Compensation
- Workflow Automation
- AI Companion
- Agentic AI
- UK
- London
---
