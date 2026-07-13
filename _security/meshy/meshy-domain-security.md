---
api_specs:
- filename: meshy-openapi.yml
  format: yaml
  label: Meshy API
  slug: platform
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meshy/refs/heads/main/openapi/meshy-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: meshy.ai
  spf: false
hosts:
- cert_expires: Sep 11 23:59:59 2026 GMT
  host: www.meshy.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 01:07:36 2026 GMT
  host: docs.meshy.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 11 23:59:59 2026 GMT
  host: api.meshy.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Meshy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Meshy, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: Meshy
provider_slug: meshy
slug: meshy-domain-security
source_filename: meshy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.meshy.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 23:59:59 2026 GMT\n  hsts: false\n- host: docs.meshy.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 01:07:36 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.meshy.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: meshy.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/meshy/refs/heads/main/security/meshy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- 3D
- Generation
- Texturing
- Animation
- Rigging
- Printing
---
