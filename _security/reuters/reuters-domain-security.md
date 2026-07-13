---
api_specs:
- filename: reuters-connect-api-openapi.yml
  format: yaml
  label: Reuters Connect API
  slug: reuters-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reuters/refs/heads/main/openapi/reuters-connect-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: reuters.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: reutersconnect.com
  spf: true
hosts:
- cert_expires: Nov 12 23:59:59 2026 GMT
  host: www.reuters.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 31 23:59:59 2026 GMT
  host: www.reutersconnect.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 23 23:59:59 2026 GMT
  host: rmb.reuters.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Reuters Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Reuters, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Reuters
provider_slug: reuters
slug: reuters-domain-security
source_filename: reuters-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.reuters.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.reutersconnect.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: rmb.reuters.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 23 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: reuters.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: reutersconnect.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reuters/refs/heads/main/security/reuters-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Business
- Finance
- Journalism
- Media
- News
- Wire Service
---
