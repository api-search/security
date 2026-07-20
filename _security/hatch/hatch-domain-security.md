---
api_specs:
- filename: hatch-openapi-original.json
  format: json
  label: Hatch API
  slug: hatch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hatch/refs/heads/main/openapi/hatch-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: usehatchapp.com
  spf: true
hosts:
- cert_expires: Oct 15 20:04:06 2026 GMT
  host: www.usehatchapp.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 14 18:42:16 2026 GMT
  host: docs.usehatchapp.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 15 20:04:06 2026 GMT
  host: api.usehatchapp.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hatch Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hatch, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Hatch
provider_slug: hatch
slug: hatch-domain-security
source_filename: hatch-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.usehatchapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 20:04:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.usehatchapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 18:42:16 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.usehatchapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 20:04:06 2026 GMT\n  hsts: null\ndomains:\n- domain: usehatchapp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hatch/refs/heads/main/security/hatch-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Vertical Software
- Customer Communication
- Conversational AI
- SMS
- Voice
- Email
- Marketing
- Home Services
- Contact Center
---
