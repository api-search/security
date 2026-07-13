---
api_specs:
- filename: abilityone-procurement-list-api-openapi.yml
  format: yaml
  label: AbilityOne Procurement List API
  slug: procurement-list-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-abilityone-commission/refs/heads/main/openapi/abilityone-procurement-list-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: abilityone.gov
  spf: true
hosts:
- cert_expires: Jan 30 23:59:59 2027 GMT
  host: www.abilityone.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 30 23:59:59 2027 GMT
  host: plims.abilityone.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Us Abilityone Commission Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for US AbilityOne Commission, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: US AbilityOne Commission
provider_slug: us-abilityone-commission
slug: us-abilityone-commission-domain-security
source_filename: us-abilityone-commission-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.abilityone.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 30 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: plims.abilityone.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 30 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: abilityone.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/us-abilityone-commission/refs/heads/main/security/us-abilityone-commission-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Federal Government
- Disability Employment
- Procurement
- Nonprofit
- Accessibility
---
