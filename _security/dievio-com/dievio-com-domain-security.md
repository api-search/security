---
api_specs:
- filename: dievio-com-openapi-generated.yml
  format: yaml
  label: Dievio API
  slug: dievio-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dievio-com/openapi/_ae-authored/dievio-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: dievio.com
  spf: true
hosts:
- cert_expires: Dec 30 00:39:35 2026 GMT
  host: dievio.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Dievio Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dievio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Dievio
provider_slug: dievio-com
slug: dievio-com-domain-security
source_filename: dievio-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dievio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 00:39:35 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: dievio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/dievio-com/security/dievio-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- B2B
- Lead Generation
- Sales
- Marketing
- Data
---
