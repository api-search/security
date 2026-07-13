---
api_specs:
- filename: riiid-openapi.yml
  format: yaml
  label: Riiid Adaptive Learning
  slug: adaptive-learning
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/riiid/refs/heads/main/openapi/riiid-openapi.yml
- filename: riiid-openapi.yml
  format: yaml
  label: Riiid Knowledge Tracing
  slug: knowledge-tracing
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/riiid/refs/heads/main/openapi/riiid-openapi.yml
- filename: riiid-openapi.yml
  format: yaml
  label: Riiid Santa
  slug: santa
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/riiid/refs/heads/main/openapi/riiid-openapi.yml
- filename: riiid-openapi.yml
  format: yaml
  label: Riiid Partner Solutions
  slug: partner-solutions
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/riiid/refs/heads/main/openapi/riiid-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: riiid.com
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: socra.ai
  spf: true
hosts:
- cert_expires: Oct  2 23:59:59 2026 GMT
  host: www.riiid.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 08:12:15 2026 GMT
  host: corp.socra.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  7 19:46:05 2027 GMT
  host: apps.apple.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Riiid Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Riiid, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Riiid
provider_slug: riiid
slug: riiid-domain-security
source_filename: riiid-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.riiid.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: corp.socra.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 08:12:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: apps.apple.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 19:46:05 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: riiid.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: socra.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/riiid/refs/heads/main/security/riiid-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Education
- Adaptive Learning
- Knowledge Tracing
- EdTech
---
