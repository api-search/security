---
api_specs:
- filename: higgsfield-openapi-original.json
  format: json
  label: Higgsfield API
  slug: higgsfield-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/higgsfield/refs/heads/main/openapi/higgsfield-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: higgsfield.ai
  spf: true
hosts:
- cert_expires: Oct 17 13:17:19 2026 GMT
  host: higgsfield.ai
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 15:13:49 2026 GMT
  host: docs.higgsfield.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 12 23:31:49 2026 GMT
  host: platform.higgsfield.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Higgsfield Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Higgsfield, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Higgsfield
provider_slug: higgsfield
slug: higgsfield-domain-security
source_filename: higgsfield-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: higgsfield.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 13:17:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\n- host: docs.higgsfield.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 15:13:49 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: platform.higgsfield.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 23:31:49 2026 GMT\n  hsts: null\ndomains:\n- domain: higgsfield.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/higgsfield/refs/heads/main/security/higgsfield-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai
- Generative AI
- Video Generation
- Image Generation
- Machine Learning
- Media
- Content Creation
- Developer API
---
