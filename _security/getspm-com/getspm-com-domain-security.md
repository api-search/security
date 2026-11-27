---
api_specs:
- filename: getspm-com-openapi-generated.yml
  format: yaml
  label: SPM API
  slug: getspm-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getspm-com/openapi/_ae-authored/getspm-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: getspm.com
  spf: false
hosts:
- cert_expires: Dec 14 14:30:34 2026 GMT
  host: getspm.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: SPM Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SPM, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: SPM
provider_slug: getspm-com
slug: getspm-com-domain-security
source_filename: getspm-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getspm.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 14 14:30:34 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: getspm.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/getspm-com/security/getspm-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Project Memory
- Artificial Intelligence
- Collaboration
- Team Productivity
- Software-as-a-Service
---
