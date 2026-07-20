---
api_specs:
- filename: accept-midas-openapi-original.yml
  format: yaml
  label: MIDAS API
  slug: midas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accept/refs/heads/main/openapi/accept-midas-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: accept.io
  spf: true
hosts:
- cert_expires: Aug 25 14:54:27 2026 GMT
  host: www.accept.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 23:59:59 2026 GMT
  host: midas.accept.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Accept Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Accept, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Accept
provider_slug: accept
slug: accept-domain-security
source_filename: accept-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.accept.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 14:54:27 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: midas.accept.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: accept.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/accept/refs/heads/main/security/accept-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Enterprise
- Governance
- AI Agents
- Authority
- Decision Governance
- Audit
- Open Source
---
