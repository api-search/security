---
api_specs:
- filename: freshpaint-openapi.yml
  format: yaml
  label: Freshpaint Tracking Events API
  slug: freshpaint-tracking-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshpaint/refs/heads/main/openapi/freshpaint-openapi.yml
- filename: freshpaint-openapi.yml
  format: yaml
  label: Freshpaint Identify API
  slug: freshpaint-identify-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshpaint/refs/heads/main/openapi/freshpaint-openapi.yml
- filename: freshpaint-openapi.yml
  format: yaml
  label: Freshpaint Page and Screen API
  slug: freshpaint-page-screen-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshpaint/refs/heads/main/openapi/freshpaint-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: freshpaint.io
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: perfalytics.com
  spf: false
hosts:
- cert_expires: Sep 12 06:11:16 2026 GMT
  host: www.freshpaint.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  1 05:13:12 2026 GMT
  host: documentation.freshpaint.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 24 23:59:59 2026 GMT
  host: api.perfalytics.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Freshpaint Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Freshpaint, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Freshpaint
provider_slug: freshpaint
slug: freshpaint-domain-security
source_filename: freshpaint-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.freshpaint.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 06:11:16 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: documentation.freshpaint.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 05:13:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.perfalytics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 24 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: freshpaint.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: perfalytics.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/freshpaint/refs/heads/main/security/freshpaint-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Customer Data Platform
- Event Tracking
- Healthcare
- HIPAA
- Privacy
- Analytics
---
