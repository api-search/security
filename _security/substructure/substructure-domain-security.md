---
api_specs:
- filename: substructure-openapi-generated.yml
  format: yaml
  label: Substructure API
  slug: substructure-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/substructure/openapi/_ae-authored/substructure-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: substructure.ai
  spf: true
hosts:
- cert_expires: Jan  1 20:57:55 2027 GMT
  host: substructure.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Substructure Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Substructure, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Substructure
provider_slug: substructure
slug: substructure-domain-security
source_filename: substructure-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: substructure.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 20:57:55 2027 GMT\n  hsts: false\ndomains:\n- domain: substructure.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/substructure/security/substructure-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Artificial Intelligence
- Agents
- Cloud-Native
- Automation
---
