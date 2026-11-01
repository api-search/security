---
api_specs:
- filename: wolfram-openapi-generated.yml
  format: yaml
  label: Wolfram Research API
  slug: wolfram-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wolfram/openapi/_ae-authored/wolfram-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: wolfram.com
  spf: true
hosts:
- cert_expires: Apr 10 16:13:44 2027 GMT
  host: wolfram.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Wolfram Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wolfram Research, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Wolfram Research
provider_slug: wolfram
slug: wolfram-domain-security
source_filename: wolfram-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: wolfram.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 10 16:13:44 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: wolfram.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/wolfram/security/wolfram-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Computational
- Mathematics
- Cloud
---
