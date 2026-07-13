---
api_specs:
- filename: runsignup-openapi.yml
  format: yaml
  label: RunSignup API
  slug: runsignup
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runsignup/refs/heads/main/openapi/runsignup-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: runsignup.com
  spf: true
hosts:
- cert_expires: Sep 24 09:23:57 2026 GMT
  host: runsignup.com
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Runsignup Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RunSignup, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: RunSignup
provider_slug: runsignup
slug: runsignup-domain-security
source_filename: runsignup-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: runsignup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 09:23:57 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\ndomains:\n- domain: runsignup.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/runsignup/refs/heads/main/security/runsignup-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Race Registration
- Event Management
- Running
- Sports
- Fitness
- Timing
- Fundraising
---
