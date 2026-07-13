---
api_specs:
- filename: openapi-accounts.yaml
  format: yaml
  label: Docupilot API
  slug: docupilot-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/docupilot/refs/heads/main/openapi/openapi-accounts.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: docupilot.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: docupilot.app
  spf: true
hosts:
- cert_expires: Sep  1 16:57:32 2026 GMT
  host: www.docupilot.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  1 02:29:04 2026 GMT
  host: help.docupilot.app
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 11 23:59:59 2026 GMT
  host: api-us1.docupilot.app
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Docupilot Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Docupilot, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Docupilot
provider_slug: docupilot
slug: docupilot-domain-security
source_filename: docupilot-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.docupilot.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 16:57:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: help.docupilot.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 02:29:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api-us1.docupilot.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: docupilot.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: docupilot.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/docupilot/refs/heads/main/security/docupilot-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Document Generation
- PDF Generation
- Document Automation
- Template Engine
- eSignature
- Workflow Automation
---
