---
api_specs:
- filename: getdoloop-com-openapi-generated.yml
  format: yaml
  label: DoLoop API
  slug: getdoloop-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getdoloop-com/openapi/_ae-authored/getdoloop-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: getdoloop.com
  spf: true
hosts:
- cert_expires: Feb  3 17:18:32 2027 GMT
  host: getdoloop.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: DoLoop Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DoLoop, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: DoLoop
provider_slug: getdoloop-com
slug: getdoloop-com-domain-security
source_filename: getdoloop-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getdoloop.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  3 17:18:32 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: getdoloop.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/getdoloop-com/security/getdoloop-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Productivity
- Task Management
- Automation
- Personal Development
- Software-as-a-Service
---
