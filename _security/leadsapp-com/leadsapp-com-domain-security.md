---
api_specs:
- filename: leadsapp-com-openapi-generated.yml
  format: yaml
  label: LeadsApp API
  slug: leadsapp-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/leadsapp-com/openapi/_ae-authored/leadsapp-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: leadsapp.com
  spf: true
hosts:
- cert_expires: Dec 27 23:05:32 2026 GMT
  host: leadsapp.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: LeadsApp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LeadsApp, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: LeadsApp
provider_slug: leadsapp-com
slug: leadsapp-com-domain-security
source_filename: leadsapp-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: leadsapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 23:05:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: leadsapp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/leadsapp-com/security/leadsapp-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Lead Management
- Automation
- Software-as-a-Service
- CRM
---
