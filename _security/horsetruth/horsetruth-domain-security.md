---
api_specs:
- filename: horsetruth-openapi-generated.yml
  format: yaml
  label: Horse Truth API
  slug: horsetruth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/horsetruth/refs/heads/main/openapi/_ae-authored/horsetruth-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: horsetruth.com.au
  spf: false
hosts:
- cert_expires: Dec 24 22:21:59 2026 GMT
  host: horsetruth.com.au
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Horsetruth Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Horse Truth, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: Horse Truth
provider_slug: horsetruth
slug: horsetruth-domain-security
source_filename: horsetruth-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: horsetruth.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 22:21:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: horsetruth.com.au\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/horsetruth/refs/heads/main/security/horsetruth-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Racehorse Intelligence
- Horse Reports
- API
- Developers
- Trainers
---
