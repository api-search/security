---
api_specs:
- filename: nuzur-com-openapi-generated.yml
  format: yaml
  label: nuzur API
  slug: nuzur-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nuzur-com/openapi/_ae-authored/nuzur-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: nuzur.com
  spf: false
hosts:
- cert_expires: Feb 11 12:18:52 2027 GMT
  host: nuzur.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: nuzur Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for nuzur, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: nuzur
provider_slug: nuzur-com
slug: nuzur-com-domain-security
source_filename: nuzur-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nuzur.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 11 12:18:52 2027 GMT\n  hsts: false\ndomains:\n- domain: nuzur.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/nuzur-com/security/nuzur-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Database Schema Design
- Go Backend
- Code Generation
- Deploy
- AI Agents
- Open Source
---
