---
api_specs:
- filename: buggazi-com-openapi-generated.yml
  format: yaml
  label: Buggazi API
  slug: buggazi-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buggazi-com/openapi/_ae-authored/buggazi-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: buggazi.com
  spf: true
hosts:
- cert_expires: Dec 14 10:29:41 2026 GMT
  host: buggazi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Buggazi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Buggazi, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Buggazi
provider_slug: buggazi-com
slug: buggazi-com-domain-security
source_filename: buggazi-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: buggazi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 14 10:29:41 2026 GMT\n  hsts: false\ndomains:\n- domain: buggazi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/buggazi-com/security/buggazi-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Project Management
- Bug Tracking
- Sprint Planning
- AI Coding Agents
- Collaboration
---
