---
api_specs:
- filename: ninetyio-openapi-original.json
  format: json
  label: Ninety Public API
  slug: ninety-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ninetyio/refs/heads/main/openapi/ninetyio-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ninety.io
  spf: true
hosts:
- cert_expires: Sep 25 07:32:20 2026 GMT
  host: www.ninety.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ninetyio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ninety.io, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Ninety.io
provider_slug: ninetyio
slug: ninetyio-domain-security
source_filename: ninetyio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ninety.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 07:32:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ninety.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ninetyio/refs/heads/main/security/ninetyio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- EOS
- Entrepreneurial Operating System
- Business Management
- Meetings
- Productivity
- Scorecard
- Team Management
- Goal Tracking
---
