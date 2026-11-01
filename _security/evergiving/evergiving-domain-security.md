---
api_specs:
- filename: evergiving-openapi-generated.yml
  format: yaml
  label: EverGiving API
  slug: evergiving-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evergiving/openapi/_ae-authored/evergiving-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: evergiving.com
  spf: true
hosts:
- cert_expires: Dec 19 16:19:09 2026 GMT
  host: evergiving.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Evergiving Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EverGiving, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: EverGiving
provider_slug: evergiving
slug: evergiving-domain-security
source_filename: evergiving-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: evergiving.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 16:19:09 2026 GMT\n  hsts: false\ndomains:\n- domain: evergiving.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/evergiving/security/evergiving-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Fundraising
- Nonprofit
- API
- Integration
---
