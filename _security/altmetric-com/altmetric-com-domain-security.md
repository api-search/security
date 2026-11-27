---
api_specs:
- filename: altmetric-com-openapi-generated.yml
  format: yaml
  label: Altmetric API
  slug: altmetric-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/altmetric-com/openapi/_ae-authored/altmetric-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: altmetric.com
  spf: true
hosts:
- cert_expires: Dec 16 15:24:08 2026 GMT
  host: altmetric.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Altmetric Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Altmetric, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Altmetric
provider_slug: altmetric-com
slug: altmetric-com-domain-security
source_filename: altmetric-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: altmetric.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 16 15:24:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: altmetric.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/altmetric-com/security/altmetric-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Research
- Metrics
- Analytics
- Scholarly Communication
- Altmetrics
---
