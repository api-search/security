---
api_specs:
- filename: doingwork-work-status-api-openapi.yml
  format: yaml
  label: doingwork-work Status API
  slug: doingwork-work-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/doingwork-work/openapi/doingwork-work-status-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: doingwork.work
  spf: true
hosts:
- cert_expires: Dec 23 18:05:41 2026 GMT
  host: doingwork.work
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Doingwork Work Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for doingwork-work, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: doingwork-work
provider_slug: doingwork-work
slug: doingwork-work-domain-security
source_filename: doingwork-work-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: doingwork.work\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 18:05:41 2026 GMT\n  hsts: false\ndomains:\n- domain: doingwork.work\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/doingwork-work/security/doingwork-work-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Field Service
- Invoicing
- API
- Mobile
---
