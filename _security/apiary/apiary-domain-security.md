---
api_specs:
- filename: apiary-apiary-api-openapi.yml
  format: yaml
  label: Apiary API
  slug: apiary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apiary/refs/heads/main/openapi/apiary-apiary-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: apiary.io
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: apiblueprint.org
  spf: false
hosts:
- cert_expires: Mar  6 23:59:59 2027 GMT
  host: apiary.io
  hsts: true
  hsts_max_age: 604800
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 25 15:56:18 2026 GMT
  host: apiblueprint.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  6 23:59:59 2027 GMT
  host: api.apiary.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Apiary Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Apiary, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Apiary
provider_slug: apiary
slug: apiary-domain-security
source_filename: apiary-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: apiary.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  6 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 604800\n- host: apiblueprint.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 25 15:56:18 2026 GMT\n  hsts: false\n- host: api.apiary.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  6 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: apiary.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: apiblueprint.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apiary/refs/heads/main/security/apiary-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- API Blueprint
- API Design
- API Testing
- Collaboration
- Design-First
- Documentation
- Mock Servers
- Oracle
---
