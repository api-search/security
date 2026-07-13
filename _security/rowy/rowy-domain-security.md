---
api_specs:
- filename: rowy-openapi.yml
  format: yaml
  label: Rowy Webhooks
  slug: rowy-webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rowy/refs/heads/main/openapi/rowy-openapi.yml
- filename: rowy-openapi.yml
  format: yaml
  label: Rowy Run / Cloud Functions
  slug: rowy-run-cloud-functions
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rowy/refs/heads/main/openapi/rowy-openapi.yml
- filename: rowy-openapi.yml
  format: yaml
  label: Rowy Firestore Data
  slug: rowy-firestore-data
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rowy/refs/heads/main/openapi/rowy-openapi.yml
description: ''
domains:
- caa:
  - cdn.webflow.com.
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: rowy.io
  spf: false
hosts:
- cert_expires: Sep 11 04:09:10 2026 GMT
  host: www.rowy.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 19 21:26:52 2026 GMT
  host: docs.rowy.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rowy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rowy, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC present (p=quarantine).'
provider_name: Rowy
provider_slug: rowy
slug: rowy-domain-security
source_filename: rowy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.rowy.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 04:09:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.rowy.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 21:26:52 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: rowy.io\n  dnssec: true\n  caa:\n  - cdn.webflow.com.\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rowy/refs/heads/main/security/rowy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Low-Code
- Backend
- Firestore
- Firebase
- Webhooks
- Cloud Functions
---
