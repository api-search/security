---
api_specs:
- filename: monotype-openapi-generated.yml
  format: yaml
  label: Monotype API
  slug: monotype-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/monotype/openapi/_ae-authored/monotype-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: monotype.com
  spf: true
hosts:
- cert_expires: Dec 10 23:59:59 2026 GMT
  host: monotype.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Monotype Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Monotype, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Monotype
provider_slug: monotype
slug: monotype-domain-security
source_filename: monotype-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: monotype.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: monotype.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/monotype/security/monotype-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fonts
- Font Management
- Typography
- Creative Services
- Enterprise Software
- Licensing
---
