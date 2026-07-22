---
api_specs:
- filename: p0-security-jit-openapi.yml
  format: yaml
  label: P0 Just-in-Time Access API
  slug: p0-security-jit
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/p0-security/refs/heads/main/openapi/p0-security-jit-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: p0.dev
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: p0.app
  spf: false
hosts:
- cert_expires: Sep  5 16:33:47 2026 GMT
  host: docs.p0.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 13 09:56:44 2026 GMT
  host: api.p0.app
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: P0 Security Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for P0 Security, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: P0 Security
provider_slug: p0-security
slug: p0-security-domain-security
source_filename: p0-security-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.p0.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 16:33:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.p0.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 09:56:44 2026 GMT\n  hsts: false\ndomains:\n- domain: p0.dev\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: p0.app\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/p0-security/refs/heads/main/security/p0-security-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Security
- Privileged Access Management
- Identity and Access Management
- Just-in-Time Access
- Cloud Security
- Authorization
- Zero Trust
- Agentic Access
- MCP
---
