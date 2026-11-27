---
api_specs:
- filename: mozg-sh-openapi-generated.yml
  format: yaml
  label: Mozg API
  slug: mozg-sh-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mozg-sh/openapi/_ae-authored/mozg-sh-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: mozg.sh
  spf: false
hosts:
- cert_expires: Feb 10 05:50:13 2027 GMT
  host: mozg.sh
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Mozg Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mozg, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Mozg
provider_slug: mozg-sh
slug: mozg-sh-domain-security
source_filename: mozg-sh-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mozg.sh\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 10 05:50:13 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: mozg.sh\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/mozg-sh/security/mozg-sh-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Platform
- Open Source
- MCP
---
