---
api_specs:
- filename: auravant-openapi-generated.yml
  format: yaml
  label: Auravant API
  slug: auravant-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/auravant/openapi/_ae-authored/auravant-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: auravant.com
  spf: true
hosts:
- cert_expires: Jan 18 11:49:13 2027 GMT
  host: www.auravant.com
  hsts: true
  hsts_max_age: 10886400
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Auravant Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Auravant, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Auravant
provider_slug: auravant
slug: auravant-domain-security
source_filename: auravant-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.auravant.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 18 11:49:13 2027 GMT\n  hsts: true\n  hsts_max_age: 10886400\ndomains:\n- domain: auravant.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/auravant/security/auravant-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Agriculture
- Digital Platform
- Precision Agriculture
- Sustainability
- Company
---
