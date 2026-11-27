---
api_specs:
- filename: criminal-ip-openapi-generated.yml
  format: yaml
  label: Criminal IP API
  slug: criminal-ip-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/criminal-ip/openapi/_ae-authored/criminal-ip-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: criminalip.io
  spf: true
hosts:
- cert_expires: Feb 13 16:35:35 2027 GMT
  host: criminalip.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Criminal IP Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Criminal IP, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Criminal IP
provider_slug: criminal-ip
slug: criminal-ip-domain-security
source_filename: criminal-ip-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: criminalip.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 13 16:35:35 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: criminalip.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/criminal-ip/security/criminal-ip-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Threat Intelligence
- Cybersecurity
- Data
---
