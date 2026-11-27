---
api_specs:
- filename: hamloy-com-openapi-generated.yml
  format: yaml
  label: Hamloy API
  slug: hamloy-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hamloy-com/openapi/_ae-authored/hamloy-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: hamloy.com
  spf: true
hosts:
- cert_expires: Jan  4 22:34:41 2027 GMT
  host: hamloy.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Hamloy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hamloy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Hamloy
provider_slug: hamloy-com
slug: hamloy-com-domain-security
source_filename: hamloy-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hamloy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 22:34:41 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: hamloy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/hamloy-com/security/hamloy-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
---
