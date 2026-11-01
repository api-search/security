---
api_specs:
- filename: 1099policy-com-openapi-generated.yml
  format: yaml
  label: 1099policy-com API
  slug: 1099policy-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/1099policy-com/openapi/_ae-authored/1099policy-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: 1099policy.com
  spf: true
hosts:
- cert_expires: Jan 13 11:46:22 2027 GMT
  host: 1099policy.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: 1099Policy Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 1099policy-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: 1099policy-com
provider_slug: 1099policy-com
slug: 1099policy-com-domain-security
source_filename: 1099policy-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: 1099policy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 11:46:22 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: 1099policy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/1099policy-com/security/1099policy-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Insurance
- Compliance
- Contractors
- API
- WorkersComp
---
