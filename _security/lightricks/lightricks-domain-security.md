---
api_specs:
- filename: lightricks-ltx-openapi.yml
  format: yaml
  label: LTX API
  slug: ltx-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lightricks/refs/heads/main/openapi/lightricks-ltx-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: lightricks.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ltx.io
  spf: true
hosts:
- cert_expires: Sep  1 04:16:29 2026 GMT
  host: www.lightricks.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 13:33:13 2026 GMT
  host: docs.ltx.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 12 07:29:07 2026 GMT
  host: api.ltx.video
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lightricks Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lightricks, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Lightricks
provider_slug: lightricks
slug: lightricks-domain-security
source_filename: lightricks-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.lightricks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 04:16:29 2026 GMT\n  hsts: false\n- host: docs.ltx.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 13:33:13 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.ltx.video\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 07:29:07 2026 GMT\n  hsts: null\ndomains:\n- domain: lightricks.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: ltx.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lightricks/refs/heads/main/security/lightricks-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer
- Artificial Intelligence
- Generative AI
- Video
- Video Generation
- Media
- Machine Learning
- Creative Tools
---
