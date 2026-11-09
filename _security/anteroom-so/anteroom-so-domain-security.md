---
api_specs:
- filename: anteroom-so-openapi-generated.yml
  format: yaml
  label: Anteroom API
  slug: anteroom-so-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anteroom-so/openapi/_ae-authored/anteroom-so-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: anteroom.so
  spf: true
hosts:
- cert_expires: Jan 27 00:33:25 2027 GMT
  host: anteroom.so
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Anteroom So Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Anteroom, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Anteroom
provider_slug: anteroom-so
slug: anteroom-so-domain-security
source_filename: anteroom-so-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: anteroom.so\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 27 00:33:25 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: anteroom.so\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/anteroom-so/security/anteroom-so-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Legal Tech
- Compliance
- Regulations
- Startups
---
