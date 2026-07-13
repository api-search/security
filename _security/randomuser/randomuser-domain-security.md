---
api_specs:
- filename: randomuser-openapi.yml
  format: yaml
  label: Random User Generator API
  slug: randomuser
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/randomuser/refs/heads/main/openapi/randomuser-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: randomuser.me
  spf: true
hosts:
- cert_expires: Sep  7 10:12:55 2026 GMT
  host: randomuser.me
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Randomuser Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Random User Generator, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Random User Generator
provider_slug: randomuser
slug: randomuser-domain-security
source_filename: randomuser-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: randomuser.me\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 10:12:55 2026 GMT\n  hsts: false\ndomains:\n- domain: randomuser.me\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/randomuser/refs/heads/main/security/randomuser-domain-security.yml
summary_line: TLSv1.3
tags:
- Test Data
- Synthetic Data
- Mock Data
- Open Source
- Public API
- Free API
---
