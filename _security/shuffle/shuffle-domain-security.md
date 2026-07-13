---
api_specs:
- filename: shuffle-openapi.yml
  format: yaml
  label: Shuffle API
  slug: shuffle-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shuffle/refs/heads/main/openapi/shuffle-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: shuffler.io
  spf: true
hosts:
- cert_expires: Sep 11 06:58:48 2026 GMT
  host: shuffler.io
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Shuffle Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Shuffle, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Shuffle
provider_slug: shuffle
slug: shuffle-domain-security
source_filename: shuffle-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: shuffler.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 06:58:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\ndomains:\n- domain: shuffler.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shuffle/refs/heads/main/security/shuffle-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Security
- Workflows
- Automation
- SOAR
- Orchestration
- Open Source
---
