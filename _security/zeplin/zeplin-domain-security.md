---
api_specs:
- filename: openapi
  format: yaml
  label: Zeplin API
  slug: zeplin-api
  spec_type: OpenAPI
  url: https://github.com/zeplin/openapi
description: ''
domains:
- caa:
  - 0 issue "amazontrust.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: zeplin.io
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: zeplin.dev
  spf: false
hosts:
- cert_expires: Sep 14 23:59:59 2026 GMT
  host: zeplin.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 08:53:30 2026 GMT
  host: docs.zeplin.dev
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 23:59:59 2026 GMT
  host: api.zeplin.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zeplin Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zeplin, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Zeplin
provider_slug: zeplin
slug: zeplin-domain-security
source_filename: zeplin-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: zeplin.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.zeplin.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 08:53:30 2026 GMT\n  hsts: null\n- host: api.zeplin.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: zeplin.io\n  dnssec: false\n  caa:\n  - 0 issue \"amazontrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: zeplin.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zeplin/refs/heads/main/security/zeplin-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Design
- Design Handoff
- Developer Tools
- Figma
- Sketch
- Adobe XD
- Style Guides
- Components
- Assets
- Webhooks
---
