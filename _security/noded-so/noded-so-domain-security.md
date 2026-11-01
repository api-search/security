---
api_specs:
- filename: noded-so-openapi-generated.yml
  format: yaml
  label: Noded AI API
  slug: noded-so-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/noded-so/openapi/_ae-authored/noded-so-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: noded.so
  spf: true
hosts:
- cert_expires: Apr 25 23:59:59 2027 GMT
  host: noded.so
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Noded So Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Noded AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Noded AI
provider_slug: noded-so
slug: noded-so-domain-security
source_filename: noded-so-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: noded.so\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 25 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: noded.so\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/noded-so/security/noded-so-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- AI
- Customer-Data
- Context-Graph
- Integration
- Automation
- Company
---
