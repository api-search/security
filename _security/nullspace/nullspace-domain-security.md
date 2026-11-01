---
api_specs:
- filename: nullspace-openapi-generated.yml
  format: yaml
  label: Nullspace API
  slug: nullspace-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nullspace/openapi/_ae-authored/nullspace-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ns.rocks
  spf: true
hosts:
- cert_expires: Jan  7 17:05:55 2027 GMT
  host: ns.rocks
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Nullspace Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nullspace, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Nullspace
provider_slug: nullspace
slug: nullspace-domain-security
source_filename: nullspace-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ns.rocks\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 17:05:55 2027 GMT\n  hsts: false\ndomains:\n- domain: ns.rocks\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/nullspace/security/nullspace-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Cloud Infrastructure
- AI Agents
---
