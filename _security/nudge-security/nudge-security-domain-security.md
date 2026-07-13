---
api_specs:
- filename: nudge-security-openapi.yml
  format: yaml
  label: Nudge Security API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nudge-security/refs/heads/main/openapi/nudge-security-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: nudgesecurity.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: nudgesecurity.io
  spf: true
hosts:
- cert_expires: Sep  1 13:50:12 2026 GMT
  host: www.nudgesecurity.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 23:59:59 2026 GMT
  host: help.nudgesecurity.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 25 23:59:59 2027 GMT
  host: api.nudgesecurity.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nudge Security Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nudge Security, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Nudge Security
provider_slug: nudge-security
slug: nudge-security-domain-security
source_filename: nudge-security-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nudgesecurity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 13:50:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: help.nudgesecurity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 23:59:59 2026 GMT\n  hsts: false\n- host: api.nudgesecurity.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 25 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: nudgesecurity.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: nudgesecurity.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nudge-security/refs/heads/main/security/nudge-security-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Access Management
- AI Security
- Compliance
- Governance
- OAuth
- SaaS Management
- SaaS Security
- Security
- Shadow IT
- SSPM
---
