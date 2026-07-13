---
api_specs:
- filename: coder
  format: yaml
  label: Voxco Survey API
  slug: voxco-survey-api
  spec_type: OpenAPI
  url: https://webservices.goascribe.com/coder
- filename: coder
  format: yaml
  label: Voxco Ascribe Coder API
  slug: voxco-ascribe-coder-api
  spec_type: OpenAPI
  url: https://webservices.goascribe.com/coder
- filename: cxi
  format: yaml
  label: Voxco Ascribe CX Inspector API
  slug: voxco-ascribe-cxi-api
  spec_type: OpenAPI
  url: https://webservices.goascribe.com/cxi
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: voxco.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: goascribe.com
  spf: true
hosts:
- cert_expires: Aug 16 00:00:36 2026 GMT
  host: www.voxco.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 19 23:59:59 2026 GMT
  host: na1.voxco.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  1 23:59:59 2026 GMT
  host: webservices.goascribe.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Voxco Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Voxco, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Voxco
provider_slug: voxco
slug: voxco-domain-security
source_filename: voxco-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.voxco.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 00:00:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: na1.voxco.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 23:59:59 2026 GMT\n  hsts: false\n- host: webservices.goascribe.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  1 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: voxco.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: goascribe.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/voxco/refs/heads/main/security/voxco-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Survey Software
- Market Research
- CATI
- Omnichannel
- Text Analytics
- Data Collection
- Panel Management
---
