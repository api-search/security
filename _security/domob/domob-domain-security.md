---
api_specs:
- filename: domob-media-data-api-openapi.yml
  format: yaml
  label: Domob Media Data API
  slug: domob-media-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/domob/refs/heads/main/openapi/domob-media-data-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: domob.cn
  spf: true
hosts:
- cert_expires: Oct 12 05:23:23 2026 GMT
  host: www.domob.cn
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct 12 05:23:23 2026 GMT
  host: developer.domob.cn
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Domob Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for domob, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: domob
provider_slug: domob
slug: domob-domain-security
source_filename: domob-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.domob.cn\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 12 05:23:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.domob.cn\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 12 05:23:23 2026 GMT\n  hsts: false\ndomains:\n- domain: domob.cn\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/domob/refs/heads/main/security/domob-domain-security.yml
summary_line: TLSv1.2 · HSTS
tags:
- Company
- Advertising
- Mobile
- AdTech
- Marketing
- SDK
- DSP
- Monetization
- Reporting
- China
---
