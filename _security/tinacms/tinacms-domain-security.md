---
api_specs:
- filename: queries
  format: yaml
  label: TinaCMS GraphQL Content API
  slug: graphql-content-api
  spec_type: OpenAPI
  url: https://tina.io/docs/graphql/queries
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: tina.io
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: tinajs.io
  spf: false
hosts:
- cert_expires: Sep  2 11:09:37 2026 GMT
  host: tina.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  4 23:59:59 2026 GMT
  host: content.tinajs.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tinacms Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TinaCMS, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: TinaCMS
provider_slug: tinacms
slug: tinacms-domain-security
source_filename: tinacms-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tina.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 11:09:37 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: content.tinajs.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  4 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: tina.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: tinajs.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tinacms/refs/heads/main/security/tinacms-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- CMS
- Headless CMS
- GraphQL
- Git
- Content Management
- Visual Editing
- Markdown
- Open Source
---
