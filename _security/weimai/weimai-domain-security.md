---
api_specs:
- filename: weimai-openplatform-openapi.json
  format: json
  label: WeiMai Open Platform API
  slug: weimai-open-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weimai/refs/heads/main/openapi/weimai-openplatform-openapi.json
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: myweimai.com
  spf: true
hosts:
- cert_expires: Aug 13 23:59:59 2026 GMT
  host: myweimai.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Aug 13 23:59:59 2026 GMT
  host: openapi.myweimai.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Weimai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for WeiMai, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: WeiMai
provider_slug: weimai
slug: weimai-domain-security
source_filename: weimai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: myweimai.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 13 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: openapi.myweimai.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 13 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: myweimai.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/weimai/refs/heads/main/security/weimai-domain-security.yml
summary_line: TLSv1.2 · HSTS
tags:
- Company
- Healthcare
- Digital Health
- Internet Hospital
- Telemedicine
- Medical Services
- China
- Open Platform
---
