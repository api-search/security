---
api_specs:
- filename: dveracity-com-openapi-generated.yml
  format: yaml
  label: dVeracity API
  slug: dveracity-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dveracity-com/openapi/_ae-authored/dveracity-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: dveracity.com
  spf: true
hosts:
- cert_expires: Jan 11 10:53:10 2027 GMT
  host: dveracity.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Dveracity Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for dVeracity, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: dVeracity
provider_slug: dveracity-com
slug: dveracity-com-domain-security
source_filename: dveracity-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dveracity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 10:53:10 2027 GMT\n  hsts: false\ndomains:\n- domain: dveracity.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/dveracity-com/security/dveracity-com-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Emissions
- Verification
- Carbon Accounting
- Open Standard
---
