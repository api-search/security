---
api_specs:
- filename: 31huiyi-openapi.postman_collection.json
  format: json
  label: 31 OpenAPI
  slug: 31huiyi-openapi
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/31huiyi/refs/heads/main/postman/31huiyi-openapi.postman_collection.json
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: 31huiyi.com
  spf: true
hosts:
- cert_expires: Feb  3 01:53:21 2027 GMT
  host: www.31huiyi.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Feb  3 01:53:21 2027 GMT
  host: api-help.31huiyi.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Feb  3 01:53:21 2027 GMT
  host: 31api.31huiyi.com
  hsts: null
  https: true
  tls_version: TLSv1.2
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: 31Huiyi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 31huiyi, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: 31huiyi
provider_slug: 31huiyi
slug: 31huiyi-domain-security
source_filename: 31huiyi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.31huiyi.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb  3 01:53:21 2027 GMT\n  hsts: false\n- host: api-help.31huiyi.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb  3 01:53:21 2027 GMT\n  hsts: false\n- host: 31api.31huiyi.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb  3 01:53:21 2027 GMT\n  hsts: null\ndomains:\n- domain: 31huiyi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/31huiyi/refs/heads/main/security/31huiyi-domain-security.yml
summary_line: TLSv1.2
tags:
- Company
- Events
- Event Management
- Conferences
- Exhibitions
- Registration
- Check-In
- Scheduling
- Ticketing
- SaaS
- China
---
