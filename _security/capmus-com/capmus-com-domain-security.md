---
api_specs:
- filename: capmus-com-public-api-openapi.yml
  format: yaml
  label: Capmus Public API
  slug: capmus-com-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/capmus-com/openapi/capmus-com-public-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: capmus.com
  spf: true
hosts:
- cert_expires: Jan 24 17:50:44 2027 GMT
  host: capmus.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Capmus Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Capmus, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Capmus
provider_slug: capmus-com
slug: capmus-com-domain-security
source_filename: capmus-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: capmus.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 24 17:50:44 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: capmus.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/capmus-com/security/capmus-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Marketplace
- Classifieds
- Students
- Universities
- Housing
- Job
- Education
---
