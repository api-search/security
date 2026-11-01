---
api_specs:
- filename: foxnose-net-flux-openapi-generated.yml
  format: yaml
  label: foxnose-net flux API
  slug: flux-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/foxnose-net/openapi/_ae-authored/foxnose-net-flux-openapi-generated.yml
- filename: foxnose-net-management-openapi-generated.yml
  format: yaml
  label: foxnose-net management API
  slug: management-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/foxnose-net/openapi/_ae-authored/foxnose-net-management-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: foxnose.net
  spf: false
hosts:
- cert_expires: Dec 18 11:43:12 2026 GMT
  host: foxnose.net
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Foxnose Net Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for foxnose-net, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: foxnose-net
provider_slug: foxnose-net
slug: foxnose-net-domain-security
source_filename: foxnose-net-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: foxnose.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 11:43:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: foxnose.net\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/foxnose-net/security/foxnose-net-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- API
- Networking
- Security
- Integration
---
