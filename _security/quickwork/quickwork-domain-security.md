---
api_specs:
- filename: quickwork-embedded-api-openapi.yml
  format: yaml
  label: Quickwork Embedded API
  slug: quickwork-embedded-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/quickwork/openapi/quickwork-embedded-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: quickwork.co
  spf: true
hosts:
- cert_expires: Apr 27 23:59:59 2027 GMT
  host: quickwork.co
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Quickwork Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Quickwork, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Quickwork
provider_slug: quickwork
slug: quickwork-domain-security
source_filename: quickwork-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: quickwork.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 27 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: quickwork.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/quickwork/security/quickwork-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Integration
- Automation
- Workflows
- API Platform
- Enterprise
---
