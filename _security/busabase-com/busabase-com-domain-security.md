---
api_specs:
- filename: busabase-com-openapi.json
  format: json
  label: Busabase API
  slug: busabase-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/busabase-com/openapi/busabase-com-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: busabase.com
  spf: true
hosts:
- cert_expires: Jan 22 23:59:59 2027 GMT
  host: busabase.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: busabase-com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for busabase-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: busabase-com
provider_slug: busabase-com
slug: busabase-com-domain-security
source_filename: busabase-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: busabase.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 22 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: busabase.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/busabase-com/security/busabase-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- AI Agents
- Workspace
- Open Source
- Cloud
- Self-Hosted
---
