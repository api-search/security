---
api_specs:
- filename: later-influence-api-openapi.json
  format: json
  label: Later Influence API
  slug: later-influence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/later/refs/heads/main/openapi/later-influence-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: later.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: mavrck.co
  spf: true
hosts:
- cert_expires: Nov  1 18:53:48 2026 GMT
  host: later.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 18 20:09:08 2026 GMT
  host: app.later.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 25 23:59:59 2026 GMT
  host: api.mavrck.co
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Later Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Later, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Later
provider_slug: later
slug: later-domain-security
source_filename: later-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: later.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 18:53:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.later.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 20:09:08 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.mavrck.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: later.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: mavrck.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/later/refs/heads/main/security/later-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Social-Media
- Scheduling
- Instagram
- TikTok
- Influencer Marketing
- Content Management
- Analytics
- Social Commerce
---
