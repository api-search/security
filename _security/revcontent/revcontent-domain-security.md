---
api_specs:
- filename: revcontent-stats-management-openapi.yml
  format: yaml
  label: RevContent Stats & Management API
  slug: revcontent-stats-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revcontent/refs/heads/main/openapi/revcontent-stats-management-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: revcontent.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: revcontent.io
  spf: false
hosts:
- cert_expires: Sep 18 13:55:39 2026 GMT
  host: www.revcontent.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 07:43:47 2026 GMT
  host: help.revcontent.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 13:55:39 2026 GMT
  host: api.revcontent.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Revcontent Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RevContent, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: RevContent
provider_slug: revcontent
slug: revcontent-domain-security
source_filename: revcontent-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.revcontent.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 13:55:39 2026 GMT\n  hsts: false\n- host: help.revcontent.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 07:43:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.revcontent.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 13:55:39 2026 GMT\n  hsts: false\ndomains:\n- domain: revcontent.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: revcontent.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/revcontent/refs/heads/main/security/revcontent-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Native Advertising
- Content Recommendation
- Ad Network
- Publisher Monetization
- Programmatic Advertising
---
