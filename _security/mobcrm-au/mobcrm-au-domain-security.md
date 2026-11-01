---
api_specs:
- filename: mobcrm-au-openapi.yml
  format: yaml
  label: Mob CRM API
  slug: mob-crm-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mobcrm-au/openapi/mobcrm-au-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: mobcrm.au
  spf: true
hosts:
- cert_expires: Dec 14 23:02:29 2026 GMT
  host: mobcrm.au
  hsts: true
  hsts_max_age: 15724800
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Mobcrm Au Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for mobcrm-au, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: mobcrm-au
provider_slug: mobcrm-au
slug: mobcrm-au-domain-security
source_filename: mobcrm-au-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mobcrm.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 14 23:02:29 2026 GMT\n  hsts: true\n  hsts_max_age: 15724800\ndomains:\n- domain: mobcrm.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/mobcrm-au/security/mobcrm-au-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- CRM
- Personal Productivity
- Mobile
- Open Source
- Contact Management
---
