---
api_specs:
- filename: theidco-openapi-generated.yml
  format: yaml
  label: The ID API
  slug: theidco-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/theidco/openapi/_ae-authored/theidco-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: theidco.com
  spf: true
hosts:
- cert_expires: Dec 21 22:44:34 2026 GMT
  host: theidco.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Theidco Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for The ID, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: The ID
provider_slug: theidco
slug: theidco-domain-security
source_filename: theidco-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: theidco.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 21 22:44:34 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: theidco.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/theidco/security/theidco-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Credit Risk
- Open Banking
- Data Protection
---
