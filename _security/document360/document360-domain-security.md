---
api_specs:
- filename: document360-document360-api-openapi.yml
  format: yaml
  label: Document360 API
  slug: document360-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/document360/refs/heads/main/openapi/document360-document360-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: document360.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: document360.io
  spf: true
hosts:
- cert_expires: Sep 27 22:29:17 2026 GMT
  host: document360.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 16:36:35 2026 GMT
  host: apidocs.document360.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  6 22:01:25 2026 GMT
  host: apihub.document360.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Document360 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Document360, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Document360
provider_slug: document360
slug: document360-domain-security
source_filename: document360-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: document360.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 22:29:17 2026 GMT\n  hsts: true\n  hsts_max_age: 0\n- host: apidocs.document360.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 16:36:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: apihub.document360.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 22:01:25 2026 GMT\n  hsts: null\ndomains:\n- domain: document360.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: document360.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/document360/refs/heads/main/security/document360-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Documentation
- Knowledge Base
- SaaS
---
