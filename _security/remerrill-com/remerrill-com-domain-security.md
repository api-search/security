---
api_specs:
- filename: remerrill-com-openapi.yml
  format: yaml
  label: R.E. Merrill Pump Line Finder API
  slug: pump-line-finder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/remerrill-com/refs/heads/main/openapi/remerrill-com-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: remerrill.com
  spf: true
hosts:
- cert_expires: Nov 17 21:42:02 2026 GMT
  host: remerrill.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Remerrill Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for R.E. Merrill & Associates, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: R.E. Merrill & Associates
provider_slug: remerrill-com
slug: remerrill-com-domain-security
source_filename: remerrill-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: remerrill.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 17 21:42:02 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: remerrill.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/remerrill-com/refs/heads/main/security/remerrill-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Industrial Pumps
- Pump Selection
- Industrial Equipment
- Chemical Processing
- Manufacturing
- Distribution
- Agents
- A2A
- Agent-Native
- Texas
- United States
---
