---
api_specs:
- filename: 1factory-openapi.json
  format: json
  label: 1Factory API
  slug: 1factory
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/1factory/refs/heads/main/openapi/1factory-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: 1factory.com
  spf: true
- caa: []
  dmarc: false
  dnssec: true
  domain: 1factory.co
  spf: false
hosts:
- cert_expires: Jan 13 23:59:59 2027 GMT
  host: www.1factory.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 13 23:59:59 2027 GMT
  host: www.1factory.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 14 11:39:46 2026 GMT
  host: val.1factory.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: 1Factory Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 1Factory, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: 1Factory
provider_slug: 1factory
slug: 1factory-domain-security
source_filename: 1factory-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.1factory.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.1factory.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: val.1factory.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 11:39:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: 1factory.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: 1factory.co\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/1factory/refs/heads/main/security/1factory-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Analytics
- Data Collection
- Manufacturing
- Monitoring
- Quality
---
