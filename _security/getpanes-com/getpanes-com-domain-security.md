---
api_specs:
- filename: getpanes-com-openapi-generated.yml
  format: yaml
  label: Panes API
  slug: getpanes-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getpanes-com/openapi/_ae-authored/getpanes-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: getpanes.com
  spf: false
hosts:
- cert_expires: Jan 30 22:11:35 2027 GMT
  host: getpanes.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Panes Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Panes, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Panes
provider_slug: getpanes-com
slug: getpanes-com-domain-security
source_filename: getpanes-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getpanes.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 30 22:11:35 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: getpanes.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/getpanes-com/security/getpanes-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Private Feed
- Automation
- Developer Tools
---
