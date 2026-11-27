---
api_specs:
- filename: achieved-io-openapi-generated.yml
  format: yaml
  label: Achieved.io API
  slug: achieved-io-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/achieved-io/openapi/_ae-authored/achieved-io-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: achieved.io
  spf: true
hosts:
- cert_expires: Mar 21 23:59:59 2027 GMT
  host: achieved.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Achieved.io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Achieved.io, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Achieved.io
provider_slug: achieved-io
slug: achieved-io-domain-security
source_filename: achieved-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: achieved.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 21 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: achieved.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/achieved-io/security/achieved-io-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Investor Relations
- Reporting
- Software-as-a-Service
---
