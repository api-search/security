---
api_specs:
- filename: klaxoon-openapi.yml
  format: yaml
  label: Klaxoon API
  slug: klaxoon-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/klaxoon/refs/heads/main/openapi/klaxoon-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: klaxoon.com
  spf: true
hosts:
- cert_expires: Oct 19 23:59:59 2026 GMT
  host: www.klaxoon.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 19:16:51 2026 GMT
  host: developers.klaxoon.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Klaxoon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Klaxoon, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Klaxoon
provider_slug: klaxoon
slug: klaxoon-domain-security
source_filename: klaxoon-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.klaxoon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 19 23:59:59 2026 GMT\n  hsts: false\n- host: developers.klaxoon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 19:16:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: klaxoon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/klaxoon/refs/heads/main/security/klaxoon-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Collaboration
- Meetings
- Productivity
- Team Collaboration
- Workshops
- Brainstorming
- Whiteboard
---
