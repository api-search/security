---
api_specs:
- filename: nebulock-openapi.yml
  format: yaml
  label: Nebulock Public API
  slug: nebulock-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nebulock/refs/heads/main/openapi/nebulock-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: nebulock.io
  spf: true
hosts:
- cert_expires: Oct  2 08:59:20 2026 GMT
  host: nebulock.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 28 23:59:59 2027 GMT
  host: api.nebulock.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nebulock Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nebulock, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Nebulock
provider_slug: nebulock
slug: nebulock-domain-security
source_filename: nebulock-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nebulock.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 08:59:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.nebulock.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 28 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: nebulock.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nebulock/refs/heads/main/security/nebulock-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Security
- Threat Hunting
- Threat Detection
- Security Operations
- Detection Engineering
- AI Agents
- SIEM
---
