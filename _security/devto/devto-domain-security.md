---
api_specs:
- filename: openapi.json
  format: json
  label: DEV Community API
  slug: devto-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/devto/refs/heads/main/openapi/openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: dev.to
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: forem.com
  spf: true
hosts:
- cert_expires: Dec 12 22:06:30 2026 GMT
  host: dev.to
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.2
- cert_expires: Aug 28 22:03:49 2026 GMT
  host: developers.forem.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Devto Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DEV Community, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: DEV Community
provider_slug: devto
slug: devto-domain-security
source_filename: devto-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dev.to\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 12 22:06:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\n- host: developers.forem.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 22:03:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: dev.to\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: forem.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/devto/refs/heads/main/security/devto-domain-security.yml
summary_line: TLSv1.2 · HSTS · DNSSEC · DMARC
tags:
- Developer Community
- Articles
- Blogging
- Social
- Content
- Open Source
---
