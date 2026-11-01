---
api_specs:
- filename: pieterpost-com-openapi-generated.yml
  format: yaml
  label: pieterpost-com API
  slug: pieterpost-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pieterpost-com/openapi/_ae-authored/pieterpost-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: pieterpost.com
  spf: true
hosts:
- cert_expires: Jan  4 19:02:42 2027 GMT
  host: pieterpost.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Pieterpost Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for pieterpost-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: pieterpost-com
provider_slug: pieterpost-com
slug: pieterpost-com-domain-security
source_filename: pieterpost-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pieterpost.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 19:02:42 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: pieterpost.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/pieterpost-com/security/pieterpost-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Mail
- Postal
- Printing
- API
- Letters
- Postcards
---
