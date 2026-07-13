---
api_specs:
- filename: guru-openapi.yml
  format: yaml
  label: Guru REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/guru/refs/heads/main/openapi/guru-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: getguru.com
  spf: true
hosts:
- cert_expires: Sep 29 22:19:48 2026 GMT
  host: www.getguru.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 13:01:58 2026 GMT
  host: developer.getguru.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 15 23:59:59 2026 GMT
  host: api.getguru.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Guru Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Guru, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Guru
provider_slug: guru
slug: guru-domain-security
source_filename: guru-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.getguru.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 22:19:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.getguru.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 13:01:58 2026 GMT\n  hsts: null\n- host: api.getguru.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: getguru.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/guru/refs/heads/main/security/guru-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Knowledge Management
- Enterprise Search
- AI Knowledge Base
- Internal Wiki
- Verified Knowledge
- Workplace Productivity
---
