---
api_specs:
- filename: inboxapp-openapi-generated.yml
  format: yaml
  label: Inboxapp API
  slug: inboxapp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/inboxapp/openapi/_ae-authored/inboxapp-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: inboxapp.com
  spf: true
hosts:
- cert_expires: Jan 12 19:28:03 2027 GMT
  host: inboxapp.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Inboxapp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Inboxapp, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Inboxapp
provider_slug: inboxapp
slug: inboxapp-domain-security
source_filename: inboxapp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: inboxapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 19:28:03 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: inboxapp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/inboxapp/security/inboxapp-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- CRM
- Messaging
- Sales
- Collaboration
---
