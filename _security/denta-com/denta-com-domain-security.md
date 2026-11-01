---
api_specs:
- filename: denta-com-openapi-generated.yml
  format: yaml
  label: Denta API
  slug: denta-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/denta-com/openapi/_ae-authored/denta-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: denta.com
  spf: true
hosts:
- cert_expires: Jan 20 19:41:37 2027 GMT
  host: denta.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Denta Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Denta, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Denta
provider_slug: denta-com
slug: denta-com-domain-security
source_filename: denta-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: denta.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 20 19:41:37 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: denta.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/denta-com/security/denta-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Dental
- Benefits
- SaaS
- Healthcare
- Employer
---
