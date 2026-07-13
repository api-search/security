---
api_specs:
- filename: delighted-delighted-api-openapi.yml
  format: yaml
  label: Delighted API
  slug: delighted-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/delighted/refs/heads/main/openapi/delighted-delighted-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: delighted.com
  spf: true
hosts:
- cert_expires: Jan 15 23:59:59 2027 GMT
  host: delighted.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 13 23:59:59 2026 GMT
  host: app.delighted.com
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct 13 23:59:59 2026 GMT
  host: api.delighted.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Delighted Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Delighted, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Delighted
provider_slug: delighted
slug: delighted-domain-security
source_filename: delighted-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: delighted.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.delighted.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 13 23:59:59 2026 GMT\n  hsts: null\n- host: api.delighted.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 13 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: delighted.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/delighted/refs/heads/main/security/delighted-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- NPS
- Net Promoter Score
- CSAT
- Customer Satisfaction
- CES
- Customer Effort Score
- Survey
- Customer Experience
- Feedback
- eNPS
---
