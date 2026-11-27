---
api_specs:
- filename: intellischool-openapi-generated.yml
  format: yaml
  label: Intellischool API
  slug: intellischool-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/intellischool/openapi/_ae-authored/intellischool-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: intellischool.co
  spf: true
hosts:
- cert_expires: Jan 16 07:56:52 2027 GMT
  host: intellischool.co
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Intellischool Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Intellischool, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Intellischool
provider_slug: intellischool
slug: intellischool-domain-security
source_filename: intellischool-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: intellischool.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 16 07:56:52 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: intellischool.co\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/intellischool/security/intellischool-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Education
- Artificial Intelligence
- Data
- Software-as-a-Service
- K-12
---
