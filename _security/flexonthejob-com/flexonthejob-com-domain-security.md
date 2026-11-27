---
api_specs:
- filename: flexonthejob-com-openapi.yml
  format: yaml
  label: Flex API
  slug: flex-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flexonthejob-com/openapi/flexonthejob-com-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: flexonthejob.com
  spf: true
hosts:
- cert_expires: Dec 12 17:10:30 2026 GMT
  host: flexonthejob.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Flex on the Job Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Flex on the Job, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Flex on the Job
provider_slug: flexonthejob-com
slug: flexonthejob-com-domain-security
source_filename: flexonthejob-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: flexonthejob.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 17:10:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: flexonthejob.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/flexonthejob-com/security/flexonthejob-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Inventory
- Invoicing
- Job Management
- Construction
- Software-as-a-Service
- Company
---
