---
api_specs:
- filename: wistia-openapi.yml
  format: yaml
  label: Wistia Data API
  slug: data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wistia/refs/heads/main/openapi/wistia-openapi.yml
- filename: wistia-asyncapi.yml
  format: yaml
  label: Wistia Webhooks
  slug: webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/wistia/refs/heads/main/asyncapi/wistia-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: wistia.com
  spf: true
hosts:
- cert_expires: Jan 10 02:10:20 2027 GMT
  host: wistia.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 01:02:20 2026 GMT
  host: docs.wistia.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 27 23:59:59 2027 GMT
  host: api.wistia.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wistia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wistia, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Wistia
provider_slug: wistia
slug: wistia-domain-security
source_filename: wistia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: wistia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 02:10:20 2027 GMT\n  hsts: false\n- host: docs.wistia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 01:02:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.wistia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 27 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: wistia.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wistia/refs/heads/main/security/wistia-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Video Hosting
- Video Marketing
- Video Analytics
- Lead Generation
- Webinars
- B2B Marketing
---
