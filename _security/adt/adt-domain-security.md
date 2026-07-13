---
api_specs:
- filename: adt-platform-api-openapi.yml
  format: yaml
  label: ADT+ Platform API
  slug: adt-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adt/refs/heads/main/openapi/adt-platform-api-openapi.yml
- filename: adt-business-api-openapi.yml
  format: yaml
  label: ADT Business API
  slug: adt-business-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adt/refs/heads/main/openapi/adt-business-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: adt.com
  spf: true
hosts:
- cert_expires: Dec 27 23:59:59 2026 GMT
  host: www.adt.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  9 23:59:59 2027 GMT
  host: api.adt.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Adt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ADT, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: ADT
provider_slug: adt
slug: adt-domain-security
source_filename: adt-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.adt.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.adt.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: adt.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adt/refs/heads/main/security/adt-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Access Control
- Automation
- Home Security
- IoT
- Monitoring
- Security
- Smart Home
- Fortune 1000
---
